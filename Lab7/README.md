Lab 7 - Introduction to Continuous Integration and Jenkins
Objective
Understand Continuous Integration (CI) and install Jenkins using Docker.

Topics
Continuous Integration
Jenkins
CI Workflow
Jenkins Installation with Docker

Rememeber:
1. Go Back to the Job

Click:

Plain Text
Lab7-CI-Demo

Then:

Plain Text
Configure
2. Remove the Current Build Step

Under Build Steps, delete:

Plain Text
Execute Windows batch command
3. Add Correct Build Step

Click:

Plain Text
Add build step

Choose:

Plain Text
Execute shell
``

(not Windows batch command)

4. Enter This
Shell
echo "Jenkins CI Pipeline Running"
echo "Build Successful"

Save.

5. Build Again

Click:

Plain Text
Build Now

Then open:

Plain Text
Build #2
→ Console Output