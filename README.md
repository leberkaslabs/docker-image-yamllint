# YAML Lint

[![Container Release (yamllint)](https://github.com/leberkaslabs/docker-image-yamllint/actions/workflows/build-push-action.yml/badge.svg)](https://github.com/leberkaslabs/docker-image-yamllint/actions/workflows/build-push-action.yml)

This repository is designed to build Docker images for [yamllint](https://yamllint.readthedocs.io/en/stable/).

```bash
docker pull dudecalledbro/yamllint:latest
```

## Usage

You can easily run `yamllint` using Docker, which provides cross-platform solution for linting your YAML files. Simply pipe your YAML file into the Docker container with the following command:

```bash
docker run --rm -i dudecalledbro/yamllint:latest < $YAML_FILE
```

This will run `yamllint` on your YAML fle without needing to install anything locally.

## Build

This image build is scheduled with GitHub Actions and will be pushed to DockerHub. The image will also be rebuilt, if the `main` branch is updated. If you need to build the image locally, ensure [Docker](https://docs.docker.com/engine/installation/) is installed and execute the following:

```bash
docker build -t yamllint:latest .
```

## License

Copyright © 2025 Niclas Spreng

Licensed under the [MIT license](LICENSE).
