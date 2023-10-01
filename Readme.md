# NGINX + React + Vite + TypeScript

This repo is my sample of React + Vite + TypeScript + Nginx + Docker + DockerCompose

## Project Hierarchy Review

nginx_vite_react<br/>
├─ client<br/>
│   ├─ public<br/>
│   │   └─ vite.svg<br/> 
│   ├─ src<br/>
│   │   ├─ assets<br/>
│   │   │  └─ react.svg<br/>
│   │   ├─ App.css<br/>
│   │   ├─ index.css<br/>
│   │   ├─ main.tsx<br/>
│   │   └─ vite-env.ts<br/>
│   ├─ .eslintrc.cjs<br/>
│   ├─ index.html<br/>
│   ├─ package.json<br/>
│   ├─ package.lock.json<br/>
│   ├─ tsconfig.json<br/>
│   ├─ tsconfig.node.json<br/>
│   └─ vite.config.json<br/>
├─ nginx<br/>
│   └─ nginx.conf<br/>
├─ .gitignore<br/>
├─ docker-compose.yml<br/>
└─ Readme.md<br/>

## Installation (on host)

- First change work directory<br/>
<code>$ cd client</code><br/>

- Second install node_modules dependencies<br/>
<code>$ npm i</code><br/>

- Third start dev server<br/>
<code>$ npm run dev</code><br/>

## Run in Docker-compose

- First input in terminan command<br/>
<code>$ docker image build -f Dockerfile -t vite_react .</code><br/>
<i>or sudo:</i>
<code># sudo docker image build -f Dockerfile -t vite_react . </code>

- Second input next<br/>
<code>$ docker compose -f docker-compose.yml -p <i>serve</i> up</code>

- Use it!

<i>serve</i> - is name of project started in docker-compose

<i>author: <a href='https://github.com/letnull19A'>@letnull19a</a></i>