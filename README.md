## 👋 Welcome to blinko 🚀

Minimalist note-taking and knowledge management application

## 📋 Description

Minimalist note-taking and knowledge management application

## 🚀 Services

- **app**: blinkospace/blinko:latest

### Infrastructure Components

- **db**: Postgres database


## 📦 Installation

### Option 1: Quick Install
```bash
curl -q -LSsf "https://raw.githubusercontent.com/composemgr/blinko/main/docker-compose.yaml" -o compose.yml
```

### Option 2: Git Clone
```bash
git clone "https://github.com/composemgr/blinko" ~/.local/srv/docker/blinko
cd ~/.local/srv/docker/blinko
docker compose up -d
```

### Option 3: Using composemgr
```bash
composemgr install blinko
```

## 🔧 Configuration

### Environment Variables

```shell
ENCRYPTION_KEY=changeme_nextauth_secret_min_32_chars
DB_ADMIN_PASS=CezapmhZiHlefz7V6xHbRGtd4jdmSeqV
```

See `docker-compose.yaml` for complete list of configurable options.

## 🌐 Access

- **Web Interface**: http://172.17.0.1:59095

## 📂 Volumes

- `./rootfs/data/blinko` - Data storage
- `./rootfs/data/db/postgres/blinko` - Data storage

## 🔐 Security

- Change all default passwords before deploying to production
- Use strong secrets for all authentication tokens
- Configure HTTPS using a reverse proxy (nginx, traefik, caddy)
- Regularly update Docker images for security patches
- Backup your data regularly

## 🔍 Logging

```shell
docker compose logs -f app
```

## 🛠️ Management

```bash
# Start services
docker compose up -d

# Stop services
docker compose down

# Update to latest images
docker compose pull && docker compose up -d

# View logs
docker compose logs -f

# Restart services
docker compose restart
```

## 📋 Requirements

- Docker Engine 20.10+
- Docker Compose V2+

## 🤝 Author

🤖 casjay: [Github](https://github.com/casjay) 🤖  
🦄 composemgr: [Github](https://github.com/composemgr) 🦄
