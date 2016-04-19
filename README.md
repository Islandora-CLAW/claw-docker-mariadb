# Islandora CLAW: Mariadb Docker Image

[![Docker Stars](https://img.shields.io/docker/stars/islandora/claw-mariadb.svg)](https://hub.docker.com/r/islandora/claw-mariadb/)
[![Docker Pulls](https://img.shields.io/docker/pulls/islandora/claw-mariadb.svg)](https://hub.docker.com/r/islandora/claw-mariadb/)
[![Image Size](https://img.shields.io/imagelayers/image-size/islandora/claw-mariadb/latest.svg)](https://imagelayers.io/?images=islandora/claw-mariadb:latest)
[![Image Layers](https://img.shields.io/imagelayers/layers/islandora/claw-mariadb/latest.svg)](https://imagelayers.io/?images=islandora/claw-mariadb:latest)

### Introduction

Defines the MariaDB Docker image.

Based on the [Base Docker Image](https://github.com/Islandora-CLAW/docker-base).

### Includes

* MariaDB

### Build Arguments

No additional build arguments are provided.

**Example:**
```bash
docker build -t islandora/claw-mariadb .
```

### Environment Variables

| Variable            | Required | Default |
|---------------------|----------|---------|
| MYSQL_ROOT_USER     | no       | root    |
| MYSQL_ROOT_PASSWORD | yes      |         |

Please consult the
[parent image](https://github.com/Islandora-CLAW/docker-base).

**Example (foreground, port 3306, auto-remove):**
```bash
docker run --rm -ti -p 3306:3306 -e "MYSQL_ROOT_PASSWORD=password" islandora/claw-mariadb
```

Do note that none of the variables above will have any effect if you start
the container with a data directory that already contains a database.

### Maintainers/Sponsors

* UPEI
* discoverygarden inc.
* LYRASIS
* McMaster University
* University of Limerick
* York University
* University of Manitoba
* Simon Fraser University
* PALS
* American Philosophical Society
* common media inc.

Current maintainers:

* [Nigel Banks](https://github.com/nigelgbanks)

### Development

If you would like to contribute, please get involved with the
[Islandora Fedora 4 Interest Group](https://github.com/Islandora/Islandora-Fedora4-Interest-Group).
We love to hear from you!

If you would like to contribute code to the project, you need to be covered by
an Islandora Foundation
[Contributor License Agreement](http://islandora.ca/sites/default/files/islandora_cla.pdf)
or
[Corporate Contributor Licencse Agreement](http://islandora.ca/sites/default/files/islandora_ccla.pdf).
Please see the [Contributors](http://islandora.ca/resources/contributors) pages
on Islandora.ca for more information.

### License

[GPLv3](http://www.gnu.org/licenses/gpl-3.0.txt)
