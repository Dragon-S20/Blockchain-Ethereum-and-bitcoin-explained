# Blockchain-Ethereum-and-bitcoin-explained

## Les caractéristiques d'une blockchain:

// Une blockchain est un registre comptable distribué (Distributed Ledger Technology).

// On dit que la chaine est immuable car il n'existe pas qu'un seul point d'autorité. En somme, le réseau distribué est une réponse à l'expression du "single point of authority, single point of failure".

// Sur une blockchain, toutes les transactions sont inscrites au journal

// Une blockchain est un ensemble de block disponible sur un réseau distribué

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

1. Preuve de travail (PoW) 1

La preuve de travail est le principe originel implanté dans la première blockchain. Ce principe au départ était utilisé pour lutter contre le spam.

C'est un consensus algorithmique garantissant l'intégrité du minage. Chaque mineur se doit résoudre un puzzle plus ou moins difficile. La difficulté va varier en fonction du temps de minage. C'est-à-dire qu'en cas de minage rapide, les prochains puzzles seront plus difficiles

Le puzzle consiste à trouver un numéro de hash plus grand que celui présent dans le block header _(target)_. Pour ce faire, les mineurs vont utiliser le _nonce_ (un champs qui au début de la résolution de problème sera vide) et y inscrire tout ce qui va être utile à la résolution du problème.

Le mineur qui aura résolu le problème obtiendra une récompense pour le travail fournit.

1. Preuve d'enjeu (PoS) 2

La preuve d'enjeu est un concept créée par éthereum pour palier à la grande demande d'énergie demandé par le PoW.
Avec la preuve d'enjeu, le créateur du prochain bloc de la chaine est celui ayant laissé une caution de minimum 32ETH.

Au final, Ethereum change le paradigme du mécanisme de confiance, en implantant ce concept. L'intégrité de la chaîne n'est alors garantit que par ceux qui y ont des intérêts (gros montant d'ETH).

1. Le minage 3

Le minage est un processus couteux. Il est exécuté par des mineurs attirés par la récompense et de hauts frais de transactions. Plus les frais de transactions proposés seront haut et plus le minage de a transactions à effecté sera fait rapidement.

## Les frais de transaction:

## Le chiffrement asymétrique:

## Les particularités d'Ethereum:
