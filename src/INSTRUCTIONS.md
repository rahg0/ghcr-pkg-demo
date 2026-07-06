# Sample app instructions

This repository includes a minimal Python HTTP app in `app.py`.

Build the Docker image from the repo root and run it:

```bash
docker build -t ghcr-pkg-demo .
docker run --rm -p 8000:8000 ghcr-pkg-demo
```

The app serves a plain-text response on port 8000. To change the port, set the `PORT` environment variable when running:

```bash
docker run --rm -p 9000:9000 -e PORT=9000 ghcr-pkg-demo
```
