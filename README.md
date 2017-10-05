# docker-aliases
A set of cool Docker and Docker Compose bash aliase

**Important: It only works in Linux' Bash** Pull Request are welcome to support other shells and operational systems.

## Setup
Clone this project, cd into it and run `cat aliases >> ~/.bash_aliases` in your terminal. 

After that, run `source ~/.bashrc` to update these changes in your current bash session.

## Docker Compose

### `dc_up`
will up all services in the docker-compose file as daemonized services (`docker-compose up -d`)

### `dc_up api` 

will up only api service as daemonized service (`docker-compose up -d`)

### `dc_up --build` 

up daemonized services but forcing build (`docker-compose up -d --build`)

### `dc_up api --build`

will up a daemonized service but forcing build (`docker-compose up -d`)

### `dc_logs 100`

show last 100 lines of api service, attaching to the log (`docker-compose logs -f --tail 100 api`)

### `dc_restart` 

Restart all services

`dc_restart api` Restart only api service

### `dc_kill`

Stop all services in docker-compose file and remove the containers. Good for a fresh start (`docker-compose stop && docker-compose rm -f`)
