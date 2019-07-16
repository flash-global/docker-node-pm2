# node-pm2

## Purpose
This image provide a light setup of node v12 and pm2 lastest version.

## How to use it
Add it in your docker-compose :
```
image: feiit/node-pm2:latest
```

Then configure the working_dir and the volumes:
```
volumes:
    - ./:/var/www
working_dir: /var/www
```
