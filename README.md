### Nextcloud 21.02 in docker-compose with Redis, PostgreSQL and Traefik.


To use:
========
Make sure you have Git:
```
sudo apt-get update && sudo apt-get install git -y
```

Clone this repo:
```
git clone https://github.com/stefanfluit/nextcloud-deploy.git && cd nextcloud-deploy/src/docker
```

Copy the .env template and edit it.
```
cp .env.template .env && vim .env
```

To create the containers after:
```
docker-compose up -d
```

To destroy the server and infrastructure:
```
docker-compose down
```


# DNS:
Make sure that the URL's in the docker-compose.yml file resolve to the IP they need to!
This repo/docker-compose file uses Route53. Take a look at the DNS documentation of Traefik if you have another DNS provider, or open an issue in this repo if you want my help.