# Démo stack LAMP avec ANsible

Ce projet à pour but d'offrir une démonstration d'utilisation d'un playbook avec Ansible pour construire une stack LAMP avec un blog.  
[Lien vers le tuto de devopssec](https://devopssec.fr/article/creation-playbook-ansible-stack-lamp#begin-article-section)


![Logo](https://www.toolin.fr/wp-content/uploads/2021/08/ansible-logo.png)

## Installation

* 192.168.10.23 web-lamp
* 192.168.10.24 db-lamp

Vous devez :
1. Ajouter les deux serveur dans `/etc/hosts` et modifier le fichier `hosts`dans le répertoire de la release
2. Générer une paire de clé ssh et copier la clé sur les deux hôtes (cf `ssh-keygen` et `ssh-copy-id`)
3. Vérifier les variables dans `var/main.yml`


## Deployment

To deploy this project run

```bash
  wget <release.tar.gz>
  tar xvzf <release.tar.gz>
  ansible-playbook release/playbook.yml
```













