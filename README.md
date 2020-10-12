# Blockchain: Ethereum et Bitcoin expliqués

## Les caractéristiques d'une blockchain:

Une blockchain est un registre comptable distribué (Distributed Ledger Technology).

On dit que la chaine est immuable car il n'existe pas qu'un seul point d'autorité. En somme, le réseau distribué est une réponse à l'expression du "single point of authority, single point of failure".

Sur une blockchain, toutes les transactions sont inscrites au journal

Une blockchain est un ensemble de block disponible sur un réseau distribué

## Les avantages que fournit la technologie:

Il existe deux grands avantages à l'utilisation d'une blockchain: son incorruptabilité (immutability), et son l'utilisation d'un réseau distribué.

Chaque block est créée grâce au processus de hashage. Ce processus est généré par la fonction hash, qui est une fonction à sens unique. Tous les blocks sont reliés intimement entre eux grâce aux hashs.

Nous pouvons considérer que le hash est l'identité d'une donnée passé en input.

Il existe plusieurs fonctions de hashage :

- MD5 1
- Sha1sum 2

En réalité, chaque bloc est constitué d'un numéro unique, ainsi que des hashs des précédents blocs: tous les blocs de la chaine sont donc reliés entre eux. Il ne pas y avoir de bloc manquant dans une chaine puisque les numéros de blocs se suivent avec les hashs du bloc précédent.

Le bloc constitue un lieu de stockage pour les hashs et participe au maintient de l'immuabilité (lien entre blocs).

Enfin, il faut savoir qu'un bloc se divise en deux parties :

- Un bloc header qui regroupe les transactions et les hashs précédents 1

- Une liste de transactions à enregister dans le bloc (les tx) 2

![GitHub Logo](/img/blockchain.jpeg)

Pour conclure, le hash est une fonction importante qui garantit l'intégrité du registe. Présent dans chaque block, il devient donc extrèmement difficile de corrompre la chaine.

## Mécanisme de consensus:

1. Preuve de travail (PoW):

La preuve de travail est le principe originel implanté dans la première blockchain. Ce principe au départ était utilisé pour lutter contre le spam.

C'est un consensus algorithmique garantissant l'intégrité du minage. Chaque mineur se doit résoudre un puzzle plus ou moins difficile. La difficulté va varier en fonction du temps de minage. C'est-à-dire qu'en cas de minage rapide, les prochains puzzles seront plus difficiles

Le puzzle consiste à trouver un numéro de hash plus grand que celui présent dans le block header _(target)_. Pour ce faire, les mineurs vont utiliser le _nonce_ (un champs qui au début de la résolution de problème sera vide) et y inscrire tout ce qui va être utile à la résolution du problème.

Le mineur qui aura résolu le problème obtiendra une récompense pour le travail fournit.

2. Preuve d'enjeu (PoS):

La preuve d'enjeu est un concept créée par éthereum pour palier à la grande demande d'énergie demandé par le PoW.
Avec la preuve d'enjeu, le créateur du prochain bloc de la chaine est celui ayant laissé une caution de minimum 32ETH.

Au final, Ethereum change le paradigme du mécanisme de confiance, en implantant ce nouveau concept. L'intégrité de la chaîne n'est alors garantit que par ceux qui y ont des intérêts (gros montant d'ETH).

3. Le minage :

Le minage est un processus couteux. Il est exécuté par des mineurs attirés par la récompense et de hauts frais de transactions. Plus les frais de transactions proposés seront haut et plus le minage de a transactions à effecté sera fait rapidement.

4. Les frais :

La blockchain Bitcoin utilisent des frais de transation (ou gas pour Ethereum) afin de rémunérer les mineurs pour leur travail. Il y a des frais pour modifierla chaîne, effectuer un processus d'information.

Ce système a été créée pour protéger la chaine d'une surcharge du réseau.

## Le chiffrement asymétrique:

Le chiffrement asymétrique à ne pas ne pas confondre avec le cryptographie (mauvaise traduction de l'anglais), se définit par l'utilisation d'un clé privée et d'une clé publique.

La clé privée , qui doit rester secrète, est définit de manière aléatoire et est donc générée par un algorithme (l'ecdsa). Cet algorithme fonctionne comme une courbe elliptique.

La clé privée générée va passer une fonction qui va être à l'origine de la clé publique.

La clé publique peut être librement partagée sur le réseau. De cette clé va être créée une adresse utilisée lors des transactions.

Chaque transaction contient un message, et une signature générée par la clé privée de l'expéditeur.

## Les particularités d'Ethereum:

Il existe 3 grandes différences entre la blockchain d'Ethereum et de Bitcoin :

- Ethereum utilise une marchine virtuelle (turing complete). Même si dans le script de bitcoin il existe une certaine logique, elle est beaucoup plus avancée chez Ethereum. La machine virtuelle va créer un back code compris entre 0 et 1. C'est elle qui sera à l'origine de toutes les opérations et est même présente dans des noeuds Ethereum.

Chaque execution faite sur le réseau, Ethereum facture un cout spécifique ( voir lien en dans les ressources à connaître)

- Ethereum offre la possibilité d'y déployer des smart contract

Ethereum a introduit la notion de gas pour les frais de transactions

## Ressources importantes à connaître:

- Bitcoin white paper: https://bitcoin.org/bitcoin.pdf

- Ethereum yellow paper: https://ethereum.github.io/yellowpaper/paper.pdf

- https://ethervm.io/
