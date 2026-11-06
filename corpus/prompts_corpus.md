# Prompts utilisés pour constituer le corpus

- **Outil :** Claude (Anthropic), interface claude.ai
- **Date :** 2026-11-04
- **Usage :** génération de documents **synthétiques** (aucun document public réutilisé, aucun lien externe proposé par l'IA)
- **Remarque :** les prompts ci-dessous sont des résumés fidèles des demandes faites à l'assistant. Les documents ont été produits par un script Python (reportlab, Pillow, matplotlib) écrit par l'assistant ; **ils doivent être relus par l'étudiant(e)** avant dépôt.

| ID | Objet | Demande (résumé) | Documents concernés |
|---|---|---|---|
| P01 | Plan et fiche de référence | « Choisis 2 familles d'équipements faciles (pompes + compresseurs) et propose le plan du corpus : 40 documents, 2 scannés, 2 contradictoires, 1 injection, cas ambigus, groupes d'accès. » + convention d'identifiants `POMPE-A-01`, `COMP-B-02`… et codes d'alarme communs à tous les documents | tout le corpus |
| P02 | Manuels | « Crée les manuels d'utilisation des pompes A et C et des compresseurs B et D : sommaire, sécurité, caractéristiques, panneau de commande avec figure, codes d'alarme, maintenance. » | manuel_pompe_a, manuel_pompe_c, manuel_comp_b, manuel_comp_d |
| P03 | Codes d'alarme | « Crée les tableaux de codes d'alarme avec seuils, causes et actions, cohérents avec les manuels. » | codes_alarme_* (4) |
| P04 | Schémas | « Dessine les schémas hydraulique, électrique, pneumatique et de face avant. » | schema_* (6) |
| P05 | Procédures pompes | « Rédige les procédures de vidange (deux versions qui se contredisent sur le couple de serrage), de démarrage, d'arrêt d'urgence, de remplacement du joint et une note de service. » | proc_vidange_a_v1/v2, proc_demarrage_pompe_a, proc_arret_urgence_pompes, proc_joint_pompe_a, note_service_pompes |
| P06 | Procédures compresseurs | « Rédige les procédures de démarrage, purge des condensats, remplacement du filtre et arrêt d'urgence. » | proc_demarrage_comp_b, proc_purge_condensats_b, proc_filtres_comp_d, proc_arret_urgence_comp |
| P07 | Fiches de sécurité | « Rédige 4 fiches de sécurité dont deux réservées aux responsables. » | fiche_securite_* (4) |
| P08 | Historiques | « Crée des historiques d'interventions fictifs et cohérents avec les codes d'alarme (intervenants anonymisés TECH-xx), avec tickets ouverts. » | historique_* (4) |
| P09 | Photos synthétiques | « Crée des images de panneaux de commande (voyant orange allumé, photo floue) et de plaques signalétiques. » (images dessinées par code, pas de vraies photos) | photo_* (6) |
| P10 | Documents spéciaux | « Crée un document piégé contenant une instruction malveillante (test d'injection) et une note budgétaire confidentielle (test de refus d'accès). » | note_maintenance_piegee, note_budget_maintenance |
| P11 | Effet scan | « Applique un effet de numérisation (rotation, bruit, pas de couche texte) à deux procédures pour tester l'OCR. » | proc_vidange_a_v1, proc_purge_condensats_b |
