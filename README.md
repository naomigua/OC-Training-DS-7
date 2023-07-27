# Notebooks, présentation et note méthodologique pour le projet de détection de faillite bancaire

## Description
### Mon rôle : 
Je suis Data Scientist au sein de la société Prêt à dépenser qui propose des crédits à la consommation pour des personnes ayant peu ou pas du tout d’historique de prêt.
### Le contexte : 
L’entreprise souhaite mettre en oeuvre un outil de “scoring crédit” pour calculer la probabilité qu’un client rembourse son crédit, puis classifier la demande en accord ou refus. Elle souhaite donc développer un algorithme de classification en s’appuyant sur des sources de données variées (données comportementales, données provenant d'autres institutions financières, etc.). De plus, les chargés de relation client ont fait remonter le fait que les clients sont de plus en plus demandeurs de transparence vis-à-vis des décisions d’octroi de crédit. Cette demande de transparence des clients va tout à fait dans le sens des valeurs que l’entreprise veut incarner.
### La solution : 
Prêt à dépenser décide donc de développer un dashboard interactif pour que les chargés de relation client puissent à la fois expliquer de façon la plus transparente possible les décisions d’octroi de crédit, mais également permettre à leurs clients de disposer de leurs informations personnelles et de les explorer facilement.

### Les données à disposition : des données anonymisées sur des clients avec :
- TARGET : 1 difficultés de paiement, ou 0 absence de difficultés (ce que l’on
cherche à prédire)
- plein de données sur les clients : genre, si le client a une voiture, s’il possède de
l’immobilier, son nombre d'enfants, ses revenus, sa source de revenus, son type
d’habitation, ses études, qui l’a accompagné pour la demande d’emprunt…

### La mission :
- Construire un modèle de scoring qui donnera une prédiction sur la probabilité de
faillite d'un client de façon automatique.
- Construire un dashboard interactif à destination des gestionnaires de la relation
client permettant d'interpréter les prédictions faites par le modèle, et
d’améliorer la connaissance client des chargés de relation client.
- Mettre en production le modèle de scoring de prédiction à l’aide d’une API, ainsi
que le dashboard interactif qui appelle l’API pour les prédictions.

## Découpage des dossiers
- Notebooks/  
  - datadrift_report.html #rapport de datadrift evidently des données brutes
  - Guarneri_Naomi_1_modelisation_062023.ipynb #notebook de modélisation des données avec les premiers essais
  - Guarneri_Naomi_2_modelisation_balanced_062023.ipynb #idem avec le traitement de l'imbalanced problem
  - Guarneri_Naomi_3_modelisation_balanced_LR_seuil_cost_score_fonctions_062023.ipynb #choix du meilleur modèle, cost function, et détermination du seuil optimal
  - Guarneri_Naomi_4_note_methodologique_062023.pdf #note méthodologique pour le choix du modèle et entrainement
  - Guarneri_Naomi_5_presentation_062023.pdf #présentation du travail effectué dans le projet
  - README.md # fichier descriptif
