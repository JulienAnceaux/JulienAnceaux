Prospects Tracker
Objectif

Détecter les vendeurs motivés 6 à 12 mois avant qu'ils ne mettent leur bien en ligne, à partir de signaux publics uniquement (RGPD/CNIL compliant — aucun signal privé type divorce ou succession).

Hypothèse métier

Trois signaux publics indiquent un vendeur potentiellement motivé :

Divisions cadastrales récentes — un propriétaire qui mandate un géomètre pour diviser son terrain prépare souvent une vente
Permis de construire approuvés (signal secondaire, non encore intégré)
Mutations DVF récentes (signal secondaire, non encore intégré)
Validation empirique

Proof of concept sur Pontoise (95) : 6 078 parcelles analysées, 53 prospects qualifiés en quelques minutes (contre ~200 minutes de pige manuelle pour un volume comparable), zéro faux positif sur les données officielles.

Fonctionnement
Recherche libre par commune, sur toute la France
Source : cadastre.data.gouv.fr (IGN/DGFiP, licence ODbL)
Score +40 si la fiche cadastrale a été modifiée il y a moins de 12 mois
Export CSV
Stack technique

Node.js (fonctions serverless), API cadastre.data.gouv.fr, Vercel, authentification par mot de passe serveur.

Prochaine étape

Intégrer les signaux PermisAPI (+30) et DVF (+20) pour atteindre le scoring composite complet (0-90 points).

🔗 Démo (accès protégé par mot de passe)
