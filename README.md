# wpmysqlphpmyadm
# Quick and dirty docker compose example for Wordpress + MySQL + phpmyadmin

Using Compose is basically a three-step process.

1. Define your app's environment with a Dockerfile so it can be reproduced anywhere.
2. Define the services that make up your app in docker-compose.yml so they can be run together in an isolated environment.
3. Lastly, run docker-compose up and Compose will start and run your entire app.

###

1. Create
docker-compose.yml

2. Run
docker-compose up -d

Something wrong then clean up...

1. docker stop phpmyadmin database wordpress; docker-compose rm -v
2. docker volume rm wordpress_wordpress-db-data wordpress_wordpress-data-uploads

Troubleshoting

1. docker logs wordpress
