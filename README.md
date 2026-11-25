# Compte Rendu TP4

# 1. Les Liens
- GitHub : https://github.com/chaimamaj065-netizen
- Profil Docker Hub : https://hub.docker.com/u/chaimamaj
- Image Client : https://hub.docker.com/r/chaimamaj/mern-client
- Image Server : https://hub.docker.com/r/chaimamaj/mern-server

# 2.Les étapes réalisées
1. Dockerfiles (Client/Dockerfile et Server/Dockerfile) :
   J'ai écrit les Dockerfiles pour conteneuriser le backend (Node/Express sur le port 9000) et le frontend (React/Vite sur le port 3000).

2. Orchestration avec docker-compose.yml :
   J'ai configuré les trois services (mongodb, server et client), le réseau entre eux, les dépendances (depends_on) et la variable MONGO_URI pour relier l'API à la base de données.

3. Build et push sur Docker Hub :
   J'ai construit les images chaimamaj/mern-server:latest et chaimamaj/mern-client:latest, puis je les ai envoyées sur Docker Hub.

4. Pipeline Jenkins (MyAppReact-Pipeline) :
   Après avoir réglé le démarrage du service Jenkins, j'ai créé et lancé le pipeline pour vérifier le dépôt, builder les images et démarrer les conteneurs.

5. Captures d'écran :
   Les captures montrant le pipeline Jenkins, les images Docker et les conteneurs actifs sont enregistrées dans le dossier Captures/.