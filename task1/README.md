# Running a Docker continer

In this we are going to run a Docker container to run the todo application

Steps followed:

Step1: Create a ubuntu machine

Step2: Install docker using below command
```bash
sudo apt-get update -y
sudo apt-get install docker.io -y
```

![image](https://user-images.githubusercontent.com/98816965/234772060-f1f87bfc-aa18-4e74-b13b-c6a29b86f4bf.png)


Step3: Create a Docker file for running the application of todo. For the docker file [click](https://github.com/sanket363/internship-tasks/blob/main/task1/Dockerfile) here

Step4: After the File is ready run the container using below command:
```bash
docker build -t todo-app:latest
```

![image](https://user-images.githubusercontent.com/98816965/234772123-fa546007-175c-4283-a8e9-68cad8322e3d.png)


Step5: Once the build is complete now run the container using below command:
```bash
docker run -d -p 8000:8000 todo-app:latest
```

Step6: Now you can navigate to browser and paste the below url you will access your application
```bash
http://<public-ip>:8000
```

![image](https://user-images.githubusercontent.com/98816965/234772266-725e0f51-1b2f-4c8c-a798-94145e056915.png)

