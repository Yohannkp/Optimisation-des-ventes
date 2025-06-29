# Optimisation des ventes de chips via l'analyse comportementale client et A/B testing

Réaliser une analyse complète des données transactionnelles pour le compte d’un Category Manager en retail, identifier les segments clients clés, et évaluer l’impact d’un nouveau layout en magasin à l’aide de tests statistiques.
![alt text](<images/Capture d'écran 2025-06-23 193846.png>)
## Étapes réalisées

1. **Préparation et nettoyage des données**
   - Import des données transactionnelles et transformation des variables temporelles.
   - Agrégation des indicateurs mensuels par magasin (ventes, clients uniques, transactions, panier moyen).

2. **Sélection des magasins contrôle**
   - Recherche des magasins les plus similaires à chaque magasin test (corrélation sur ventes et clients avant test).
   - Attribution d'un magasin contrôle optimal pour chaque magasin test.

3. **Analyse statistique**
   - Comparaison des indicateurs clés (ventes, clients, transactions/client, panier moyen) entre magasins test et contrôle sur la période du test (février à avril 2019).
   - Utilisation de tests statistiques (t-test) pour évaluer la significativité des différences observées.

4. **Visualisations**
   - Génération de graphiques comparant l'évolution des indicateurs avant/après et test/contrôle pour chaque magasin.

5. **Synthèses et recommandations**
   - Rédaction de synthèses claires pour chaque magasin test, avec recommandations sur la généralisation du layout.
   - Documentation structurée et professionnelle dans les notebooks, avec explications pour chaque étape.

6. **Commentaires du code**
   - Ajout de commentaires détaillant les étapes principales dans chaque cellule de code pour faciliter la compréhension.

## Fichiers principaux
- `task2.ipynb` : Analyse d'impact du layout, sélection des magasins contrôle, tests statistiques, visualisations, synthèses.
- `task1.ipynb` : Analyses complémentaires sur les segments clients, visualisations, conclusions générales.

## Résultats clés
![alt text](<images/Capture d'écran 2025-06-23 193828.png>)
- Le magasin test 77 a connu une hausse significative des ventes (+X%) et de la fréquentation (+Y%) par rapport à son magasin contrôle, indiquant un effet positif du nouveau layout.
![alt text](<images/Capture d'écran 2025-06-23 193834.png>)
- Le magasin test 86 n'a pas montré de différence significative sur les ventes ou la fréquentation par rapport à son contrôle : l'impact du layout y est donc limité ou nul.
![alt text](<images/Capture d'écran 2025-06-23 193839.png>)
- Le magasin test 88 a présenté une légère amélioration, mais celle-ci n'est pas statistiquement significative.
- Les variations du panier moyen et du nombre de transactions par client confirment ces tendances : seuls les magasins avec une hausse de fréquentation voient aussi leur panier progresser.

- Les tests statistiques (t-test) valident la significativité des écarts pour le magasin 77 uniquement.


Voir le document de presentation : Impact-des-nouveaux-layouts-sur-les-ventes-de-chips.pptx

**Recommandation :**
- Généraliser le nouveau layout uniquement dans les magasins où une amélioration significative des ventes et de la fréquentation a été constatée (ex : magasin 77).
- Poursuivre l'analyse sur une période plus longue ou sur d'autres indicateurs pour confirmer ces résultats dans les autres magasins.

## Structure professionnelle
- Notebooks nettoyés, structurés, sans doublons, avec documentation claire et synthétique.
- Chaque étape est expliquée pour garantir la reproductibilité et la compréhension du raisonnement analytique.