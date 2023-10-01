# NGINX + React + Vite + TypeScript

This repo is my sample of React + Vite + TypeScript + Nginx + Docker + DockerCompose

## Project Hierarchy Review

nginx_vite_react 
├─ client
│   ├─ public
│   │   └─ vite.svg 
│   ├─ src
│   │   ├─ assets
│   │   │  └─ react.svg
│   │   ├─ App.css
│   │   ├─ index.css
│   │   ├─ main.tsx
│   │   └─ vite-env.ts
│   ├─ .eslintrc.cjs
│   ├─ index.html
│   ├─ package.json
│   ├─ package.lock.json
│   ├─ tsconfig.json
│   ├─ tsconfig.node.json
│   └─ vite.config.json
├─ nginx
│   └─ nginx.conf
├─ .gitignore
├─ docker-compose.yml
└─ Readme.md

## Installation (on host)

- First change work directory<br/>
<code>$ cd client</code><br/>

- Second install node_modules dependencies<br/>
<code>$ npm i</code><br/>

- Third start dev server<br/>
<code>$ npm run dev</code><br/>

## Run in Docker-compose

- First input in terminan command<br/>
<code>$ docker image build -f Dockerfile -t vite_react . </code>
<i>or sudo:</i>
<code># sudo docker image build -f Dockerfile -t vite_react . </code>

- Second input next<br/>
<code>$ docker compose -f docker-compose.yml -p <i>serve</i> up</code>

- Use it!

<i>serve</i> - is name of project started in docker-compose

<i>maded by <a href='https://github.com/letnull19A'>@letnull19a</a></i>