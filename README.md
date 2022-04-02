# Docker + ReactJS tutorial: Development to Production workflow + multi-stage builds + docker compose

## Available Scripts

In the project directory, you can run:

### `docker build .`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

Access to remote machine container
### `docker exec -it react-app bash`

Remove container (force)
### `docker rm react-app -f`

Access folders in src file
### `cd /src` ### `cat App.js`

Syncing Local : Remote (Powershell)

<!-- ### `docker run -v CHOKIDAR_USEPOLLING=true ${pwd}:/app -d -p 3000:3000 --name react-app react-image`

Syncing Local : Remote (CMD)

### `docker run -v CHOKIDAR_USEPOLLING=true %cd%:/app -d -p 3000:3000 --name react-app react-image`

Syncing Local : Remote (Linux)

### `docker run -v CHOKIDAR_USEPOLLING=true $(pwd):/app -d -p 3000:3000 --name react-app react-image`
-->

Read only from remote machine (v : ro)

### `docker run -e CHOKIDAR_USEPOLLING=true -v %cd%\src:/app/src:ro -d -p 3000:3000 --name react-app react-image`


Docker compose watch Dockerfile

### `docker compose up -d --build`