# laranjo-api


![GitHub](https://img.shields.io/github/license/romajs/laranjo-api)
[![js-standard-style](https://img.shields.io/badge/code%20style-standard-brightgreen.svg)](http://standardjs.com)
[![codecov](https://codecov.io/gh/romajs/laranjo-api/branch/master/graph/badge.svg)](https://codecov.io/gh/romajs/laranjo-api)
[![Maintainability](https://api.codeclimate.com/v1/badges/3a975d6c0360ac841545/maintainability)](https://codeclimate.com/github/romajs/laranjo-api/maintainability)
[![Test Coverage](https://api.codeclimate.com/v1/badges/3a975d6c0360ac841545/test_coverage)](https://codeclimate.com/github/romajs/laranjo-api/test_coverage)

[![CircleCI](https://img.shields.io/circleci/project/github/romajs/laranjo-api.svg)](https://circleci.com/gh/romajs/laranjo-api)
[![node](https://img.shields.io/badge/node-v10-yellow.svg)](https://nodejs.org/en/blog/release/v10.15.0/)
[![npm](https://img.shields.io/badge/npm-v6-green.svg)](https://github.com/npm/cli/releases/tag/v6.4.1)
![Requires.io](https://img.shields.io/requires/github/romajs/laranjo-api)

[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/65a494c6277d4e451080)

## Description

API for Google Hangouts Chat Bot contemplating `@Laranjo` memes.

## Development

### Requirements

* Node v6
* Docker
* Docker-compose v2

### Stack

* Express
* MongoDB
* Cloudinary (Resurce/Image Upload)

### Git hooks

This project use **husky** npm module to manage git hooks.
Please see **husky** configuration under `package.json`file.
To avoid git hooks execution you can use the `--no-verify` flag.

### Test

All tests are unitary api level, and done with **mocha** and **sinnon** npm modules.  

```sh
npm run test
```

### Coverage

Coverage is done with **istanbul** npm module.

```sh
npm run test:cover
```

### Lint

Lint is done with **eslint** and **eslint-watch** npm modules.

```sh
npm run lint
```

Can also be done in **watch** mode:


```sh
npm run lint:watch
```

### Configuration

All configuration is done with **convict** npm module.  
Everything can be specified through environment variables. 

### Build

Docker image build for development purpouse (hot reload).

```sh
npm install --dev
docker-compose build
```  

### Run

Bring all stack up and running.

```sh
docker-compose up
```  

Can also be done simply with `npm run start:dev`, but you will need to manage things on your own:
* MongoDB
* Cloudinary
* A lot of environment variables

### Access

```
http://localhost:8000
```

### Update dependencies

```sh
npm install -g npm-check-updates
ncu -u
npm i
```

## Documentation

- [Postmant collection](./docs/laranjo-api.postman_collection.json)

---

romajs - 2018
