# solana-dapp-test

[Tuto de hashlips](https://www.youtube.com/watch?v=35RO0lAEIxE&list=PLvfQp12V0hS2FPD0yAQXF4BpGxGeUyIPw&index=1)

## [Hashlips Art Engine](https://github.com/HashLips/hashlips_art_engine)

Permet de générer les png avec leurs méta-données.

L'outils est capable de générer la structure des métadatas compatible pour le réseau ETH et SOL.

Avant de commencer, il faut renseigner le réseaux pour lequel on souhaite générer les NFTs. ça se passe dans le fichier `src/config.js`

Dans ce fichier de config il faut renseigner :

- le nom du projet NFT
- la description
- le lien IPFS (pas besoin pour un projet Solana car géré avec Metaplex)
- les metadatas pour un projet Solana
  - Acronyme du projet
  - % de comission sur les ventes du second marché (applicable sur le mint ?? A vérifier)
  - les adresses et répartition des royalties
- les dossiers des layers pour la génération des images
- etc ... (Encore à tester)

Une fois les images et leurs metadatas générées, les déplacer à la racine d'un dossier `/metaplex/assets/`

L'outils se chargera de d'envoyer les images & metadatas sur un stockage décentralisé.

## [Metaplex](https://docs.metaplex.com/)

Metaplex est une collection d'outils & smart contratcs permettant 