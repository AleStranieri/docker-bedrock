## Install Bedrock 

Install Bedrock following the instructions: https://github.com/roots/bedrock

_Note: for DB_HOST variable in .env file use_ `DB_HOST=db:3306` _and for WP_HOME use the same domain from site.conf_ `server_name`

## Start 

From your project directory, start up your application by running `docker-compose up`

Stop the application, either by running `docker-compose down` from within your project directory in the second terminal, or by hitting CTRL+C in the original terminal where you started the app.

If you started Compose with `docker-compose up -d`, stop your services once you’ve finished with them:

```
$ docker-compose stop
```

You can bring everything down, removing the containers entirely, with the down command. Pass --volumes to also remove the data volume used by the Redis container:

```
$ docker-compose down --volumes
```