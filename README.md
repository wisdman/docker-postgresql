## [PostgreSQL][https://www.postgresql.org/] SOCKS server as [Docker container][https://hub.docker.com/r/wisdman/postgresql/]

[![Docker Automated build](https://img.shields.io/docker/automated/wisdman/postgresql.svg)][docker]
[![Docker Build Status](https://img.shields.io/docker/build/wisdman/postgresql.svg)][docker]
[![License](https://img.shields.io/github/license/wisdman/docker-postgresql.svg)](LICENSE)

[PostgreSQL][https://www.postgresql.org/] with [WAL-G][https://github.com/wal-g/wal-g] backup, some psql console tuning and [pspg][https://github.com/okbob/pspg] pager.

This Docker image is released under a [MIT license](LICENSE).

### Usage

```console
docker pull wisdman/postgresql
docker volume create pgdata
docker run -d --net=host -p 5432:5432 -v pgdata:/var/lib/postgresql/data --name postgresql wisdman/postgresql
```

### Manage

```console
docker exec -ti psql
```

### Donation

* PayPal: https://www.paypal.me/wisdman
* YandexMoney: https://yasobe.ru/na/wisdman
* BTC: 1862ZyKQLpkrnHC5zN2Xm8UtwW7PEHnFTW
* ETH: 0x1572F3A21487eDD3b88811F87520e8cadB1ee136

### Feedbacks

Suggestions are welcome on [GitHub issue tracker](https://github.com/wisdman/docker-postgresql/issues).
