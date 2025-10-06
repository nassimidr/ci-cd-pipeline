# Étape 1 : Image Node.js officielle
FROM node:18

# Étape 2 : Dossier de travail dans le conteneur
WORKDIR /app

# Étape 3 : Copier les fichiers nécessaires
COPY package*.json ./
RUN npm install

# Étape 4 : Copier le reste du code
COPY . .

# Étape 5 : Exposer le port 5000
EXPOSE 5000

# Étape 6 : Lancer le serveur
CMD ["node", "server.js"]
