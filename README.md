# Getting started

## Installation

Clone the repository

    git clone https://github.com/mateusmlsv/email-sender-worker.git

Switch to the repo folder

    cd email-sender-worker
    
Execute docker-compose
    
    docker-compose up -d
    
----------

## Docker script

- `docker-compose up -d` - Build all the containers
- `docker-compose up -d --scale worker=3` - Build all containers with scalable worker service
- `docker-compose exec db psql -U postgres -d email_sender -c 'select * from emails'` - You can see the data in the database table
- `docker-compose down` - Stops containers and removes containers

----------

## Worker service to simulate an email sender
 
This application uses docker container to simulate an email sender. Was used `nginx`, `postgres`, `python`, `redis` container to simulate sending email. But the reason for this application was to improve my docker skills: a tool that I use every day at work.

----------
 
# Docker-compose example

this example was developed in the Docker course: Essential Tool for Developers. [Docker-compose](https://www.docker.com/) - [www.udemy.com](https://www.udemy.com/course/curso-docker/)        
