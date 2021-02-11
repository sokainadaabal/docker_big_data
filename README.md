---
title: 'Big Data Docker Project '
disqus: hackmd
---

Big Data Docker  
===
![downloads](https://img.shields.io/github/downloads/atom/atom/total.svg)
![build](https://img.shields.io/appveyor/ci/:user/:repo.svg)
![docker](https://img.shields.io/docker/pulls/e.g._/ubuntu?logo=docker)
## Table de Matières 

 [TOC]

## Les Etapes d'instalation docker et docker composer

  pour réaliser ce Projet on doit suivre c'est étapes :

1. Updating all your software :
```gherkin= 
$ apt-get update
``` 
2. Set up the repository :
```gherkin= 
      # Install packages to allow apt to use a      repository over HTTPS.
    $ sudo apt-get install apt-transport-https    ca-certificates curl software-properties-common
      #Add Docker’s official GPG key.
    $ curl -fsSL https://download.docker.com/linux/ubuntu/gpg | apt-key add -
      #Use the following command to set up the     stable repository.
    $ add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"
```
3. Install Docker CE :
```gherkin=
    $ sudo apt-get update 
    # installe Docker 
    $ apt-get install docker-ce
    #Docker doit maintenant être installé, le démon démarré et le processus activé pour démarrer au démarrage. 
    $  sudo systemctl status docker
    #Vérifiez que Docker CE est correctement installé en exécutant l'image hello-world
    $ sudo docker run hello-world
      #resultat of this commande :
      #    Hello from Docker 
      #    This message shows that your installation appears to be working correctly.
```
4. Executing Docker without sudo :
```gherkin=
    
   
```
5. installe docker compose :
```gherkin=
    # install docker composer version 1.17
   $ sudo curl -L https://github.com/docker/compose/releases/download/1.17.0/docker-compose-`uname -s`-`uname -m` -o /usr/local/bin/docker-compose
    # donne des permessions 
   $ sudo chmod +x /usr/local/bin/docker-compose
    #test 
   $ docker-compose --version
   
```
