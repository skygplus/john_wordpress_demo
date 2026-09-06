# WordPress Docker Compose Demo

This repository is a simple demo of running WordPress and its MySQL DB using Docker Compose.

## Prerequisites

- Basic understanding of Git, GitHub, Docker, and Docker Compose
- Right versions of Git, Docker, and Docker Compose installed
- GitHub account

## Getting Started

- Clone this repository to your local machine.

## How to run

- Create a `.env` file in the project root
- Populate this file with the variables in the `.env.example` file
- Provide appropriate value to each of these variables
- Take note of the value you provided as `WORDPRESS_PORT`
- Run `docker compose up` from the project root
- Open any browser on your computer and visit `http://localhost:WORDPRESS_PORT`

## Dependencies

- Git
- Docker
- Docker Compose

## License

## Command

WORDPRESS

### 1. Go to the project root

```bash
cd /path/to/dc-wp-demo
```

### 2. Create `.env` from `.env.example`

```bash
cp .env.example .env
```

### 3. Edit the `.env` file

```bash
nano .env
```

Populate all the required variables. For example:

```env
WORDPRESS_PORT=8080
```

Save in `nano` with:

* `Ctrl + O` → Enter
* `Ctrl + X`

### 4. Start Docker Compose

```bash
docker compose up
```

Or run it in the background:

```bash
docker compose up -d
```

### 5. Check that the containers are running

```bash
docker compose ps
```

### 6. Open WordPress

If you set:

```env
WORDPRESS_PORT=8081
```

open:

```text
http://localhost:8081
```

### Complete Bash sequence

```bash
cd /path/to/dc-wp-demo
cp .env.example .env
nano .env
docker compose up -d
docker compose ps
```

Then visit:

```text
http://localhost:WORDPRESS_PORT
```

**For example:**

```text
http://localhost:8081
```

The key command from the project's instructions is:

```bash
docker compose up
```

This repository is free to use.
