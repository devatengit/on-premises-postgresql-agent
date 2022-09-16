# on-premises-postgresql-agent

## How to Install 

To run the On-Premise PostgreSQL Agent Docker Compose File locally, you must have git, docker and docker compose installed and do the following:

Firstly Clone the Docker Compose file from Github using -

```
https://github.com/devatengit/on-premises-mysql-agent.git
``` 
## Note:

This document has been written for ``` Ubuntu ```

Windows users and the Linux users who access the terminals with ``` root ``` access they do not need to type ``` sudo ``` in front of Docker commands. ``` e.g. docker-compose pull ```

## How to Run

You will see the 'on-premises-mysql-agent' folder as soon as the clone is complete. Go to that folder, open terminal and run the following commands:

```
sudo docker-compose pull
```

This will download the docker images locally.

To run Docker Images mentioned in Docker Compose File, Write the following command:

```
sudo docker-compose up
```

This command starts all the docker containers.

Once the docker image is running, go to your browser and hit the http://localhost:8081/ URL. Your Devaten dashboard will open. After opening the dashboard add your agent, add the application and database of your application and you are ready to use the application.

If you want to stop the running containers, type

```
sudo docker-compose pause
```

command in your terminal. It will stop your application.

If you want to resume the stopped containers, type 

``` 
sudo docker-compose unpause 
```

command in your terminal. It will start your application again.

If you want to check the logs of any of the running containers use this command- 

``` 
sudo docker logs -f Container_Name 
```

To remove all the running containers of the on-premise dashboard docker image use this command- 

``` 
sudo docker-compose down 
``` 

It will stop all running containers and delete all the containers.
