# Sup de Vinci - Containers module project

*Tested with `rust v1.82.0` et `node 23.0.0`.*

## Development

### API

#### Basics

Use `cargo run` to start the dev environment.

You can also install [cargo-watch](https://crates.io/crates/cargo-watch) to watche over your project's source for changes, and runs Cargo commands when they occur : `cargo-watch -x run`.

#### Using Docker

> TODO

### Web

#### Basics

Use `npm install` to install all dependancies, and `npm run dev` to start the dev environment.

#### Using Docker

> TODO

## Production

### API

#### Basics

Run `cargo build --release` to build and compile the app. This will create an executable in `/target/release/sdv-api`.

#### Using Docker

Run `docker compose -d --profile dev up` to build the containers to start the application, and `docker compose --profile prod dev` to stop them.
You may have to wait until the containers are fully initialized, as it can take a while for the API to build everything necessary for it to run.

### Web

#### Basics

Run `npm run build` to build the application, and run `npm run start` to start the Node.js server. 

#### Using Docker

Run `docker compose -d --profile prod up` to build the containers to start the application, and `docker compose --profile prod down` to stop them.
