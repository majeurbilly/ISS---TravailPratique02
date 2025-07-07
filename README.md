<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://https://github.com/majeurbilly/ISS---TravailPratique02">
    <img src="docs/images/logo.png" alt="Logo" width="100" height="100">
  </a>
  
  <h3 align="center">Travail pratique 2 - Docker</h3>

  <h4 align="center">Billy Halle</h4>

  <h5>07/03/2025</h5>

  <p align="center">
    Installation un système de conteneurs et création de conteneurs
    <br />
    <a href="#description"><strong>Captures d'écran 🖼️»</strong></a>
      <br />
      <br />
      <a href="https://github.com/majeurbilly/ISS---TravailPratique02/issues/new?assignees=&labels=bug&template=01_BUG_REPORT.md&title=bug%3A+">Report a Bug</a>
      ·
      <a href="https://github.com/majeurbilly/ISS---TravailPratique02/issues/new?assignees=&labels=enhancement&template=02_FEATURE_REQUEST.md&title=feat%3A+">Request a Feature</a>
      ·
      <a href="https://github.com/majeurbilly/ISS---TravailPratique02/issues/new?assignees=&labels=question&template=04_SUPPORT_QUESTION.md&title=support%3A+">Ask a Question</a>
  </p>
</div>




  ## Table des matières
  <ol>
    <li>
      <a href="#description">Description</a>
      <ul>
        <li><a href="#développé-avec">Développé avec</a></li>
      </ul>
    </li>
    <li>
      <a href="#guide-dinstallation">Guide d'installation</a>
      <ul>
        <li><a href="#prérequis">Prérequis</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#auteurs--contributeurs">Auteurs & contributeurs</a></li>
    <li><a href="#Remerciment">Remerciment</a></li>
  </ol>




<!-- ABOUT THE PROJECT -->
## Description
Ce projet comporte deux sections; 

<br> La section 1, concerne la vérifier l'installation de Docker Engine et Docker Compose, puis de créer un réseau Docker privé avec des conteneurs Apache et MongoDB, en documentant toutes les étapes de vérification.

<br> La section 2, implique la personnalisation et le déploiement d'une image Docker pour Drupal, en y intégrant des éléments spécifiques et en la connectant à une base de données PostgreSQL distincte, afin de valider une installation web fonctionnelle.

<details>
 <summary>
    Captures d'écran section 1 🖼️
    
 </summary>
<br>
🛠️ Section 1 : <br>
<br>
Version de Docker Engine et Docker Compose :
<img src="docs/images/docker_version.png" alt="test">
<br>
<br>
Lister tous les réseaux Docker présents sur le système :
<img src="docs/images/mon_reseau.png" alt="test">
<br>
<br>
Liste de tous les volumes de données gérés par Docker sur le système :
<img src="docs/images/mongodb.png" alt="test">
<br>
<br>
Lister des conteneurs Docker qui sont actuellement en cours d'exécution sur votre système :
<img src="docs/images/apache_mangodb.png" alt="test">
<br>
<br>
Afficher des informations très détaillées sur le réseau Docker nommé "mon_reseau" :
<img src="docs/images/conteneurs.png" alt="test">
<br>
<br>
Afficher les journaux (logs) du conteneur Docker nommé "apache" :
<img src="docs/images/logs.png" alt="test">
<br>
<br>
http://localhost
<img src="docs/images/localhost.png" alt="test">
</details>
<details>
 <summary>
    Captures d'écran section 2 🖼️
    
 </summary>
 <img src="docs/images/logs.png" alt="test">
<br>
<br>
 </details>

### Développé avec

**Section 1 :**
- **Docker Engine version 28.2.2**
- **Docker Compose version v2.36.2**
- **Apache HTTP Server** (`httpd`)
- **MongoDB Community Server**

**Section 2 :**
- **f**



## Guide d'installation

### Prérequis

Pour travailler sur ce projet, vous devez avoir :

- **Linux**
- **Ubuntu version 24.04.2**


### Installation

#### Section 1 :

1. Ouverez votre  **terminal**.
2. Crée le réseau virtuel - `docker network create mon_reseau` 
3. Crée le volume MongoDB - `docker volume create mongodb` 
4. Lance le conteneur Apache - `docker run -d --name apache -p 80:80 --network mon_reseau httpd:latest` 
5. Lance le conteneur MongoDB - `docker run -d --name mongodb --network mon_reseau \
-v mongodb:/data/db \
-e MONGO_INITDB_ROOT_USERNAME=adminmongo \
-e MONGO_INITDB_ROOT_PASSWORD=EncoreUneAutreBD \
mongodb/mongodb-community-server` 
6. Vérifie que vos conteneurs sont en cours d'exécution - `docker ps` 

#### Section 2 :

1. Install `...` 
4. Install `...` 
4. Install `...` 
4. Install `...` 
4. Install `...` 
4. Install `...` 
4. Install `...` 
4. Install `...` 
4. Install `...` 

## Auteurs & contributeurs

Billy Hallé

## Remerciment

Remerciment:

* [EXEMPLE](https://EXEMPLE.io/)
* [EXEMPLE](https://EXEMPLE.com/)

<p align="right">(<a href="#readme-top">back to top</a>)</p>


