# Ansible repo
![Tests](https://github.com/nigma1337/ansible/actions/workflows/main.yml/badge.svg)
![Awesome](https://img.shields.io/badge/autism-included-brightgreen)


This is a collection of personal ansible playbooks, for setting up different things

## Projects

* CTFD
    sets up a ctfd instance via `docker compose`, with SSL from certbot.
* ghidra
    sets up a ghidra server.
* lumen
    sets up a private lumina server.

## Running tests
Simply doing `vagrant up` in the root directory is enough to run said ansible playbook.

Do `vagrant up [name]` to run tests against a single service
