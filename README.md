[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/pacoogle) Thanks in advance if you want to offer me a coffee :-)


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
Currently in the "lumen" folder you will find the dist 8.X of Lumen but if you want to customize the dist or use Laravel you can manually configure the docker-compose.yml file indicating where the code of your app resides

## Debugger
If you use PhpStorm you must configure your IDE:
- open `Preferences | Languages & Frameworks | PHP | Servers`
- add new server named `localhost`
- set host to `localhost`
- set port to `8181`
- enable `use path mapping`
- configure your absolute path
- your Lumen/Laravel app root => `/var/www`
- your Lumen/Laravel app /app root => `/var/www/app`
- your Lumen/Laravel app /public root => `/var/www/public`
- open `Preferences | Languages & Frameworks | PHP` => `CLI interpreter`
- add new CLI from Docker => `docker_php:latest`
