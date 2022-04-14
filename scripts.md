# To build docker image from development dockerfile

```bash
docker build -f Dockerfile.dev .
```

# To attach volume and keep files in container and local in sync

## Without docker-compose.yml file

```bash
docker run -p 3000:3000 -v /app/node_modules -v $(pwd):/app <image-id>
```

## With docker-compose.yml file

Check the content of docker-compose.yml file that replicates the port mapping and volume mapping. Run the following command

```bash
docker-compose up
```
