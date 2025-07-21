[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![tests](https://github.com/siliconmeadow/ddev-azurite/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/siliconmeadow/ddev-azurite/actions/workflows/tests.yml?query=branch%3Amain)
[![last commit](https://img.shields.io/github/last-commit/siliconmeadow/ddev-azurite)](https://github.com/siliconmeadow/ddev-azurite/commits)
[![release](https://img.shields.io/github/v/release/siliconmeadow/ddev-azurite)](https://github.com/siliconmeadow/ddev-azurite/releases/latest)

# DDEV Azurite

## Overview

This add-on integrates Azurite into your [DDEV](https://ddev.com/) project.

## Installation

```bash
ddev add-on get siliconmeadow/ddev-azurite
ddev restart
```

After installation, make sure to commit the `.ddev` directory to version control.

## Usage

| Command | Description |
| ------- | ----------- |
| `ddev describe` | View service status and used ports for Azurite |
| `ddev logs -s azurite` | Check Azurite logs |

## Advanced Customization

To change the Docker image:

```bash
ddev dotenv set .ddev/.env.azurite --azurite-docker-image="busybox:stable"
ddev add-on get siliconmeadow/ddev-azurite
ddev restart
```

Make sure to commit the `.ddev/.env.azurite` file to version control.

All customization options (use with caution):

| Variable | Flag | Default |
| -------- | ---- | ------- |
| `AZURITE_DOCKER_IMAGE` | `--azurite-docker-image` | `busybox:stable` |

## Credits

**Contributed and maintained by [@siliconmeadow](https://github.com/siliconmeadow)**
