# SSR et SSG

Pour CE catalogue (quelques dizaines de produits, mis à jour occasionnellement) :

1. Je choisirais le **SSG** : quelques dizaines de fiches qui changent rarement
   peuvent être générées au moment du build. Les pages sont servies rapidement
   en HTML déjà rendu et sont régénérées lors d'une mise à jour du catalogue.

2. Si demain ce site affichait un **stock en temps réel** (quantité
   disponible qui change à chaque commande), ce choix changerait-il ? Pourquoi ?

   Le contenu statique des fiches pourrait rester en SSG, mais le stock devrait
   être récupéré depuis une API au moment de la consultation, ou rendu côté
   serveur (SSR) pour chaque requête. Le HTML généré au build serait trop vite
   obsolète pour garantir une quantité à jour.
