Docker compose yaml configuration files for various application stacks and integrations (webservers etc)

Below folder structure should be present on the host which runs docker:
```
myDocker\on_host       shell scripts to build and run the docker configurations
        \services      folder with the various configurations of services
        \integrations  folder with the docker compose yaml files (YOU SHOULD BE HERE)
        \storage       not used yet
```

Below folder structure should be present on the workstation on which development is done:
```
myDocker\dev_scripts   command/batch files to interact with docker host
        \secrets       secrets not to be put on github
        \on_host       shell scripts to build and run the docker configurations
        \services      folder with the various configurations of services    
        \integrations  folder with the docker compose yaml files (OR YOU SHOULD BE HERE)
        \storage       not used yet
```
