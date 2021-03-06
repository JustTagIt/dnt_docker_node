# dnt_docker_node
Docker image for Node.js including Yarn and some other basic additions. Current version: `7.4`

## Getting the Image

```
docker pull domandtom/node:7.7
```

## Implementation

### Additional Packages

| Package Name          | CLI Executable | Notes                        |
| --------------------- | -------------- | ---------------------------- |
| `apt-transport-https` |                |                              |
| `yarn`                | `yarn`         | [Yarn](https://yarnpkg.com/) |

### Dockerfile Defaults

| Description       | Setting         |
| ----------------- | --------------- |
| `WORKDIR`         | `/data/src`     |
| `EXPOSE`          | `80`            |
| `CMD`             | `node index.js` |

### Environment Variable Defaults

| Key               | Value           |
| ----------------- | --------------- |
| `NODE_ENV`        | `production`    |
| `PORT`            | `80`            |

## Versions

| Node.js Version             | Base Image                                                                       |
| --------------------------- | -------------------------------------------------------------------------------- |
| [`7.7`](./7.7/Dockerfile)   | [`node:7.7`](https://github.com/nodejs/docker-node/blob/master/7.7/Dockerfile)   |
| [`7.6`](./7.6/Dockerfile)   | [`node:7.4`](https://github.com/nodejs/docker-node/blob/master/7.6/Dockerfile)   |
| [`7.5`](./7.5/Dockerfile)   | [`node:7.5`](https://github.com/nodejs/docker-node/blob/master/7.5/Dockerfile)   |
| [`7.4`](./7.4/Dockerfile)   | [`node:7.4`](https://github.com/nodejs/docker-node/blob/master/7.4/Dockerfile)   |
| [`6.9`](./6.9/Dockerfile)   | [`node:6.9`](https://github.com/nodejs/docker-node/blob/master/6.9/Dockerfile)   |
| [`6.10`](./6.10/Dockerfile) | [`node:6.10`](https://github.com/nodejs/docker-node/blob/master/6.10/Dockerfile) |
