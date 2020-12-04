# Projet 03 (vagrant + ansible + docker + nginx)

## Installation de vagrant:

1. Télécharger la bonne version du vagrant depuis le site : (https://www.vagrantup.com/downloads)


2. Installer la VM avec vagrant en configurant Vagrantfile voir les boxes dans (https://app.vagrantup.com/boxes/search)

3. Lancer Vagrant et accéder
```bash
 > vagrant up
 > vagrant ssh
```
4. Pour arrêter vagrant (optionnel)
```bash
 > vagrant halt
```

5. Pour supprimer la VM d'abord chercher l'instance et ensuite utiliser l'option destroy
```bash
> vagrant global-status --prune
> vagrant destroy xxxxx
```


## Installation Ansible

1. Entrer dans la VM
```bash
> vagrant ssh

sudo apt update
sudo apt install software-properties-common
sudo apt-add-repository --yes --update ppa:ansible/ansible
sudo apt install ansible
```


## Installation de Docker
```bash
>vagrant ssh
sudo apt update
sudo apt install apt-transport-https ca-certificates curl software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu focal stable"
sudo apt update
apt-cache policy docker-ce
sudo apt install docker-ce --fix-missing
sudo systemctl status docker

sudo docker help

```


