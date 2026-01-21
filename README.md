## 👋 Welcome to blinko 🚀

Blinko - Minimalist note-taking and bookmarking

## 📋 Description

Blinko is a fast, minimalist note-taking and bookmarking application with a clean interface for capturing thoughts, links, and ideas quickly.

## 🚀 Services

- **app**: Blinko application (`blinkospace/blinko:latest`)

## 📦 Installation

### Using curl
```shell
curl -q -LSsf "https://raw.githubusercontent.com/composemgr/blinko/main/docker-compose.yaml" | docker compose -f - up -d
```

### Using git
```shell
git clone "https://github.com/composemgr/blinko" ~/.local/srv/docker/blinko
cd ~/.local/srv/docker/blinko
docker compose up -d
```

### Using composemgr
```shell
composemgr install blinko
```

## 🔧 Configuration

### Environment Variables

```shell
TZ=America/New_York
BASE_HOST_NAME=${HOSTNAME}
```

## 🌐 Access

- **Web Interface**: http://172.17.0.1:60046

## 📂 Volumes

- `./rootfs/data/blinko` - Notes and bookmarks database

## 🔍 Logging

```shell
docker compose logs -f app
```

## 🛠️ Management

```shell
docker compose up -d
docker compose down
docker compose pull && docker compose up -d
```

## 📋 Requirements

- Docker Engine 20.10+
- Docker Compose V2+

## 🤝 Author

🤖 casjay: [Github](https://github.com/casjay) 🤖  
🦄 composemgr: [Github](https://github.com/composemgr) 🦄
