Radar BODACC
Objectif

Outil de veille des procédures collectives (sauvegarde, redressement, liquidation judiciaire) pour repérer les locaux commerciaux susceptibles de se libérer, avant publication sur les portails immobiliers.

Fonctionnement
Recherche live par ville : le client tape le nom d'une ville, l'application interroge le BODACC en direct via l'API publique DILA/opendatasoft
Classification automatique par type de procédure et poids d'urgence (liquidation > redressement > sauvegarde)
Recherche par enseigne ou activité au sein des résultats
Export CSV des résultats filtrés
Protection par mot de passe (page de connexion + cookie de session signé)
Stack technique

React, Vite, fonctions serverless Node.js (Vercel) pour l'authentification et l'appel à l'API BODACC, middleware Edge pour la protection par mot de passe.

Limite connue

L'adresse publiée est celle du siège social, pas nécessairement celle du local commercial en vitrine ; un croisement complémentaire (Pappers, SIRENE) peut être nécessaire pour les enseignes multi-sites.

🔗 Démo
https://bodacc-radar.vercel.app/
