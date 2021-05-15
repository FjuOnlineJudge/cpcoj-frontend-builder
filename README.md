# cpcoj-frontend-builder

## Download
* Download from Dockerhub
```
$ docker pull fjuonlinejudge/cpcoj-frontend-builder
```

* Download from Gittub Registry
```
docker pull docker.pkg.github.com/fjuonlinejudge/cpcoj-frontend-builder/cpcoj-frontend-builder:latest
```

## Using `docker-compose.yml` (Recommand)
```yml
version: "3.7"
services:
  frontend:
    # image: fjuonlinejudge/cpcoj-frontend-builder:latest
    container_name: frontend
    build:
      context: ./
      dockerfile: Dockerfile.dev   
    ports: 
      - "3000:3000"
    volumes:
      - .:/usr/src/app
```

## Running

```
$ docker-compose up -d
```
