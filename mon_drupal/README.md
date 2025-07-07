<!-- PROJECT LOGO -->
<br />
<div align="center">
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
    
  </ol>




<!-- ABOUT THE PROJECT -->
## Description
Ce répertoire contient les fichiers nécessaires pour construire une 
image Docker personnalisée de Drupal, incluant le thème Bootstrap 3. 
Il est également configuré pour interagir avec une base de données PostgreSQL.


<details>
 <summary>
    Captures d'écran section 2 🖼️
    
 </summary>
 <br>
Construction d'une image Docker à partir du Dockerfile présent dans le répertoire courant :
 <img src="img/1-docker_build_success.png" alt="test">
<br>
<br>
 Liste toutes les images Docker stockées localement sur la machine :
 <img src="img/2-docker_images_list.png" alt="test">
 <br>
<br>
Lister tous les conteneurs Docker actuellement en cours d'exécution sur le système :
<img src="img/3-Docker-PS-Postgres-Container-Running.png.png" alt="test">
 <br>
<br>
Créer et de démarrer un nouveau conteneur Docker en lui attribuant le nom drupal-postgres : 
<img src="img/4-Docker-Run-PostgreSQL-Image-Pull.png.png" alt="test">
 <br>
<br>
Crée un nouveau volume Docker persistant nommé drupal-data <img src="img/5-Drupal-Docker-Volume-Creation.png.png" alt="test">
 <br>
<br>
Lister tous les conteneurs Docker actuellement en cours d'exécution sur le système : 
<img src="img/6-Docker-Images-List-and-Drupal-Run.png" alt="test">
 <br>
<br>
Lister tous les conteneurs Docker actuellement en cours d'exécution sur le système :
<img src="img/7-Docker-PS-Drupal-Postgres-En-Cours.png" alt="test">
 <br>
 L'image présente la première étape de l'installation de Drupal 9.5.11 :
 <img src="img/8-Drupal-Installation-Etape1.png" alt="test">
 <br>
L'image présente la deuxième étape de l'installation de Drupal 9.5.11 :  <img src="img/9-Drupal-Installation-Etape2.png.png" alt="test">
 <br>
L'image illustre la page de configuration de la base de données de l'installation de Drupal 9.5.11  <img src="img/10-Drupal-Installation-Etape3.png" alt="test">
 <br>
L'image montre la page d'accueil de l'interface d'administration de Drupal : <img src="img/12-Drupal-Installation-Etape4.png" alt="test">
 <br>
L'image présente la page d'administration de Drupal permettant d'ajouter un nouveau thème : <img src="img/13-Drupal-Installation-Etape5.png" alt="test">
 <br>
L'image montre la page du gestionnaire de mises à jour de Drupal, confirmant l'ajout réussi des fichiers et du thème Bootstrap : <img src="img/14-Drupal-Installation-Etape6.png" alt="test">
 </details>

 

