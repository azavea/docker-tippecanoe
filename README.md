# docker-tippecanoe

![](https://github.com/azavea/docker-tippecanoe/workflows/CI/badge.svg)

This repository contains a templated `Dockerfile` designed to support the usage of multiple [Tippecanoe](https://github.com/mapbox/tippecanoe) versions.

## Usage

### Template Variables

- `TIPPECANOE_VERSION` - Tippecanoe version.
- `VARIANT` - Base container image variant. Currently supports: `slim`.

### Testing

An example of how to use `cibuild` to build and test an image:

```bash
$ CI=1 TIPPECANOE_VERSION=1.35.0 VARIANT=slim \
  ./scripts/cibuild
```
