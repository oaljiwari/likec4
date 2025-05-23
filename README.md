# Architecture As Code (en LikeC4)

Ce dépôt décrit l’architecture fonctionnelle et applicative du système d’information Fnac Darty, modélisée avec [LikeC4](https://likec4.dev).

## Contexte

Le projet vise à documenter et visualiser l’ensemble des flux, applications, bases de données et composants techniques intervenant dans la gestion du référentiel produit, du référencement, de l’enrichissement et de la distribution des données produits pour Fnac, Darty et leurs partenaires.

L’arborescence du dossier `/src` reflète cette organisation :

- **/src/models/** : Modélisation des applications, systèmes, bases de données et composants pour chaque entité (Darty, Fnac, FnacDarty).
  - Chaque sous-dossier (`darty`, `fnac`, `fnacdarty`) contient des fichiers `.c4` décrivant les applications (ex : `pcm`, `mdm`, `productlive`, `metacat`, etc.), leurs interactions et les flux de données associés.
- **/src/views/** : Définition des vues statiques et dynamiques pour visualiser les flux, groupes fonctionnels et cinématiques d’alimentation du référentiel produit.
  - Les vues dynamiques illustrent les scénarios de référencement, d’intégration et de synchronisation entre les différents systèmes.

## Exemples de domaines couverts

- Référentiel produit centralisé (PCM, MDM, NewRef, ProductLive…)
- ETL et intégration de données (BizTalk ETL, DataStage, R-One…)
- Catalogues et bases de données pour les fronts web et magasins (Catalog ES, Catalog Mag Darty, FrontRef, FrontMC…)
- Applications partenaires et portails fournisseurs (TradeExpress, Gupt, MCM Mirakl…)
- Flux de codification, enrichissement, synchronisation et distribution des données produits

## Utilisation

1. Ouvrir le projet avec [github.dev](https://github.dev/likec4/example-cloud-system/blob/main/model.c4) ou [vscode.dev](https://vscode.dev/github/likec4/example-cloud-system/blob/main/model.c4)
2. Installer l’extension recommandée LikeC4 pour VSCode.
3. Ouvrir un aperçu via CodeLens ou la palette de commandes pour explorer les modèles et vues.
4. Naviguer dans les fichiers du dossier `/src` pour consulter le détail des modèles et des flux.

## Ressources

- [Documentation LikeC4](https://likec4.dev/docs/)
- [Extension VSCode LikeC4](https://marketplace.visualstudio.com/items?itemName=likec4.likec4-vscode)