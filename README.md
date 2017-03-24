# Wordpress-docker-ansible

wordpress on nginx with docker-compose and ansible.

## Requirements

- [ansible](http://docs.ansible.com/ansible/intro_installation.html)
- [docker](https://docs.docker.com/engine/installation/)
- [docker-compose](https://docs.docker.com/compose/install/)

## Getting Started

Clone this repository.

    git clone https://github.com/shomatan/docker-ansible-wordpress.git wordpress

Build docker images using ansible.

    cd wordpress
    ansible-galaxy install -p roles/ -r requirements.yml
    ansible-playbook build-containers.yml

Run containers using docker-compose.

    cd wordpress
    docker-compose up -d
```

Now, you can access to `http://your-docker-machine-ip/`
