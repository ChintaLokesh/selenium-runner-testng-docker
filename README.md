# selenium-runner-testng-docker
Integrated TestNG Automation project  with the Docker 



This project illustrates on how to run the Docker Automation Scripts / Framework using Docker Engine with the use of Docker Containers 
Docker Automation Framework is integrated with TEST NG 

jenkins file contains the pipeline scripts required to execute step by step in jenkins

steps used to run the Automation tests in Jenkins

Customized Docker Image is created for the Automation Framework
once the Docker Image is created , added the Docker image for execution in docker-compose.yaml file
This framework uses Selenium GRID to run the tests



After Automation Execution : 

Target folder contains all the reports including the screenshots
After successful execution of test scripts , Volume mapping is done and the target folder of Docker Container is shared to local machine ( or Jenkins Machine ) 

