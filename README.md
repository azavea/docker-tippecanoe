# docker-tippecanoe

[![CircleCI](https://circleci.com/gh/azavea/docker-tippecanoe.svg?style=svg)](https://circleci.com/gh/azavea/docker-tippecanoe)

This repository contains a collection of templated `Dockerfile` for image variants designed to support the usage of [Tippecanoe](https://github.com/mapbox/tippecanoe).

## Usage

### Template Variables

- `TIPPECANOE_VERSION` - Tippecanoe version
- `VARIANT` - Base container image variant

### Testing

An example of how to use `cibuild` to build and test an image:

```bash
$ CI=1 TIPPECANOE_VERSION=1.35.0 VARIANT=slim \
  ./scripts/cibuild
```
