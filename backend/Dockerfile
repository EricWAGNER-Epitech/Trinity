# backend/Dockerfile
# Utilisez l'image de Node.js 18 comme base
FROM node:18

# Définissez le dossier de travail dans le conteneur
WORKDIR /app

# Copiez les fichiers package.json et package-lock.json dans le conteneur
COPY package*.json ./

# Installez les dépendances
RUN npm install

# Copiez tous les fichiers dans le conteneur
COPY . .

# Exposez le port du backend (4000)
EXPOSE 4000

# Commande pour lancer l'application en mode développement
# Pour Express, utilisez "node server.js"
CMD ["npm", "run", "start:dev"] # Pour Nest.js
