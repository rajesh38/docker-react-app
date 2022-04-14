# To build docker image from development dockerfile

```bash
docker build -f Dockerfile.dev .
```

# To attach volume and keep files in container and local in sync

```bash
docker run -p 3000:3000 -v /app/node_modules -v $(pwd):/app <image-id>
```