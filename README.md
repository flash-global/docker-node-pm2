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

Finally add your pm2 config file in your project with name `ecosystem.config.js` ([documentation](http://pm2.keymetrics.io/docs/usage/application-declaration/)). It need to be in the root directory.

If you want another name/location for your config file, orverride the ENTRYPOINT like this :
```
entrypoint:
    - pm2-docker
    - path/to/config/file.js
```
