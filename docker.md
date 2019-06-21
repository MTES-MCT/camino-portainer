# Docker

## Environnement de développement

```bash
# démarre Portainer dans un conteneur Docker
# accessible à http://localhost:PORTAINER_PORT
docker-compose -f ./docker-compose.localhost.yml up --build
```

## Environnement de test

Pour utiliser Portainer en local dans un environnement de production

Pré-requis:

- une installation locale active de https://github.com/jwilder/nginx-proxy
- un certificat ssl auto-signé
- [instructions](https://medium.com/@francoisromain/set-a-local-web-development-environment-with-custom-urls-and-https-3fbe91d2eaf0)

```bash
# démarre Portainer dans un container Docker
# accessible à https://portainer.local
docker-compose -f ./docker-compose.local.yml up --build
```

## Environnement de production

Pré-requis:

- une installation active de https://github.com/jwilder/nginx-proxy
- [instructions](https://medium.com/@francoisromain/host-multiple-websites-with-https-inside-docker-containers-on-a-single-server-18467484ab95)

```bash
# démarre Portainer dans un container Docker
# accessible à http://portainer.camino.beta.gouv.fr
docker-compose -f ./docker-compose.yml up -d --build
```
