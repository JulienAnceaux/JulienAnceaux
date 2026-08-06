Parcelles Tracker
Objectif

Outil de prospection foncière amont : identifier des terrains nus détenus par des sociétés privées (SCI, SCCV en priorité) pour approcher les propriétaires potentiellement vendeurs avant la mise en concurrence des portails d'annonces.

Fonctionnement
Recherche libre par commune, sur toute la France (référentiel officiel geo.api.gouv.fr)
Source de données : MAJIC "personnes morales" (DGFiP, open data via Koumoul)
Qualification automatique du titulaire : public/parapublic, association, SCCV, SCI, professionnel immobilier, ou entreprise générique
Détection des biens déjà bâtis (garde-fou pour éviter les faux positifs)
Système de priorité (SCCV > SCI > autre)
Suivi de prospection intégré : statuts, notes, horodatage
Export CSV
Stack technique

Node.js (fonctions serverless), API Koumoul, Vercel, authentification par mot de passe serveur.

Limite connue

Une nature cadastrale ne prouve pas la constructibilité actuelle — le PLU/PLUi, les servitudes et les contraintes opérationnelles doivent être vérifiés manuellement avant toute prospection.

🔗 Démo (accès protégé par mot de passe)
https://parcelles-tracker.vercel.app/

