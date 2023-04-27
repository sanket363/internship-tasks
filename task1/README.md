# Running a Docker continer

In this we are going to run a Docker container to run the todo application

Steps followed:

Step1: Create a ubuntu machine

Step2: Install docker using below command
```bash
sudo apt-get update -y
sudo apt-get install docker.io -y
```

Step3: Create a Docker file for running the application of todo. For the docker file [click](https://github.com/sanket363/internship-tasks/blob/main/task1/Dockerfile) here

Step4: After the File is ready run the container using below command:
```bash
docker build -t todo-app:latest
```

Step5: Once the build is complete now run the container using below command:
```bash
docker run -d -p 8000:8000 todo-app:latest
```

Step6: Now you can navigate to browser and paste the below url you will access your application
```bash
http://<public-ip>:8000
```
