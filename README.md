# postgres-docker

# Creating and filling a Postgres DB with Docker Compose
This project create tables and fill the tables in a Postgres data base. The tables and data that create are in sql/ folder

# Parameteres for Docker Compose
| Parameter          | Description|
| :---               |:----  | 
| POSTGRES_USER      |user name to connect postgres|
| POSTGRES_PASSWORD  |password to connect postgres|        
| POSTGRES_DB        |database name|
| Port               |port mapped by Postgres is 5432 in your container.use the port 5438 on the host machine| 

# Running the Docker Compose File
```
$ docker-compose up
```
