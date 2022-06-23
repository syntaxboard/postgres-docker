# Installing Git
[Git for Windows](https://git-scm.com/download/win)

# postgres-docker

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
