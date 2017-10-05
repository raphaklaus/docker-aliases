# docker-aliases
A set of cool Docker and Docker Compose bash aliase

**Important: It only works in Linux' Bash** Pull Request are welcome to support other shells and operational systems.

## Setup
Clone this project, cd into it and run `cat aliases >> ~/.bash_aliases` in your terminal.

## Docker Compose
`dc_up` = `docker-compose up -d`
`dc_up --build` = `docker-compose up -d --build`
`dc_restart` = `docker-compose restart`
`dc_kill` = `docker-compose stop && docker-compose rm /y`
`dc_logs <lines> <service name>` = `docker-compose logs -f --tail <lines> <service name>`
