# Node application 
1. application can be web-service (REST API) or web application
   
   web application returns HTML page
   web applications are used by humans
   web applications are harder to test. Selenium is used to test web-applications.


   web-services returns application-data in JSON format
   web-services are consumed by applications/bots
   usually tested with POSTMAN tool by humans
   API testing is easier than testing the web-applications


2. developer workstation setup

   install node
   use visual code editor 
   
   we will develop web-service
   we will use javascript webframework called express

   npm is used to install node modules
   javascript is used as programming language

   node is used as runtime to run the javascript + express web-service application

3. Dockerfile 
   
   package the web-service application as container image
   upload the docker image to docker-hub (public repository)

4. we will use github as remote git repository

   web-service application code will be committed to public github repository


5. code base to have helmfile

   helmfile > chart-name to use > release name > values

6. web-service will be deployed into kubernetes as helm release

7. docker build, tag, push
8. Dockerfile in the github repo
9. .dockerignore in the github repo
10. k8s deployment manifest in the github repo
11. k8s service manifest in the github repo
12. helm chart in the github repo
    
    helm create <name-of-chart> # creates a folder with chart-name
    helm install <release-name> <chart-name/chart-folder-path>
    helm upgrade <release-name> <chart-name/local-chart-folder-path>
    helm list # list the releases in the cluster 