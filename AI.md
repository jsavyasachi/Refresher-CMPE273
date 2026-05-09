# Refresher-CMPE273 AI Instructions

## Purpose
A collection of basic web technology reviews (HTML5, JavaScript, CSS) and a simple task deployer.

## Tech Stack
- **Frontend**: HTML5, Vanilla JavaScript
- **Deployment**: Docker (Nginx)

## Security
- This project has been patched to fix DOM-based XSS vulnerabilities and insecure storage of plaintext passwords in localStorage.

## Project Layout
- `/Deployer/`: A simple task list app with Docker support.
- `*.html`: various HTML5 review exercises.
- `*.js`: JavaScript review exercises.

## Run Instructions
- Open any `.html` file in a browser.
- **Deployer**: `cd Deployer && docker build -t task-deployer . && docker run -p 8080:80 task-deployer`
