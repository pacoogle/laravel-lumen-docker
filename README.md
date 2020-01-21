# laravel-lumen-docker
Laravel, Lumen platform dockerization

## Start environment
To start docker environment, you must install [Docker](https://www.docker.com/get-started) and digit this command in your favorite terminal:
```sh
make docker-start
```
When the process finished you can open your browser and digit http://localhost:8181 to se you app works!

## Stop environment
To stop your environment you must digit this command in your favorite terminal:
```sh
make docker-stop
```

## Customization
Currently in the "lumen" folder you will find the dist 6.2 of Lumen but if you want to customize the dist or use Laravel you can manually configure the docker-compose.yml file indicating where the code of your app resides