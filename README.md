Wordpress local development boilerplate template

Made with this guide: https://medium.com/@richardevcom/wordpress-development-environment-with-docker-ba52427bdd65

## Managing the Docker containers:
### How to build and run backend:
1. `docker compose up -d`

### How to restart entire backend:
1. `docker compose restart`

OR
1. `docker restart $(docker ps -aq)`

### How to restart individual containers/services:
`docker compose restart <service_name>`
* Service name can be found inside `docker-compose.yml`
* Example: restart a container for service called API - `docker compose restart api`

### How to stop all running containers
`docker container stop $(docker ps -aq)`
