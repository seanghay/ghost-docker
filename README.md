# Ghost CMS - Docker Compose

Ghost v4 + MySQL 5.7

[![Validation](https://github.com/seanghay/ghost-docker/actions/workflows/validate.yml/badge.svg)](https://github.com/seanghay/ghost-docker/actions/workflows/validate.yml)

### Prerequisites

1. `ghost.env`

```env
url=http://localhost:8080
NODE_ENV=production

database__client=mysql
database__connection__host=db
database__connection__user=root
database__connection__password=password
database__connection__database=ghost
```

2. `db.env`

```env
MYSQL_ROOT_PASSWORD=password
MYSQL_DATABASE=ghost
MYSQL_USER=seanghay
MYSQL_PASSWORD=password
```

3. Start

```sh
docker-compose up -d
```


4. Stop 

```sh
docker-compose down
```

> if you want to remove the volume, use `docker-compose down -v`

---

### LICENSE

MIT

