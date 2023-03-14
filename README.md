# n3tuk Concourse Pipelines Repository

This repository provides the base configuration for all standard pipelines to be
configured inside of the [n3tuk Concourse][n3tuk-concourse] service.

[n3tuk-concourse]: https://ci.pip3.uk

## Deployment

This pipeline is designed to be self-deployed; it will configure itself and then
build all the required pipelines configured in this repository.

## Bootstrapping

To run this configuration for the first time to configure the initial pipeline
to bootstrap this repository, run the following:

```sh
$ fly -t n3tuk login -c https://ci.pip3.uk -n main -b
logging in to team 'main'
(snip...)
$ task bootstrap
```
