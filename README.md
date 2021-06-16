
## Why
Im trying to setup an enviroment that any developer can clone, install docker and have the same enviroment as everyone else, and not need NodeJS on their local machine either.  Building Wordpress sites, which use SASS, the current developer uses NodeJS only to process SASS, minifiy code etc, ad also uses Gulp.

If someone knows how to do this, please update whatever you need, this is a demo site anyway.

I tried running : 
docker exec -it "wordpress-docker-sass_node_1" npm run install-dependencies 


## #############################################################################################




## Requeriments

- [Node](https://nodejs.org/en/download/package-manager/) 
- [Docker](https://docs.docker.com/installation/) 
- [Docker Compose](http://docs.docker.com/compose/install/)
- A local domain:  
Use the [configured DOMAIN of .env file](https://github.com/Ferrmolina/WordPress-Docker-SASS/blob/master/.env#L1), into your ```/etc/hosts``` file as ```127.0.0.1 DOMAIN```

## Installation

```bash 
git clone https://github.com/Ferrmolina/WordPress-Docker-SASS.git
cd WordPress-Docker-SASS
docker-compose up -d
npm run install-dependencies
npm run init-gulp
```

If everything worked correctly, you should see the installer for your WordPress web site!


