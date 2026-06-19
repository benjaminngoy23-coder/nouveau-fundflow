# FundFlow - version finale prête à déployer

Cette version est conçue pour éviter les erreurs de dépendances : elle utilise Python standard + SQLite.

## Test local Windows

1. Décompressez le ZIP.
2. Ouvrez le dossier `FundFlow_GitHub_READY`.
3. Double-cliquez sur `LANCER_FUNDFLOW.bat`.
4. Ouvrez l'adresse affichée, par exemple `http://127.0.0.1:5000`.

## Comptes de test

- Admin : `admin@fundflow.local` / `admin123`
- Agent : `agent@fundflow.local` / `agent123`
- Chauffeur : `chauffeur@fundflow.local` / `chauffeur123`
- Chef Achats : `chef@fundflow.local` / `chef123`
- Finance : `finance@fundflow.local` / `finance123`
- Logistique : `logistique@fundflow.local` / `logistique123`

## Déploiement Render

1. Envoyez ce dossier sur GitHub.
2. Créez un Web Service.
3. Build Command : `pip install -r requirements.txt`
4. Start Command : `python app.py --no-browser`
5. L'application utilise automatiquement la variable `PORT` du serveur.

## Déploiement Railway

1. Envoyez ce dossier sur GitHub.
2. Créez un nouveau projet depuis ce dépôt.
3. Railway lit `railway.json`.
4. Start Command : `python app.py --no-browser`.

## Vérification

Après déploiement, ouvrez :

`/health`

Si la page retourne `{"ok": true}`, le serveur fonctionne.

## Remarque importante

Cette version est stable pour démonstration et première mise en ligne. Elle utilise SQLite. Pour une grande entreprise avec plusieurs utilisateurs et données permanentes, il faudra ensuite brancher PostgreSQL.


## Mise à jour ajoutée

Cette version contient aussi :

- Bouton **Mot de passe oublié** sur la page de connexion.
- Table des demandes de réinitialisation visible par l’administrateur.
- Réinitialisation du mot de passe d’un utilisateur par l’administrateur dans **Utilisateurs**.
- Champ **Fonction** dans la création de compte et dans le profil.
- Fonctions proposées : Déclarant, Déclarant chargé des opérations, Secrétaire, Attaché aux finances, Chef d’agence, DRH, Directeur Général, Chauffeur, etc.

## Version mise à jour par rapport à la demande

Ajouts inclus :

- Mot de passe oublié sur la page de connexion.
- Demande de réinitialisation enregistrée dans l’application.
- Réinitialisation du mot de passe par l’administrateur dans le menu Utilisateurs.
- Champ Fonction à la création de compte, dans le profil et dans l’administration.
- Fonctions proposées : Déclarant, Déclarant chargé des opérations, Secrétaire, Attaché aux finances, Chef d’agence, DRH, Directeur Général, Chauffeur, Logisticien, Comptable, Caissier, Superviseur, etc.
