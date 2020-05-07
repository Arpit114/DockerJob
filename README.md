# DockerJob
TASK
There is a system of Developer side , Quality Assurance side , Client side. 
When Developer writes a code and commits it over Github ,it is forwarded to the Quality Aassurance side for testing . 
If tested OK , the developer code is de[ployed on the Client Side webpage .
Job 1 Jenkins:
When the Developer writes a code in a developer branch(dev) on his local Git repository(git) and uploads it to the Github , 
Jenkins get that code and deploy on the Quality Assurance Team Environment on Docker server (Testing) .
Job 2 : Jenkins
Create the Client side Docker environment for displaying the changes in the Master branch , 
these changes are carried out by the Job 3. This is the website which is live to the clients.
Job 3 : Jenkins
This is Triggered by the Quality assurance team if the developer's code is correct .
The Quality Test is triggered and it merges the Developer changes to the Master branch and then runs the Job 2 to display those change on the Client side.
