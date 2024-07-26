# school-site

## stack

- Jenkins CI
pipeline that clones the repo, installs dependencies(with PHP Composer), launches tests, builds Docker image and containers. automatically runs by push(with GitHub webhook)

- Docker, docker-compose
builds image and creates containers with the app, Nginx and PostgreSQL

- Ansible
playbooks to deploy on the server

- Vault
store secrets. integrates with jenkins and ansible

- Kubernetes
creates Kuber claster to deploy this app with manifests, uses Helm and Ingress Controller

## branches

- master
- dev
- feature/*
- bugfix/*
- hotfix/*
- release/*