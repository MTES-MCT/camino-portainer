# Camino Portainer

> Instance Portainer de [Camino](http://camino.beta.gouv.fr/)

---

## Technologies

- [Portainer CE](https://www.portainer.io/products-services/portainer-community-edition/)
- [Docker](https://www.docker.com/)

---

## Docker

### Environnement de développement

```bash
# démarre Portainer dans un conteneur Docker
# accessible à http://localhost:PORTAINER_PORT
docker-compose -f ./docker-compose.localhost.yml up --build
```

### Environnement de test

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

### Environnement de production

Pré-requis:

- une installation active de https://github.com/jwilder/nginx-proxy
- [instructions](https://medium.com/@francoisromain/host-multiple-websites-with-https-inside-docker-containers-on-a-single-server-18467484ab95)

```bash
# démarre Portainer dans un container Docker
# accessible à http://portainer.camino.beta.gouv.fr
docker-compose -f ./docker-compose.prod.yml up -d --build
```

---

## Crédits

### Production

- [La Fabrique Numérique, Ministère de la transition écologique et solidaire](https://www.ecologique-solidaire.gouv.fr/inauguration-fabrique-numerique-lincubateur-des-ministeres-charges-lecologie-et-des-territoires)

### Équipe

- Guillaume Levieux, intrapreneur
- Joeffrey Arruyer, coach
- [François Romain](http://francoisromain.com), développeur

---

## Licence

Camino, le cadastre minier numérique ouvert

[AGPL 3 ou plus récent](https://spdx.org/licenses/AGPL-3.0-or-later.html)
