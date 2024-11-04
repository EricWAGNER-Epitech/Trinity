# frontend/Dockerfile
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

# Exposez le port par défaut pour Next.js (3000)
EXPOSE 3000

# Commande pour lancer l'application en mode développement
CMD ["npm", "run", "dev"]
