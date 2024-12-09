# FROM python:3.7-slim
# RUN mkdir -p /app
# WORKDIR /app
# COPY ./requirements.txt /app/
# RUN pip install -r requirements.txt
# COPY . /app
# ENTRYPOINT ["python", "app.py"]

# # Utiliser l'image Python comme base
# FROM python:3.7-slim

# # Créer un répertoire de travail
# WORKDIR /

# # Copier d'abord les dépendances (meilleure gestion du cache Docker)
# COPY ./requirements.txt /app/

# # Installer les dépendances
# RUN pip install -r requirements.txt

# # Copier le reste des fichiers de l'application
# COPY . /

# # Assurer les permissions d'exécution sur app.py
# RUN chmod +x /app.py



# # Lancer l'application
# ENTRYPOINT ["python", "/app.py"]

FROM python:3.7-slim
RUN mkdir -p /app
WORKDIR /app
COPY ./requirements.txt /app/
RUN pip install -r requirements.txt
COPY . /app
# Exposer le port sur lequel l'application s'exécutera
EXPOSE 5000
ENTRYPOINT ["python", "app.py"]


