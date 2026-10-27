# Boutique (voitures cyberpunk)

Site de vente de véhicules : catalogue, fiche véhicule avec variantes de couleur, panier et connexion. Front en HTML/JS, API en Node.js (Express) avec une base MySQL.

Projet de groupe réalisé en formation.

## Lancer le projet

Il faut Node.js et MySQL.

1. Créer la base (par défaut `voiture_cyberpunk`) et importer `backend/api/database/migration_boutique_cyberpunk.sql`, puis `backend/api/database/phpmyadmin_import_fixed.sql` pour les données.
2. Si besoin, définir les variables `DB_HOST`, `DB_USER`, `DB_PASSWORD`, `DB_NAME`, `DB_PORT`.
3. Démarrer l'API :

```bash
cd backend
npm install
npm start
```

L'API écoute sur `http://localhost:8080` (ex. `/api/voitures`). Ouvrir ensuite `index.html` dans le navigateur.

## Structure

- `backend/` : serveur Express, routes, contrôleurs, modèles et scripts SQL
- `js/` : code du front (catalogue, fiche véhicule, panier, connexion)
- `static/` : images et styles. Les images ont été réduites à 1000 px de large pour alléger le dépôt.

Les comptes de connexion présents dans le code (`admin`, `V_2077`) sont des comptes de démonstration.
