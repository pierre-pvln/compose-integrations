Docker compose yaml configuration files for various application stacks and integrations (webservers etc)

Level 0 = Single service in 1 container (using docker)<br>
Level 1 = Single service in 1 container (using docker-compose)<br>
Level 2 = Multiple services in 1 container (using docker-compose)<br>
Level 3 = Multiple containers creating 1 service (using docker-compose)<br>
Level 4 = Containers spread over network (using docker-compose)<br>

Below folder structure should be present on the host which runs docker:
```
a_folder\myDocker\on_host       shell scripts to build and run the docker configurations
        |        \services      folder with the various configurations of services (YOU SHOULD BE HERE)
        |        \integrations  folder with the docker compose yaml files 
        \myStorage              folder with volumes used to store data
```

Below folder structure should be present on the workstation on which development is done:
```
a_folder\dev_scripts command/batch files to interact with docker host
        \secrets       secrets not to be put on github
        \on_host       shell scripts to build and run the docker configurations
        \services      folder with the various configurations of services (OR YOU SHOULD BE HERE)    
        \integrations  folder with the docker compose yaml files
```
