# ITI - Docker Lab 🐋

## Task 1: Working with Docker Hello-world Image
### Objective
Learn how to run a container using the hello-world image and manage containers and images.

### Steps
#### 1. Run a Container with hello-world Image
```bash
```
docker pull hello-world
docker run hello-world
#### 2. Check Container Status and Explain
```bash
```
docker ps -a
output : Exited
Explanation : docker stops the container as its job is complete

#### 3. Start the Stopped Container
```bash
```
docker ps -a 
docker start gifted_matsumoto 
#### 4. Remove the Container
```bash
``` 
docker stop gifted_matsumoto
remove gifted_matsumoto
#### 5. Remove the Image
```bash
```
docker rmi  gifted_matsumoto
---

## Task 2: Running Container with Ubuntu Image
### Objective
Run an Ubuntu container in interactive mode, create a file inside it, and manage containers.

### Steps
#### 1. Run Ubuntu Container in Interactive Mode
```bash
```
docker run -it ubuntu
#### 2. Create a File inside the Container
```bash
```
touch hello-ubuntu
echo 'hello ubuntu form mansoura'>> hello-ubuntu
#### 3. Stop and Remove the Container
```bash
```
docker ps -a 
docker stop pensive_jemison
docker rm pensive_jemison
#### 4. Check File Status
```bash
```
ls hello-ubuntu
ls: hello-ubuntu: No such file or directory >>cuz the container is removed 

#### 5. What happened to hello-docker file?
```bash
```
it was removed cuz the conatiner has been removed
#### 6. Remove All Stopped Containers
```bash
```
docker container prune
#### 7. Bonus: Remove All Containers in One Command
```bash
```
docker rm -f $(docker ps -aq)
---
## Task 3: Creating a Custom Nginx Docker Image
### Objective
Create a custom Docker image using Nginx and a local HTML file.

### Steps
#### 1. Create a Local HTML File
```bash
```
#### 2. Write Dockerfile and Copy the HTML file to the Docker Image
```bash
```
#### 3. Run Container with New Image
```bash
```

#### 4. Test the Container, open your browser and navigate to http://localhost:8088 to check if everything is okay
```bash
```

