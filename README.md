## Setting Up Git and Docker 

### Requirements:

1. [Github Account](https://github.com)
2. [Heroku Account](https://id.heroku.com/login)
3. [VSCode IDE](https://code.visualstudio.com/)
4. [GIT Cli](https://git-scm.com/downloads)


### Steps:
1. Check your systemm variables for Conda path
2. Use command prompt (cmd) in terminal t execute the below syntax
3. creating conda environment
```
conda create -p venv python==3.7 -y
```

```
conda activate venv/
```
4. Create requirements.txt out of venv and list all the required libraries for the project
5. cmd cd.. for getting out of venv and follow the command
```
pip install -r requirements.txt
```


> Few Git Commands used in the process:
1. ``` git add .``` ---> to commit all files
2. ``` git status``` ---> to check the status (staged or committed)
3. ``` git log``` ---> to check the hashes of commits, author and date
4. ``` git commit -m "message"``` ---> writing the changes 
5. ``` git remote -v``` ---> To check remote url
6. ``` git branch``` ---> to check the branch name to push
7. ``` git push origin main``` ---> push it to the main branch

### To Setup CI/CD Pipeline in Heroku
1. HEROKU_EMAIL = sandeepiit.ism@gmail.com
2. HEROKU_API_KEY = ***************************
3. HEROKU_APP_NAME = mlapp-v1.0

### Create Dockerfile
1. create dockerfile and .dockerignore
2. cmd ---> ``` docker --version```
3. ``` docker status```
4. Build docker image:
``` 
docker build -t <image_name>:<tagname> .
```
5. To list docker images:
```
docker images
```
6. To Run the docker image:
```
docker run -p 5000:5000 -e PORT=5000 45c4548c7725
```
7. To check running containers:
```
docker ps
```

8. To Stop docker container:
```
docker stop container_id 
``` <e9c6>
