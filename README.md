<h1 align="center">
    <!--<img alt="Remote Robot" title="Remote Robot" src="https://github.com/vzhou842/example-.io-game/blob/master/public/assets/icon.svg" width="140"> <br />-->
    RR - HELPER
</h1>

## Development

To get started, make sure you have Node and NPM installed. Then,

```bash
$ npm install
$ npm run develop
```

on your local machine.

To run the project in a production setting, simply

```bash
$ npm install
$ npm run build
$ npm start
```

## Tests

To run the tests for this this project, simply

```bash
$ npm install
$ npm test
```

## Docker example
## Core module (OS, updates)
docker build --no-cache -f Dockerfile_core . -t rr-main-serv-core

## DEV
docker build --no-cache -f Dockerfile_dev . -t rr-main-serv

## PROD
docker build --no-cache -f Dockerfile_prod . -t rr-main-serv

docker run --rm -p 3000:3000 -p 8765:8765 rr-main-serv
