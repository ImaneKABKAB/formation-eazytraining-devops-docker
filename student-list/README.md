# 🧾Project theme

The project aims to :
✔ Containerize a simple application .
✔ Automate the deployement infrastructure using Iac approach.
✔ Push the application image to a Docker private registry.
The application lists the students with their  ages using a webserver (PHP) and an API (Flask).
I list through this repo all the process for accomplishing the project  

# 🔧Build and Test 
At this step , we will build a Docker image for the student_age api and to do so we will write a Dockerfile 
(https://github.com/ImaneKABKAB/formation-eazytraining-devops-docker/blob/main/student-list/simple_api/Dockerfile) where we specify the libraries , dependecies and the source file of the app .
To test it we use the curl command and we should see as an output the students list with ages as in the follow image 
(https://github.com/ImaneKABKAB/formation-eazytraining-devops-docker/blob/main/images/stu7.png) .

# ⚙️Infrastructure automation
At this phsase , we deploy the application using Iac approach by writing a docker-compose.yml file
(https://github.com/ImaneKABKAB/formation-eazytraining-devops-docker/blob/main/student-list/docker-compose.yml).

The application is devided into 2 services :
 - API service : it represents the api 
 - Website service : it represents the user interface 
 We put the 2 services in the same network of type bridge .
 We have as result  a site as the follow image (https://github.com/ImaneKABKAB/formation-eazytraining-devops-docker/blob/main/images/app.png)

# ⚠️ Private registry
We build a Docker private registry to store the produced images .
We create 2 containers :
 - Registry backend container where we store images 
 - Registry user interface  to facilitate managing the images
 To do so we use this docker-compose.yml file https://github.com/ImaneKABKAB/formation-eazytraining-devops-docker/blob/main/private-registry/docker-compose.yml
 Here is the result image https://github.com/ImaneKABKAB/formation-eazytraining-devops-docker/blob/main/images/TP8.png
 https://github.com/ImaneKABKAB/formation-eazytraining-devops-docker/blob/main/images/TP81.png
