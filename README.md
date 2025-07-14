# devops-learning
A personal DevOps learning journey with weekly projects
---

## 📅 Week 1: Git & GitHub Basics

### ✅ Topics Covered:
- What is Git and why it's used
- Initializing a Git repository (`git init`)
- Cloning repositories from GitHub
- Tracking changes (`git add`, `git commit`)
- Pushing to GitHub (`git push`)
- Branching (`git branch`, `git checkout`, `git merge`)
- Handling merge conflicts
- Creating Pull Requests (PRs)

### 🛠️ Tools:
- Git CLI
- GitHub
- VS Code Git integration

### 📁 Mini Project:
> Create a GitHub repository named `devops-learning` and push this README file from VS Code using Git commands.



---

## 📅 Week 2: Linux & Shell Scripting

### ✅ Topics Covered:
- Basic Linux commands (navigation, files, directories)
- File permissions and ownership (`chmod`, `chown`)
- Working with processes (`ps`, `top`, `kill`)
- Package managers (apt/yum)
- Bash scripting:
  - Variables and data types
  - Conditional statements (`if`, `elif`, `else`)
  - Loops (`for`, `while`)
  - Functions in bash

### 🛠️ Tools:
- Terminal (Linux and WSL on Windows)
- Bash Shell
- VS Code with shell scripting extension

### 📁 Mini Project:
> Write a shell script that:
> - Backs up a folder (e.g., `/home/user/docs`)
> - Logs the backup process to a `.log` file
> - Runs automatically (optionally using a cron job)

Example script name: `backup.sh`

---

### 🧪 Bonus Practice:
- Create a script that deletes temp files older than 7 days.
- Set file permissions to make your script executable (`chmod +x script.sh`).
- Test the scripts in both interactive and non-interactive modes.



---

## 📅 Week 3: Networking & HTTP Basics

### ✅ Topics Covered:
- Basics of networking (IP, DNS, ports, TCP vs UDP)
- HTTP request methods (GET, POST, PUT, DELETE)
- Common status codes (200 OK, 404 Not Found, 500 Internal Server Error)
- Hostnames, domain names, and DNS resolution
- Inspecting HTTP traffic using browser dev tools
- Networking tools: `ping`, `traceroute`, `nslookup`, `curl`, `telnet`, `netstat`

### 🛠️ Tools:
- Terminal
- curl / wget
- browser dev tools (network tab)
- Postman (optional for testing HTTP APIs)

### 📁 Mini Project:
> Build a simple bash script that:
> - Accepts a list of URLs
> - Sends a request to each URL
> - Logs the HTTP response status code to a file (`status_report.log`)

Example script name: `check_status.sh`

---

### 🧪 Bonus Practice:
- Use `nslookup` or `dig` to check domain name resolution
- Use `curl -I` to fetch just headers and inspect HTTP response codes
- Test how a server reacts to different HTTP methods


---

## 📅 Week 4: DevOps Principles & CI/CD Basics

### ✅ Topics Covered:
- What is DevOps? Key goals and benefits
- DevOps lifecycle and culture (collaboration, automation, feedback loops)
- Agile & Scrum fundamentals
- CI vs CD (Continuous Integration vs Continuous Delivery/Deployment)
- Common stages of a CI/CD pipeline:
  - Code → Build → Test → Release → Deploy → Monitor
- Intro to pipeline tools: GitHub Actions, Jenkins, GitLab CI/CD

### 🛠️ Tools:
- GitHub Actions (built-in CI/CD tool for GitHub)
- YAML syntax (for defining pipelines)
- VS Code

### 📁 Mini Project:
> Create a GitHub Actions pipeline that:
> - Triggers on push to the `main` branch
> - Runs basic steps (e.g., `echo "Build successful"`)
> - Includes `jobs` and `steps` in a YAML workflow file

Example file: `.github/workflows/ci.yml`

---

### 🧪 Bonus Practice:
- Add a step to run a linter or shell script
- Set up matrix builds (e.g., test multiple Node.js versions)
- Use GitHub Actions secrets to inject environment variables





---

## 📅 Week 5: Docker Basics

### ✅ Topics Covered:
- What is Docker? Why containers are useful
- Difference between VMs and containers
- Key concepts: images, containers, layers, volumes, networks
- Docker CLI commands:
  - `docker run`, `docker ps`, `docker exec`, `docker stop`, `docker rm`
  - `docker build`, `docker images`, `docker rmi`
- Writing a basic `Dockerfile`

### 🛠️ Tools:
- Docker Desktop (Windows/macOS) or Docker Engine (Linux)
- Docker CLI
- VS Code with Docker extension (optional)

### 📁 Mini Project:
> Containerize a basic web app (Node.js, Python Flask, or static HTML) by:
> - Creating a `Dockerfile`
> - Building a Docker image locally
> - Running the app in a Docker container

Example file: `Dockerfile`

---

### 🧪 Bonus Practice:
- Explore `docker inspect` to view container details
- Try mounting a volume to persist data
- Tag and save your image locally: `docker build -t myapp:1.0 .`



---

## 📅 Week 6: Docker Compose & Registries

### ✅ Topics Covered:
- What is Docker Compose and why it's used
- Structure of a `docker-compose.yml` file
- Defining multi-container apps (e.g., web + database)
- Networking between services in Compose
- Environment variables in Compose files
- Publishing images to Docker Hub

### 🛠️ Tools:
- Docker Compose
- Docker CLI
- Docker Hub (for image hosting)
- VS Code

### 📁 Mini Project:
> Build a multi-container app using `docker-compose`:
> - One container runs a web app (Flask, Express, etc.)
> - Another runs a database (PostgreSQL, MySQL, or MongoDB)
> - Use a shared Docker network
> - Use environment variables for DB config

Example file: `docker-compose.yml`

---

### 🧪 Bonus Practice:
- Push your Docker image to Docker Hub using `docker push`
- Use `depends_on` in Compose to control startup order
- Try scaling services with `docker-compose up --scale web=2`
