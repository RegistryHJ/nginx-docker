# NGINX Docker

[**DockerHub Repository Link**](https://hub.docker.com/r/registryhj/nginx)

<br />

## Supported Tags

- [`1.26`](https://hub.docker.com/repository/docker/registryhj/nginx/tags/1.26/sha256-690483adad70f3b03afd1f9e7f633e59073e8f5307f67a4326ade5ac765a0362): (`1.26.3`)
- [`1.24`](https://hub.docker.com/repository/docker/registryhj/nginx/tags/1.24/sha256-d716cce227bf56a394998ca03843af6d17e4220dba369b62de3df49b18fe6b0d): (`1.24.0`)
- [`1.22`](https://hub.docker.com/repository/docker/registryhj/nginx/tags/1.22/sha256-e289a89b06c8542fa5e5b065ba7c2ec0f29e93b698c54e13f7775467cd78e519): (`1.22.1`)
- [`1.20`](https://hub.docker.com/repository/docker/registryhj/nginx/tags/1.20/sha256-d864449fc2f152ffab9f316e23349d61cd6950d117faa5393657af0a8833b62e): (`1.20.2`)

<br />

## How to use

**Pull this image:**

```
docker pull registryhj/nginx:<tag_name>
```

**Create container in background process:**

```
docker run \
    --name <container_name> \
    -p <port>:<port> \
    registryhj/nginx:<tag_name>
```

or (if you want to set `/etc/nginx/conf.d/*`):

```
docker run \
    --name <container_name> \
    -p <port>:<port> \
    -v <path>/conf.d:/etc/nginx/conf.d \
    registryhj/nginx:<tag_name>
```

**Execute Shell Prompt:**

```
docker exec -it <container_name> zsh
```

**Execute NGINX Directly:**

(if you want to check `*.conf` file syntax)

```
docker exec -it <container_name> nginx -t
```

(if you want to reload NGINX)

```
docker exec -it <container_name> nginx -s reload
```

<br />

## Supported Architectures

- `linux/amd64`
- `linux/arm64`

# <br />

Copyright © 2025 RegistryHJ
