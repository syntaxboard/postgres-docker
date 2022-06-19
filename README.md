# Installing Git
[Git for Windows](https://git-scm.com/download/win)
# Installing Docker
## Docker Windows
## Download Docker Desktop for Windows
[Docker Desktop for Windows](https://desktop.docker.com/win/main/amd64/Docker%20Desktop%20Installer.exe)
## Install interactively
1. Double-click Docker Desktop Installer.exe to run the installer.
![image](https://user-images.githubusercontent.com/51730523/174503709-5eb96362-797a-4c95-9d8e-99a39de3497d.png)

2. Follow the instructions on the installation wizard to authorize the installer and proceed with the install.
3. When the installation is successful, click Close to complete the installation process.
4. If you get WSL2 installation is in complete error
![image](https://user-images.githubusercontent.com/51730523/174503480-da66df95-6c0d-4832-87a9-dec2005f1c16.png)
![image](https://user-images.githubusercontent.com/51730523/174503525-b9bcae75-4ff6-4184-80a1-1b0267c56fc4.png)
![image](https://user-images.githubusercontent.com/51730523/174503528-cf5a5666-2ab5-4e58-9699-fd87f7db95a9.png)
![image](https://user-images.githubusercontent.com/51730523/174503534-6d450057-50b4-444f-9b9e-f73a0d9a19c3.png)
![image](https://user-images.githubusercontent.com/51730523/174503537-2e785c6f-998d-4cc9-b517-6aaa0d916b83.png)
![image](https://user-images.githubusercontent.com/51730523/174503542-f50193ad-4646-474d-a672-caaefc5da557.png)
5. Download the Linux kernel update package
[Linux kernel update](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi)

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
