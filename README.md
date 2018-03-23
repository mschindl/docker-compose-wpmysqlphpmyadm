# wpmysqlphpmyadm
# Quick and dirty docker compose example for Wordpress + MySQL + phpmyadmin

1. Create
docker-compose.yml

2. Run
docker-compose up -d

Something wrong then clean up...

1. docker stop phpmyadmin database wordpress; docker-compose rm -v
2. docker volume rm wordpress_wordpress-db-data wordpress_wordpress-data-uploads

Troubleshoting

1. docker logs wordpress
