# Usage

* Precondition: https://github.com/oceanBT/nextcloud-nginx-with-traefik-and-lets-encrypt-docker
* clone this repo.
* ```cp env.template .env```
* add two new subdomain like `recipes.YOURDOMAIN.com` in your DNS-Server (or deposit it at your registrar) with the server IP. Since the propagation can take up to 24 hours, an entry should be made in the hosts file at the beginning, so that the name resolution works immediately.

* edit .env (replace all REPLACE_ME values)
* ```docker-compose up ``` (the first run takes a few minutes to create the certificate.)
* open `recipes.YOURDOMAIN.com`
