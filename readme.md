# My Deployment Process:
1. I created a repository on dockerhub.
2. After creating the file, From my project termina, I built the docker file with

    `docker build -t <hub-user>/<repo-name>[:<tag>`

    `docker build -t sca-exercise:v1 .`

3. I committed all changes to docker repository created using the command below. existing container will be replaced with the container ID, hub-user will be replaced with dockerhub username, repo-name wil be replaced with the repository name created on dockerhub. tag will be replaced with tag version. 

    `docker commit <existing-container> <hub-user>/<repo-name>[:<tag>]`
4. To get the container ID, run the command below

    `docker container ls`

5. After I commited, I pushed the commited changes to the respository created using the command below

    `docker push <hub-user>/<repo-name>:<tag>`

# Link to my docker hub repository 
#### https://hub.docker.com/repository/docker/fatimaola1/sca-cloud-exercise  
