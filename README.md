# Docker based local dev environment

This setup is not perfect and meant for my personal use! feel free to use or modify it.

This local env is using Docker & docker-compose so docker needs to be installed locally

### Commands

```bash
#build the list of images needed (run it once)
docker-compose build
```

```bash
#Bring the container up in detach mode
docker-compose up -d
```

```bash
#Brig the container down
docker-compose up -d
```

---

`localhost:8083` point to `src/frontend/`
`localhost:8083/admin` point to `src/backend/`

---

### Installed

- **Nginx**
- **mysql 5.7.29**
- **PHP 7.2**
- **Composer** (latest) pointed to src/backend
- **Node 13.7** pointed to src/frontend
- **PHP Artisan** pointed to src/backend/artisan

---

### MySql

- **Database:** `leMysql`
- **User:** `leMysql`
- **Password:** `secret`
- **PORT :** `4306`:`3306`

---

### Useful Commands

```bash
docker-compose run --rm artisan ..
```

```bash
docker-compose run --rm composer ..
```
