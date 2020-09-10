# Running app without Docker

## Install Deps
Run `npm install`


## Development server
Run `npm start` for a dev server. Navigate to `http://localhost:3000/`. The app will automatically reload if you change any of the source files.


## Code scaffolding
Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.


## Build
Run `npm run build` to build the project. The build artifacts will be stored in the `build/` directory.


## Deploying to Web server (Nginx)
Copy files from `build/` directory to `/var/www/html`. Navigate to `http://localhost`



# Running app with Docker

## Build docker image
Instructions for building docker image are specified in `Dockerfile`. Run `docker build -t docker-examples-reactjs .`


## Create/Run docker container
Run `docker run -d -p 9999:80 --name reactjs-app-container docker-examples-reactjs`

If you encounter this error-> docker: Error response from daemon: Conflict. The container name "/reactjs-app-container" is already in use by container "d46221f9f147f1881d3a19c728d70d60a9f70f4e3b54b96c7d865604d377e311". You have to remove (or rename) that container to be able to reuse that name.

Remove the container using `docker rm -f reactjs-app-container`


## Create/Run docker container
Navigate to `http://localhost:9999/`


## To login to running container
Run `docker exec -it reactjs-app-container sh` and inspect the files using regular linux commands such ls, cat .,