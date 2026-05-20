# 🐳 Docker — Command Cheat-Sheet

> Every Docker command I've actually used, grouped by topic.

---

## 1️⃣ Basic Commands

```bash
docker --version            # Check Docker version
docker info                 # Show Docker system info
docker login                # Login to Docker Hub
docker logout               # Logout
```

---

## 2️⃣ Image Commands

```bash
docker images               # List images
docker pull <image>         # Download image
docker build -t name .      # Build image from Dockerfile
docker rmi <image_id>       # Remove image
docker tag src dest         # Tag an image before pushing
docker push <image>         # Push image to Docker Hub
```

---

## 3️⃣ Container Commands

```bash
docker ps                            # Running containers
docker ps -a                         # All containers (including stopped)
docker run <image>                   # Run a container
docker run -d <image>                # Run in background (detached)
docker run -p host:container <image> # Port mapping
docker run -v host:container <image> # Mount volume
docker run --name myapp <image>      # Give container a name
docker start <container>             # Start an existing container
docker stop <container>              # Stop a running container
docker restart <container>           # Restart container
docker rm <container>                # Remove container
docker logs <container>              # Show logs
docker exec -it <container> bash     # Enter the container shell
docker inspect <container>           # Inspect details
```

---

## 4️⃣ Volume Commands

```bash
docker volume ls               # List volumes
docker volume create myvol     # Create a volume
docker volume inspect myvol    # Inspect a volume
docker volume rm myvol         # Remove a volume
```

---

## 5️⃣ Network Commands

```bash
docker network ls              # List networks
docker network create mynet    # Create a network
docker network inspect mynet   # Inspect a network
docker network rm mynet        # Remove a network
```

---

## 6️⃣ Dockerfile Instructions (Most Used)

| Instruction | Purpose |
|---|---|
| `FROM` | Base image |
| `WORKDIR` | Set working directory inside container |
| `COPY` | Copy files from host into image |
| `RUN` | Execute commands at build time |
| `CMD` | Default command when container starts |
| `EXPOSE` | Document which port the app uses |
| `ENV` | Set environment variables |
| `ENTRYPOINT` | Configure container to run as an executable |

---

## 7️⃣ Docker Compose Commands

```bash
docker-compose up              # Start all services
docker-compose up -d           # Run in background
docker-compose down            # Stop and remove
docker-compose logs            # Show logs
docker-compose ps              # List containers
```

---

📌 *See [docker-concepts.md](./docker-concepts.md) for the concept refresher.*
