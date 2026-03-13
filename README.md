[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![tests](https://github.com/stefpe/ddev-elasticmq/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/stefpe/ddev-elasticmq/actions/workflows/tests.yml?query=branch%3Amain)
[![last commit](https://img.shields.io/github/last-commit/stefpe/ddev-elasticmq)](https://github.com/stefpe/ddev-elasticmq/commits)
[![release](https://img.shields.io/github/v/release/stefpe/ddev-elasticmq)](https://github.com/stefpe/ddev-elasticmq/releases/latest)

# DDEV Elasticmq

## Overview

This add-on integrates Elasticmq into your [DDEV](https://ddev.com/) project.

## Installation

```bash
ddev add-on get stefpe/ddev-elasticmq
ddev restart
```

After installation, make sure to commit the `.ddev` directory to version control.

## Usage

| Command | Description |
| ------- | ----------- |
| `ddev describe` | View service status and used ports for Elasticmq |
| `ddev logs -s elasticmq` | Check Elasticmq logs |

## Advanced Customization

To change the Docker image:

```bash
ddev dotenv set .ddev/.env.elasticmq --elasticmq-docker-image="ddev/ddev-utilities:latest"
ddev add-on get stefpe/ddev-elasticmq
ddev restart
```

Make sure to commit the `.ddev/.env.elasticmq` file to version control.

All customization options (use with caution):

| Variable | Flag | Default |
| -------- | ---- | ------- |
| `ELASTICMQ_DOCKER_IMAGE` | `--elasticmq-docker-image` | `ddev/ddev-utilities:latest` |

## Credits

**Contributed and maintained by [@stefpe](https://github.com/stefpe)**
