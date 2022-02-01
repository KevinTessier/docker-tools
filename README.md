# Docker tools

## infos

J'utilise ce docker compose pour le developement de siteweb en local. Il rassemble différents outils que j'utilise pour tout les sites en developement.

Ce docker compose contient les images :

### Traefik
traefik pour la gestion des ports et des host de vos app.

Le site web -> [https://traefik.io/traefik/](https://traefik.io/traefik/)

### Mailhog

Une boite mail pour testé envoie les mails de vos app en local

github -> [https://github.com/mailhog/MailHog](https://github.com/mailhog/MailHog) 

## Installation

Installer docker et docker-compose sur votre machine

    sudo pacman -S docker docker-compose


Clone ce repo sur où vous voulez

    git clone https://monrepo.git ./

## Build et up 
build votre docker-compose

    docker-compose -f /dossier/docker-compose.yml --build

ou

Déplacer vous dans le dossier ou ce trouve le docker-compose

    cd votre-dossier/

et build votre docker-compose

    docker-compose build

Ensuite vous pouvez monter vos images avec

    docker-compose up

ou

    docker-compose up --build
