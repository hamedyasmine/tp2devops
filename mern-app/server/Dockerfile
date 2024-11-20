# Utiliser l'image de base node:lts-alpine
FROM node:lts-alpine

# Définir le répertoire de travail dans le conteneur
WORKDIR /usr/src/app

# Copier les fichiers package*.json dans le conteneur
COPY package*.json ./

# Installer les dépendances via npm
RUN npm install

# Copier tous les fichiers restants du serveur dans le conteneur
COPY . .

# Exposer le port 9000 (port sur lequel l'application Express tourne)
EXPOSE 9000

# Démarrer l'application avec npm start
CMD ["npm", "start"]
