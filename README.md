# docker-youtube-dl

This is a Docker image for [youtube-dl](https://github.com/rg3/youtube-dl) available at [Dockerhub](https://hub.docker.com/r/kkawa/youtube-dl/)

## How to use this.

### Download the file.

```bash
docker run --rm -v $(pwd):/data kkawa/youtube-dl URL 
```

### List available formats of the file.

```bash
docker run --rm -v $(pwd):/data kkawa/youtube-dl --list-formats URL
```

### Download the file in the specified format.

```bash
docker run --rm -v $(pwd):/data kkawa/youtube-dl --format FORMAT_NUMBER URL
```

## Tips

### Alias

```bash
alias youtube-dl='docker run --rm -u $(id -u):$(id -g) -v $(pwd):/data kkawa/youtube-dl'
```
