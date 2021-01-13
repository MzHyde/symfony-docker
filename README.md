# Symfony 5 docker

### Summary of what is included:

- PHP
- Nginx Web server
- MySQL 
- Symfony 5 framework
- Composer
- PhpMyAdmin - manage MySQL
- Mailhog - local mailing server to test emails

### How to install this in my project?

1. Clone this repository
    ```
    git clone https://github.com/MzHyde/symfony-docker.git
    ```
2. Change directory
    ```
    cd symfony-docker
    ```
3. Up the compose
    ```
     docker-compose up -d
    ```
4. Change directory
    ```
    cd app
    ```
5. run composer
    ```
     composer install
    ```
Access your project website via - http://localhost:8080

PhpMyAdmin can be accessed via http://localhost:8181
- User: user
- Password: user

Mailhog can be accessed via http://localhost:8025

You may have to change the chosen ports in docker-compose.yml if they are already in use

