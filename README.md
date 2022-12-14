# Micro Docker environment

A [Docker](https://www.docker.com/)-based installer and runtime for the [Micro](https://micro-php.net) web framework, with full HTTP/2, HTTP/3 and HTTPS support.

## Getting Started

1. If not already done, [install Docker Compose](https://docs.docker.com/compose/install/) (v2.10+)
2. To overwrite the main configuration file (.env), simply create a new file that will depend on the APP_ENV environment variable ".env.<$APP_ENV>"
3. Run `make build` to build fresh images
4. Run `make up` (the logs will not be displayed in the current shell. Use `make logs` if you want to see the container's log after it has started.)
5. Open `https://localhost` in your favorite web browser and [accept the auto-generated TLS certificate](https://stackoverflow.com/a/15076602/1352334)
6. Run `make down` to stop the Docker containers.

## Features

* Production, development and CI ready
* Automatic HTTPS (in dev and in prod!)
* HTTP/2, HTTP/3 and support
* Built-in [Mercure](https://symfony.com/doc/current/mercure.html) hub
* Native [XDebug](docs/xdebug.md) integration

## Docs

1. [Build options](docs/build.md)
2. [Deploying in production](docs/production.md)
3. [Debugging with Xdebug](docs/xdebug.md)
4. [TLS Certificates](docs/tls.md)
5. [Troubleshooting](docs/troubleshooting.md)

## License
Micro Docker is available under the MIT License.

## Credits
Thanks to [Kévin Dunglas](https://github.com/dunglas) for the good work that this environment is based on.
