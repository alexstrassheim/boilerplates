# Docker Build
```
❯ docker buildx build \
  --platform linux/amd64,linux/arm64 \
  --build-arg VERSION=2025.90.2 \
  -t gitea.bawow.de/alex/sysreptor\
  -t gitea.bawow.de/alex/sysreptor:2025.90.2 \
  --provenance=false \
  --push .
```

## Docker Inspect
```
❯ docker buildx imagetools inspect gitea.bawow.de/alex/sysreptor:latest
```
