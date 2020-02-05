# LaDoc

The goal of this repository is to create a lightweight development environment for Laravel applications. 
Alternatives like LaraDock are often much larger without giving me the desired advantage. Furthermore I wanted to get to know Docker better and this was a good opportunity.

The setup consists of three containers: 
- app: Based on PHP-FPM. It is used to install all Composer and NPM dependencies and to execute artisan commands
- webserver: Based on nginx
- db: Based on mySQL 

## Installation
To use it, the repository can be added as git submodules. Then run `docker-compose up -d`, on initial execution it will take longer, on subsequent executions it will be drastically reduced.

## Production
Note that this is a development environment and not a production environment. I would like to implement this in the future, but I need even better knowledge of dockers and production environments.