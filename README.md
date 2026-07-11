# Piiquante - API REST Sécurisée (Projet 6)

Développement du Back-End (API REST) pour une application d'avis gastronomiques sur les sauces piquantes, avec un fort accent sur la **sécurité des données** (Normes OWASP et RGPD).

## 📖 Contexte du projet

Piiquante est une marque de condiments qui souhaite développer une application web ("Hot Takes") permettant aux utilisateurs de télécharger leurs sauces piquantes préférées et de liker/disliker celles des autres. Le Front-End ayant été développé en amont via Angular, ma mission consistait à construire l'API de A à Z avec Node.js, Express et MongoDB, en implémentant des pratiques de code sécurisées.

## 🎯 Compétences validées & Sécurité

- **Architecture MVC** : Séparation logique du code en Modèles, Vues (ici remplacées par des réponses JSON) et Contrôleurs.
- **Opérations CRUD** : Création, Lecture, Mise à jour et Suppression des sauces et des utilisateurs de manière sécurisée.
- **Authentification & Autorisation** : Création de tokens JWT (JSON Web Tokens) pour sécuriser les routes de l'API.
- **Chiffrement des données** : Hachage des mots de passe utilisateurs via `bcrypt` pour protéger la base de données.
- **Gestion des fichiers** : Implémentation du middleware `multer` pour gérer l'upload des images par les utilisateurs de manière sécurisée.
- **Sécurité OWASP** : Utilisation de plugins pour contrer les attaques par force brute (Rate Limiting) et protection des headers (Helmet).

## 🛠️ Technologies utilisées

- Node.js & Express
- MongoDB (Base de données NoSQL) & Mongoose
- Bcrypt (Chiffrement)
- JSON Web Token (Authentification)
- Multer (Gestion d'images)

## 🎓 Soutenance du projet

Vous pouvez consulter le support de présentation expliquant mes choix d'architecture, la structure de mes routeurs/contrôleurs, ainsi que les mesures de sécurité mises en place :

[📄 Voir le support de présentation (PDF)](./presentation-piiquante.pdf)

## 💻 Installation locale

Pour lancer l'API localement, vous devez avoir Node.js installé sur votre machine.

Note : Ce dépôt ne contient que l'API (Back-End). L'interface utilisateur (Front-End Angular) a été fournie précompilée par OpenClassrooms. Pour tester cette API, vous pouvez utiliser des outils comme Postman, ou la relier à une interface Front-End compatible."

1. Clonez ce dépôt : `git clone https://github.com/Chaimaa-as/Piiquante-API.git`
2. Ouvrez un terminal dans le dossier et lancez la commande : `npm install`
3. Créez un fichier `.env` à la racine et ajoutez vos variables d'environnement (URL MongoDB, Clé secrète JWT). Vous pouvez vous baser sur le fichier `.env.example`.
4. Lancez le serveur avec la commande : `node server` (ou `npm start`)
5. L'API tournera par défaut sur le port 3000 (`http://localhost:3000`).
