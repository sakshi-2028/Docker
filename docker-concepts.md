# 🐳 Docker — Core Concepts

> A quick-reference of the most important Docker concepts, in my own words.

---

## What is Docker?

Docker is a **containerization tool** that lets you package an application along with all its dependencies into a single unit called a **container**. This guarantees the app runs the same way on any machine — development, testing, or production — without environment issues.

---

## Key Building Blocks

### 🛠️ Docker Image
A blueprint / template used to create containers.
> Just like a `class → object` in programming, image → container.

### 📦 Docker Container
A lightweight, isolated environment that has everything the app needs: **code, runtime, libraries, dependencies**.

### 📄 Dockerfile
A script containing instructions to **build a Docker image automatically**.

### ☁️ Docker Hub
Docker's official cloud-based **registry** where developers store, share, and download Docker images.

### 🧱 Multi-stage Build
Using multiple `FROM` statements in one Dockerfile to **reduce image size** and improve performance.

### 💾 Volume
Used to **persist data** even if the container is deleted.

---

## Docker Engine

Also known as **Docker Daemon**, this is the core component responsible for running and managing containers.

---

## Docker Networking

The set of mechanisms Docker provides for communication:
- Between containers
- Between containers and the outside world

---

## Docker Swarm

Docker's **native clustering & orchestration tool**. Groups several Docker hosts into a single cluster (a *swarm*) and runs containers across them as if they were one system.

---

## Docker Compose

A tool to run and manage **multiple Docker containers together** as a single application. Define all services (app, database, cache) in a `docker-compose.yml` with their configurations — start them all with one command.

---

## 🔍 Why Docker is Used

1. To avoid *"it works on my machine"* problems
2. To make applications portable across environments
3. To deploy apps faster
4. To isolate applications
5. To reduce infrastructure costs
6. To scale easily with microservices

---

## ⚔️ Docker vs Virtual Machine

| Docker | Virtual Machine |
|---|---|
| Lightweight | Heavy |
| Starts in seconds | Takes minutes |
| Shares OS kernel | Has full OS |
| Uses fewer resources | More resource usage |
| Faster deployment | Slower |

---

📌 *See [docker-commands.md](./docker-commands.md) for the command cheat-sheet.*
