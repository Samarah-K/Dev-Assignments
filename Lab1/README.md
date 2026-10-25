Exercise 1: Hello Pod
Goal: Run your first app inside Kubernetes and access it.

Pre-Requisites
Install Minikube (one-time setup)

On Windows (PowerShell, run as Administrator):
choco install minikube

You need Docker or a VM driver (VirtualBox, Hyper-V) installed.

Steps: Deploy Ngnix Image as a Pod
Start a local Kubernetes cluster with Minikube:
minikube start
Create your first Pod (using Nginx image):
kubectl run hello-k8s --image=nginx --port=80
Verify the Pod is running:
kubectl get pods
Expose the Pod as a Service:
kubectl expose pod hello-k8s --type=NodePort --port=80
Open the app in your browser:
minikube service hello-k8s
You should see the Nginx welcome page. Congratulations, you just deployed your first container in Kubernetes!