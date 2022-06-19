# Installing Git
[Git for Windows](https://git-scm.com/download/win)
# Installing Docker
## Docker Windows
## Download Docker Desktop for Windows
[Docker Desktop for Windows](https://desktop.docker.com/win/main/amd64/Docker%20Desktop%20Installer.exe)
## Install interactively
1. Double-click Docker Desktop Installer.exe to run the installer.
2. When prompted, ensure the Use WSL 2 instead of Hyper-V option on the Configuration page is selected or not depending on your choice of backend.
3. Follow the instructions on the installation wizard to authorize the installer and proceed with the install.
4. When the installation is successful, click Close to complete the installation process.
5. If your admin account is different to your user account, you must add the user to the docker-users group. Run Computer Management as an administrator and navigate to Local Users and Groups > Groups > docker-users. Right-click to add the user to the group. Log out and log back in for the changes to take effect.
## Install from the command line
### After downloading Docker Desktop Installer, run the following command in a terminal to install Docker Desktop:
```
"Docker Desktop Installer.exe" install
```
```
start /w "" "Docker Desktop Installer.exe" install
```
If your admin account is different to your user account, you must add the user to the docker-users group:
```
net localgroup docker-users <user> /add
```
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
