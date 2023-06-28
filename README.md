# Zabbix Monitoring in Docker Containers

This project provides a Docker-based installation of the Zabbix monitoring system. Zabbix is a powerful tool for monitoring various IT components, including networks, servers, virtual machines, and cloud services.

## Installation

### Linux Installation

Choose your platform and install Docker on your server: https://docs.docker.com/engine/install/ 

### Windows/localhost Installation (testing and experimental purposes)

1. Download Docker Desktop from [https://www.docker.com/products/docker-desktop/](https://www.docker.com/products/docker-desktop/).
2. Install Docker Desktop. It is not necessary to change anything in the installation. A system restart is required after installation.

### Verify Docker is Running
Check if Docker is in a running state by executing the command:

 ```console
    docker ps
 ```

### Clone the Zabbix Docker Repository

Download this archive, you can use download link above, or clone the repo:

 ```console
    git clone git@github.com/luaveco/zabbix-docker](https://github.com/luaveco/zabbix-docker.git
 ```

### Build and Launch Zabbix Containers

Download all necessary files by executing the command:

 ```console
	docker-compose up -d
 ```

 Wait for the containers to be downloaded, built and launched, it will take a while.

### Verify Services are Running

Confirm that all the services are running.
 ```console
	docker-compose ps 
 ```

### Access Zabbix in a Web Browser
1. Open a web browser and go to http://localhost or http://127.0.0.1 
2. Log in using the default username Admin and password zabbix.

When running the compose for the first time, it may take a minute or two before the database is initialized. If you get a database error, please try again in the next minute or two before the login screen appears. 
