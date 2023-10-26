Application Node.js Express avec MySQL
Cette application Node.js Express est un exemple d'API RESTful qui interagit avec une base de données MySQL pour effectuer des opérations CRUD (Create, Read, Update, Delete) sur les données.

Configuration de la base de données MySQL
Assurez-vous d'avoir une base de données MySQL installée et opérationnelle. Vous devrez également créer une base de données nommée "RESTAURANT" pour que cette application fonctionne. Vous pouvez ajuster les détails de la connexion MySQL dans le fichier index.js.

javascript
Copy code
const connection = mysql.createConnection({
    host: 'localhost',
    user: 'root',
    password: 'VotreMotDePasse',
    database: 'RESTAURANT'
});
Installation
Clonez ce référentiel :
bash
Copy code
git clone https://github.com/votre-utilisateur/express-mysql-app.git
cd express-mysql-app
Installez les dépendances nécessaires :
Copy code
npm install
Démarrez l'application :
Copy code
node index.js
L'application sera accessible à l'adresse : http://localhost:500.

Endpoints de l'API
L'application expose plusieurs endpoints pour interagir avec la base de données :

GET /items: Récupérer la liste des articles.
GET /formula: Récupérer la liste des formules.
GET /category/starters: Récupérer les entrées (starters) de la catégorie.
GET /category/mains: Récupérer les plats principaux (mains) de la catégorie.
GET /category/sides: Récupérer les accompagnements (sides) de la catégorie.
GET /category/drinks: Récupérer les boissons (drinks) de la catégorie.
GET /category/desserts: Récupérer les desserts de la catégorie.
GET /itemcat: Récupérer des articles en fonction de paramètres spécifiques.
GET /items/:item_id: Récupérer un article par son ID.
GET /category/:category_id: Récupérer une catégorie par son ID.
GET /formula/:formula_id: Récupérer une formule par son ID.
DELETE /delitems/:item_id: Supprimer un article par son ID.
DELETE /delformula/:formula_id: Supprimer une formule par son ID.
POST /category: Insérer une nouvelle catégorie. Assurez-vous de fournir le nom de la catégorie dans le corps de la requête.
POST /formula: Insérer une nouvelle formule. Assurez-vous de fournir le nom de la formule dans le corps de la requête.
POST /item: Insérer un nouvel article. Assurez-vous de fournir le nom de l'article dans le corps de la requête.
Pour effectuer des opérations POST, vous pouvez utiliser un outil comme Postman ou curl.

Contribuer
N'hésitez pas à contribuer en ouvrant des problèmes ou en soumettant des demandes d'extraction. Cette application peut servir de point de départ pour des projets plus avancés.

Licence
Ce projet est sous licence MIT. Veuillez consulter le fichier LICENSE pour plus d'informations.

N'hésitez pas à personnaliser ce README en fonction de votre projet, à ajouter plus de détails, des captures d'écran, des informations sur les dépendances, etc. Cela aidera les autres développeurs à comprendre et à utiliser votre application.
