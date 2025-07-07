<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/majeurbilly/ISS---TravailPratique02">
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
 <br>
Construction d'une image Docker à partir du Dockerfile présent dans le répertoire courant :
 <img src="mon_drupal/img/1-docker_build_success.png" alt="test">
<br>
<br>
 Liste toutes les images Docker stockées localement sur la machine :
 <img src="mon_drupal/img/2-docker_images_list.png" alt="test">
 <br>
<br>
Lister tous les conteneurs Docker actuellement en cours d'exécution sur le système :
<img src="mon_drupal/img/3-Docker-PS-Postgres-Container-Running.png.png" alt="test">
 <br>
<br>
Créer et de démarrer un nouveau conteneur Docker en lui attribuant le nom drupal-postgres : 
<img src="mon_drupal/img/4-Docker-Run-PostgreSQL-Image-Pull.png.png" alt="test">
 <br>
<br>
Crée un nouveau volume Docker persistant nommé drupal-data <img src="mon_drupal/img/5-Drupal-Docker-Volume-Creation.png.png" alt="test">
 <br>
<br>
Lister tous les conteneurs Docker actuellement en cours d'exécution sur le système : 
<img src="mon_drupal/img/6-Docker-Images-List-and-Drupal-Run.png" alt="test">
 <br>
<br>
Lister tous les conteneurs Docker actuellement en cours d'exécution sur le système :
<img src="mon_drupal/img/7-Docker-PS-Drupal-Postgres-En-Cours.png" alt="test">
 <br>
 L'image présente la première étape de l'installation de Drupal 9.5.11 :
 <img src="mon_drupal/img/8-Drupal-Installation-Etape1.png" alt="test">
 <br>
L'image présente la deuxième étape de l'installation de Drupal 9.5.11 :  <img src="img/9-Drupal-Installation-Etape2.png.png" alt="test">
 <br>
L'image illustre la page de configuration de la base de données de l'installation de Drupal 9.5.11  <img src="mon_drupal/img/10-Drupal-Installation-Etape3.png" alt="test">
 <br>
L'image montre la page d'accueil de l'interface d'administration de Drupal : <img src="mon_drupal/img/12-Drupal-Installation-Etape4.png" alt="test">
 <br>
L'image présente la page d'administration de Drupal permettant d'ajouter un nouveau thème : <img src="mon_drupal/img/13-Drupal-Installation-Etape5.png" alt="test">
 <br>
L'image montre la page du gestionnaire de mises à jour de Drupal, confirmant l'ajout réussi des fichiers et du thème Bootstrap : <img src="mon_drupal/img/14-Drupal-Installation-Etape6.png" alt="test">
 </details>

### Développé avec

**Section 1 :**
- **Docker Engine version 28.2.2**
- **Docker Compose version v2.36.2**
- **Apache HTTP Server** (`httpd`)
- **MongoDB Community Server**

**Section 2 :**
- **Docker Engine version 28.2.2**
- **Drupal 9 (image drupal:9)**
- **PostgreSQL (image postgres:latest)**
- **Git (installé dans l'image Drupal)**
- **Thème Bootstrap (cloné via Git)**




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

1. Docker Engine installé et en cours d'exécution. 
2. Naviguez vers le répertoire mon_drupal/drupal où se trouve le Dockerfile
3. Construisez votre image Drupal personnalisée - `docker build -t my-drupal:9 .` 
4. Créez le volume pour PostgreSQL `docker volume create drupal-data` 
5. Lancez le conteneur PostgreSQL `docker run -d --name drupal_db --network mon_reseau \
  -e POSTGRES_DB=drupal_db \
  -e POSTGRES_USER=drupal_user \
  -e POSTGRES_PASSWORD=drupal_password \
  -v drupal-data:/var/lib/postgresql/data \
  postgres:latest` 
6. Lancez le conteneur Drupal en exposant le port 8080 - `docker run -d --name my-drupal --network mon_reseau -p 8080:80 my-drupal:9` 
7. Accédez à l'installation de Drupal dans votre navigateur - `http://localhost:8080` 
8. configuration de Drupal 


## Auteurs & contributeurs

Billy Hallé

<p align="right">(<a href="https://github.com/majeurbilly/ISS---TravailPratique02">back to top</a>)</p>


