# Postgres-Docker
# Docker Installation 
The steps for installing Docker can be found here:
  [Docker Installation](https://github.com/syntaxboard/docker-installation)
# Git Installtion 
The steps for installing Git can be found here:
  [Git Installation](https://github.com/syntaxboard/git-installtion)
# Building the Docker
1. Create a directory on the local system and call it mysql.
  ![image](https://user-images.githubusercontent.com/51730523/175397289-13dc6e85-fc9e-482c-9d9e-313412986cd7.png)
2. Clone the mysql repository to that folder.
  ![image](https://user-images.githubusercontent.com/51730523/175397784-8c7895c8-93c5-40d7-ac88-2d67f6b95f7f.png)
  ![image](https://user-images.githubusercontent.com/51730523/175398164-7fbb400e-67d9-4fa7-b99d-4a4a3496d6b7.png)
3. To get the latest changes on the repository.
   ![image](https://user-images.githubusercontent.com/51730523/175399685-61d0eb7d-04bd-42f4-8efe-2f067a5940a1.png)
4. Open commmad prompt and run the Docker command from mysql as required.

## Command to run the docker in the background
   ```
   docker-compose up --d
   ```
## Command to remove the container 
   ```
   docker-compose down
   ```
## Command to force the docker recreate the image and container
   ```
   docker-compose up --force-recreate "Service Name Specified in the docker in this case it db"
   ```
## Command to list all the containers
   ```
   docker ps  -a
   ```
## Command to force remove the container
   ```
   docker ps  -a
   docker rm --force "conatiner_id" from the above command.
   ```

## Creating and filling a Postgres DB with Docker Compose
A PostgreSQL database is created and filled with tables in this project.Tables and data are stored in the sql folder.

## Parameteres for Docker Compose
| Parameter          | Description|
| :---               |:----  | 
| POSTGRES_USER      |user name to connect postgres|
| POSTGRES_PASSWORD  |password to connect postgres|        
| POSTGRES_DB        |database name|
| Port               |On the host, use the port 5432, which is mapped by Postgres as 5432 in your container| 

## Running the Docker Compose File
```
$ docker-compose up
```
