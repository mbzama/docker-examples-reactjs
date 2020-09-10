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
Run `docker run -p 9999:80 --name angular-app-container docker-examples-reactjs`


## Create/Run docker container
Navigate to `http://localhost:9999/`