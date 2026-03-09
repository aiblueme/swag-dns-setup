# swag-guide

Interactive bento-style checklist for setting up SWAG with Cloudflare DNS wildcard SSL.

## Live

https://swag-guide.shellnode.lol

## Stack

- Static HTML/CSS/JS (vanilla, no frameworks)
- nginx:alpine container
- Ghost VPS / Docker
- SSL via SWAG + Cloudflare DNS

## Run Locally

Open `index.html` in a browser, or:

    docker build -t swag-guide .
    docker run -p 8080:80 swag-guide

## Deploy

    docker context use ghost
    docker compose up -d --build
