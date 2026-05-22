# Projet-Atelier-Web3

Ce projet est un travail en groupe de 2 étudiants sur une période de 2 semaines. Ce projet a été réalisé dans le cadre d’un travail de groupe sur les NFTs, les métadonnées et les smart contracts.

Le sujet attribué est "Infalsifishable !"

L’objectif principal est de créer une collection de NFTs dont les images et les métadonnées sont liées à des hashes immuables.
Chaque NFT est associé à :

une image générée par intelligence artificielle ;
un hash de cette image ;
un fichier JSON contenant les métadonnées du NFT ;
un hash du fichier JSON ;
un identifiant de NFT basé sur le hash du JSON.
L’idée est de rendre la collection vérifiable : si une image ou un fichier JSON est modifié, son hash change. Cela permet donc de détecter toute modification non autorisée.

2. Fonctionnement général
Le fonctionnement du projet est le suivant :

a) Image générée par IA 
b) Hash de l’image 
c) Image renommée avec son hash 
d) Image mise sur GitHub
e) Création du fichier JSON contenant le lien Github de l’image + le hash de l'image
f) Hash du fichier JSON


La preuve d'intégrité se fait ainsi:
- donne le tokenURI
- tokenURI ouvre le JSON GitHub
- on recalcule le hash du JSON
- on compare avec le tokenId du NFT
- dans le JSON, on trouve le lien de l’image
- on recalcule le hash de l’image
- on compare avec le hash écrit dans le JSON
