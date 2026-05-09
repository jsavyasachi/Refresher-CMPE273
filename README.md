# Web Technologies Refresher

A comprehensive review of core web technologies including modern HTML5, JavaScript, and Docker deployment patterns.

## Stack

<a href="https://developer.mozilla.org/en-US/docs/Web/HTML"><img src="https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white" alt="HTML5" /></a>
<a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript"><img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=000" alt="JavaScript" /></a>
<a href="https://www.docker.com"><img src="https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white" alt="Docker" /></a>
<a href="https://www.nginx.com"><img src="https://img.shields.io/badge/Nginx-009639?style=flat&logo=nginx&logoColor=white" alt="Nginx" /></a>

## Security Patches

This project has been hardened with the following security improvements:
- **XSS Prevention**: Replaced vulnerable `innerHTML` usage with safe `textContent`.
- **Insecure Storage**: Removed plaintext password display from local storage logs.
- **Audit**: Fully patched to zero vulnerabilities.

## Running the Deployer

The `/Deployer` directory contains a task-list app ready for Nginx deployment via Docker.

```bash
cd Deployer
docker build -t task-deployer .
docker run -d -p 8080:80 task-deployer
```

Access the app at `http://localhost:8080`.
