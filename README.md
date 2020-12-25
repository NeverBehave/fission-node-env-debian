# Fission: NodeJS Environment working under IPv6

This repo merely changed all base into `lts-buster` from https://github.com/fission/fission/tree/master/environments/nodejs

## Related issues

https://github.com/npm/cli/issues/348

It seems that apline musl dns resolver not working properly with node under IPv6 only network. 

## Usage

Env: https://hub.docker.com/repository/docker/neverbehave/node-env  
Builder: https://hub.docker.com/repository/docker/neverbehave/node-builder

```bash
fission env create --name nodeenv --image neverbehave/node-env:latest --builder neverbehave/node-builder:latest
```
