FROM drupal:9

# Installer git et nettoyer après l'installation
RUN apt update && \
    apt install -y git && \
    rm -rf /var/lib/apt/lists/*

# Changer de répertoire de travail et cloner le thème Bootstrap
WORKDIR /var/www/html/themes
RUN git clone --branch 5.0.x --single-branch --depth 1 https://git.drupalcode.org/project/bootstrap.git && \
    chown -R www-data:www-data bootstrap

# Revenir au répertoire racine de Drupal
WORKDIR /var/www/html
