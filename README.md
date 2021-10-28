# DBP API Server Template

[GitLab](https://gitlab.tugraz.at/dbp/relay/dbp-relay-server-template)

This repository can be used as a template/starting point for your own API instance.
It consists of a minimally configures Symfony application and development environment
and includes/integrates:

* The [dbp/api-core-bundle](https://gitlab.tugraz.at/dbp/dbp-api/api-core-bundle): Which provides authentication, some same base end points and entities and configuration for [api-platform](https://api-platform.com/)
* A docker-compose based development environment
* Linter/Unittest integration

## Documentation

The documentation is work in progress and currently exists in another repository which can be viewed here:
[Relay API Gateway](https://dbp-demo.tugraz.at/dev-guide/relay/)

It will be moved into this repository in the near future.

## Creating your own API instance and creating your own Bundle

* Fork this repository
* Run the docker-compose based development environment and test it
* Copy the "api-starter-bundle" repo and rename everything
* Add the new bundle to your API fork

## Development

```bash
# clone git repository
git clone https://gitlab.tugraz.at/dbp/relay/dbp-relay-server-template.git relay-api
cd relay-api

# install dependencies (you need php and composer for this)
# you can also do this in the dev docker container (see below docker-dev link)
composer install
```

Please open [docker-dev/README.md](./docker-dev/README.md) for more information.
