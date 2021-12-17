# Building Docker nginx-php Application using docker-compose

A sample website hosted with nginx and php-fpm Application with SSL using docker-compose

## Requirements

- [Install Docker](https://docs.docker.com/engine/install/)
- [Install Docker Compose](https://docs.docker.com/compose/install/)

## Prerequisite

- Setup a php application

```
git clone https://github.com/FujiClado/aws-elb-site.git  website
```

- Create SSl Certificate files (selfsigned used here)

```
openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout swathi.com.key -out swathi.com.crt
```

- Create a custom nginx conf file


## Provisioning

1. Clone the repository

  ```
  - git clone https://github.com/Swathikarun/docker-compose-nginx-php.git nginx-php

  - cd nginx-php
  ```

2. Check the syntax

  ```
  - docker-compose config
  ```

3. Creating the docker container

  ```
  - docker-compose up -d
  ```

## Result

A docker container is created in nginx and php-fpm with SSL 
