

## Database Setup

PostgreSQL instance is running directly on the host machine.
Log into PostgreSQL database and provision the dedicated database structure before booting up the container engine.

```sql
CREATE DATABASE dockerhub_database;
```

## Create Password

```shell
mkdir -p auth
htpasswd -B -c ./auth/htpasswd [your_admin_name]
```

## Start Compose

```shell
docker compose up -d
```