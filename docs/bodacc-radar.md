Radar BODACC
Objectif

Outil de veille des procédures collectives (sauvegarde, redressement, liquidation judiciaire) pour repérer les locaux commerciaux susceptibles de se libérer, avant publication sur les portails immobiliers.

Fonctionnement
Récupération quotidienne des annonces BODACC via l'API publique DILA/opendatasoft, France entière
Classification automatique par type de procédure et poids d'urgence (liquidation > redressement > sauvegarde)
Mise en avant automatique de la zone Domus (95, 78, 60) parmi les résultats nationaux
Recherche par enseigne, activité ou ville
Export CSV des résultats filtrés
Stack technique

React, Vite, PapaParse, script Node.js de collecte (API BODACC opendatasoft), Vercel.

Limite connue

L'adresse publiée est celle du siège social, pas nécessairement celle du local commercial en vitrine ; un croisement complémentaire (Pappers, SIRENE) peut être nécessaire pour les enseignes multi-sites.

🔗 Démo
https://domus-bodacc-radar-jac-digital.vercel.app/
