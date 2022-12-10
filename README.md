# Platform - OpenProject

This setup allows you to run community edition of [OpenProject](https://www.openproject.org/)

## Production Setup

OpenProject production setup:

- Create a public network - `docker network create project_public_network`
- Issue SSL certificate - `docker-compose run --rm certbot certonly --webroot --webroot-path /var/www/certbot/ -d openproject.platform.
  jalantechnologies.com -m developer@jalantechnologies.com --agree-tos`
- Run services - `docker-compose up`
