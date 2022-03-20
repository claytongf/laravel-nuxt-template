<p align="center">Laravel - Nuxt Simple Template with Docker Compose</p>

<p align="center">
  This is a simple setup template to work with docker-compose, laravel and NuxtJS
</p>

## About

This template uses Laravel and Nuxt for backend and frontend with Mysql configured.
Also, the template is ready to use with docker-compose
I use Laravel 9 and NuxtJs 2. In the future, I'll change to Nuxt 3.

## Instalation

First, in docker-compose.yaml file, you need to change the name of the containers as you like.

- use this command to run the containers:<br/>
  <code>docker-compose up -d --build</code><br/>
  All the containers should be running.<br/><br/>
- To enter the bash inside the container, you need to run the following command:<br>
  <code>docker-compose exec app bash</code><br/>
- To run Laravel backend, you need to run the following (inside the bash):<br/>
  <code>cd backend</code>
  <code>composer install</code>
- To run the NuxtJs frontend, you need to run the commands (inside the bash):<br/>
  <code>cd frontend</code><br/>
  <code>npm install</code><br/>
  <code>npm run dev</code><br/>
  The localhost:3000 should be available<br/>

## Notes

This is for development purposes only. For production, it needs to create a different docker-compose and Dockerfile.
This template has phpmyadmin configured in docker-compose. If you don't need it, just remove it from docker-compose.yaml
