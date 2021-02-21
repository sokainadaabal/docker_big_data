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
4. installe docker compose :
```gherkin=
    # install docker composer version 1.17
   $ sudo curl -L https://github.com/docker/compose/releases/download/1.17.0/docker-compose-`uname -s`-`uname -m` -o /usr/local/bin/docker-compose
    # donne des permessions 
   $ sudo chmod +x /usr/local/bin/docker-compose
    #test 
   $ docker-compose --version
   
```
5. Setting up Docker :
```gherkin=
   $ docker --version
   $ docker-compose --version
```
## Mon Project d'infrastructures de Big data :
>    ce projet de module de big data, et dans le but de préparer un doc docker-compose.yml qui va installer tous les outils d'infrastructures de big data à l'aide de docker-compose  avec un seul commande : ``` docker-compose.yml ```
>     ce project contient ces outils : ``` HDFS``` ```Hive``` ``` Spark``` ```Hue``` ```Zeppelin``` ```Kafka``` ```Zookeeper``` ```Hbase``` ```storm``` ```Mysql``` ```pig``` ```sqoop``` ``` postgres```
 
 

---
1. Clone le pojet à partir de git :arrow_heading_down: 
```gherkin=
  git clone https://github.com/sokainadaabal/docker_big_data.git
```

2. Acceder à le dossié :arrow_down_small: 
```gherkin=
  cd /Big_Data_Docker
```
3. run ce commande : 
```gherkin=
  docker-compose up -d 
```

>  à ce moment docker comopse va s'occupe tout l'installation  image docker et prépare l'infrastructure d big data .

## quelque Images de Tools : 
  a. NameNode  : http://localhost:50070
    ![](https://i.imgur.com/KyvikPe.png)
  b.DataNode :   http://localhost:50075
    ![](https://i.imgur.com/E3xiafh.png)
  c.Hbase:  http://localhost:16010
    ![](https://i.imgur.com/KCthrxN.png)
  d.Spark Master: http://localhost:8080
    ![](https://i.imgur.com/qmmZMcL.png)
  e.Spark Worker: http://localhost:8081
    ![](https://i.imgur.com/PZMtGtv.png)
  f.Zeppelin: http://localhost:19010
    ![](https://i.imgur.com/HZq4BY1.png)
  g.Storm: http://localhost:49080
  ![](https://i.imgur.com/BCdG48L.jpg)

