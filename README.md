# La dApp de Leaf avec l'interface Owner

## Description de la dapp
- Le déroulement d'un joueur
  - achète un LNFT Grain pour devenir joueur avec niveau 0
  - fait 10000 pas et devient niveau 1 et reçoit deuxième LNFT Jeune Pousse
  - fait 20000 pas et devient niveau 2 et reçoit troisième LNFT Arbre
  - fais 30000 pas et devient niveau 3 et reçoit quatrième LNFT Arbre Producteur
  - après les 30000 pas, chaque 10000 pas sera gratifié de 10 LEAFs
  - il peut récupérer ses données (dernier nombre pas, total nombres pas, l'url de ses NFTs, sa balance etc.)
  - il peut récupérer les données globales comme le supply de LNFTs et LEAFs
 
- Fonctionnalités de l'owner
  - récupérer les données des joueurs
  - mettre le dapp en pause
  - passer le dapp en mode test
  - changer le prix de LNFT
  - mettre un joueur dans la liste noire
  - voir les données globales comme supply de LNFTs et LEAFs
  - voir/récupérer les ETH qui sont présents dans la dapp

## Lien vers Site Web
https://play2plant.github.io/leaf_owner/

## Adresses déployées

- Les adresses des contracts deployées
  - LeafToken.sol : 0x3BFf79747cbb81AD5547F01957c1F9E224f1358c
  - LeafNft.sol   : 0x291F4289ff8f366103cFD5b3Ad9D98cbf5C32825
  - LeafDapp.sol  : 0xCF3b77c9db0dB46109C09d1ec268Edbbe1A596DD

- Les liens des contracts deployés. Cliquez directement sur Contract.sol pour aller vers sa page de ropsten.etherscan.io
  - [LeafToken.sol](https://ropsten.etherscan.io/token/0x3BFf79747cbb81AD5547F01957c1F9E224f1358c)
  - [LeafNft.sol](https://ropsten.etherscan.io/token/0x291F4289ff8f366103cFD5b3Ad9D98cbf5C32825)
  - [LeafDapp.sol](https://ropsten.etherscan.io/address/0xCF3b77c9db0dB46109C09d1ec268Edbbe1A596DD)

## La documentation est générée sur ipfs.io pour chaque contracts
- [LeafToken_README.md](https://ipfs.io/ipfs/QmQrJhTsEgLgkqSL3nhSLFqceXJczfZzSfTy3NMsWhQdEn)
- [LeafNft_README.md](https://ipfs.io/ipfs/QmdoCigjx7EiGb1wid6BHmaZk9iqwWq3qoR6PxwVEatH3W)
- [LeafDapp_README.md](https://ipfs.io/ipfs/QmfYCzzauCN6iYpsvHAJ74WisGv6HWVZcTqz2WRyqUFYkK)

## Installation/exécution de la dApp
- sur le dossier parent
  - `npm install`
  - `truffle migrate --reset --network NomReseau`
- sur le dossier client
  - `npm install`
  - `npm run start`
  
## Tester la dApp
REMARQUES : à cause des conflits de node_modules @openzeppelin/test-helpers a été enlevé. Donc, pouvoir tester la dapp; il faut lancer :
  `npm install @openzeppelin/test-helpers --save`
  
- `truffle test` pour lancer les testes
- `truffle run coverage` pour lancer les testes et voir le pourcentage de couverture des tests  

## Couvetrure de testes à 96.46%
- tests d'intégration complet pour owner
- tests d'intégration complet pour le joueur
- une personne externe ne peut pas faire des transactions avec la dapp (seulement peux acheter un LNFT)
<img src="https://github.com/AramArDev/leaf_dapp/blob/main/documents/tests_coverage.jpg" alt="drawing" width="600"/>  
