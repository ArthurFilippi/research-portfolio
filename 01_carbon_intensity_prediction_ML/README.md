# Prédiction auditable de l'intensité carbone d'un portefeuille automobile multi-marchés

*Projet Scientifique Collectif (PSC), École Polytechnique, avec un partenaire bancaire européen.*

## Enjeux

Mesurer l'empreinte carbone d'un portefeuille de financement automobile suppose de prédire l'**intensité carbone** (gCO₂/km) des véhicules financés, souvent absente des bases de gestion. L'article construit une **méthodologie ML auditable** sur un jeu de données réel, multi-pays et hétérogène (sept marchés, ≈ 800 000 observations) :

- imputation des caractéristiques manquantes (*fuzzy matching*), contrôlée par divergences de Jensen-Shannon et de Wasserstein ;
- benchmark de quatre modèles (LightGBM, XGBoost, MLP) en validation croisée, **SHAP** comme outil de diagnostic ;
- intervalles de prédiction conformes (MAPIE) ;
- analyse de *dataset shift* inter-marchés (classifieur de domaine, PCA, AUC).

Détails : [`RAPPORT_PROJET_ML.pdf`](RAPPORT_PROJET_ML.pdf).

## Confidentialité

Travail soumis à des **clauses de confidentialité et de propriété intellectuelle** avec le partenaire. C'est un projet de groupe ; je ne présente **que ma contribution**, et de façon **réduite** : codes et bases de données non diffusables, considérations opérationnelles omises. L'article se limite à la méthodologie scientifique.

## Références

Pour vérification, mes tuteurs côté partenaire :

- **David Pomes** (BNP Paribas Personal Finance) : `david.pomes@bnpparibas-pf.com`
- **Christophe Bourdeaux** (BNP Paribas Personal Finance) : `christophe.bourdeaux@bnpparibas-pf.com`
