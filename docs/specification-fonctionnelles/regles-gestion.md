# Règles de gestion

***Les règles de gestion définissent comment les informations doivent être traitées pour assurer que tout fonctionne correctement et efficacement. Elles sont comme des instructions qui guident automatiquement l'application à prendre des décisions et à effectuer des tâches de manière consistante.***

*Cela aide à éviter les erreurs et à s'assurer que l'application répond bien à vos besoins spécifiques. En les suivant, l'application peut opérer de façon autonome dans beaucoup de situations, ce qui facilite la gestion au quotidien.*

<br><br>

## Entités
`Utilisateur` : **représente les personnes inscrites sur le site pour effectuer des achats ou gérer leur compte.**
- Contient des détails tels que le nom, le prénom, le numéro de téléphone, l'adresse email, le mot de passe, le sexe, la date de naissance.

<br>

`Employé` : **représente les employés du site qui gèrent l'inventaire des produits et les opérations quotidiennes liées aux articles et aux commandes.**
- Contient des détails tels que le nom, le prénom, nom du poste, l'adresse email, le mot de passe et le numéro de téléphone.

<br>

`Article` : **représente les différents articles disponibles à l'achat sur le site.**
- Contient des informations telles que le nom du produit, la description et le prix.

<br>

`Catégorie` : **regroupe différents articles sous une classification commune pour faciliter la navigation et l'organisation des produits sur le site.**
- Contient le nom de la catégorie.

<br>

`Stock` : **représente la quantité disponible d'un article spécifique.**
- Contient des informations telles que la quantité actuelle disponible.

<br>

`Commande` : **représente une transaction où des produits sont sélectionnés et achetés par un utilisateur.**
- Contient des informations telles que la date de commande, le nombre d'articles et le montant total.

<br>

`Adresse de Livraison` : **représente les informations de livraison spécifiques à chaque commande passée par l'utilisateur.**
- Contient des détails tels que le numéro de rue, la rue, le complément d'adresse, le code postal, la ville et le pays.

<br>

`Statut` : **représente l'état actuel d'une commande, essentiel pour le suivi par les utilisateurs et l'administration.**
- Contient des informations telles que les différents statuts possibles incluent des états comme "En cours de préparation", "Expédiée", "Annulée".

<br>

`Mode de Paiement` : **représente les informations de la carte bancaire qu'un utilisateur peut enregistrer pour payer ses commandes.**
- Contient des détails tels que le type de carte (Visa, MasterCard, etc.), le numéro de la carte, la date d'expiration, le cryptogramme et le nom du titulaire de la carte.

<br><br>

## Règles de gestion

### Compte de l'utilisateur
- L'`Utilisateur` doit pouvoir s'inscrire avec une adresse email valide et créer un mot de passe selon des critères de sécurité définis.

- L'`Utilisateur` doit pouvoir se connecter en utilisant son email et mot de passe.
    - L'`Utilisateur` doit pouvoir modifier ses informations personnelles à tout moment, sauf son adresse email.

<br>

- L'`Utilisateur` doit pouvoir demander la suppression de son compte, qui sera confirmée par l'administrateur après vérification.

<br>

### Gestion des articles
- Un `Article` appartient à une `Catégorie`

- Un `Article` dispose d'un `Stock`

<br>

- L'`Utilisateur` doit pouvoir ajouter un `Article` à son panier.

    - L'`Utilisateur`doit pouvoir modifier la quantité d'un `Article` de son panier.

    - L'`Utilisateur`doit pouvoir retirer undes `Article`(s) de son panier.

<br>

- Un `Employé` doit pouvoir ajouter des nouveaux `Article`(s).

- Un `Employé` doit pouvoir créer une nouvelle `Catégorie` d'articles.

    - Un `Employé` doit pouvoir assigner des articles à une `Catégorie`.

- Un `Employé` doit pouvoir mettre à jour le `Stock` des articles.

<br>

### Gestion des commandes
- L'`Utilisateur` doit pouvoir valider une `Commande`, s'il est authentifié.

    - L'`Utilisateur` doit pouvoir sélectionner son `Adresse de livraison`.

    - L'`Utilisateur` doit pouvoir sélectionner son `Mode de paiement`.

        - L'`Utilisateur` doit pouvoir finaliser la `Commande`.

<br>

- Une `Commandes` passée doit disposer d'un `Statut`.

    - La `Commande` passée doit pouvoir afficher le `Statut` à l'utilisateur.

    - Un `Employé` doit pouvoir mettre à jour le `Statut` de la commande.


<br>

- L'`Utilisateur` doit pouvoir demander l'annulation `Commande`.

    - Une `Commande` doit pouvoir être annulées, qui sera confirmée par l'administrateur après vérification du statut de commande.


---
<!-- Bouton 'Retour vers le Sommaire' et Bouton 'Retour vers haut' du document -->
<div align="right">
    <a href="#règles-de-gestion">
        <img src="../assets/icon-vers-le-haut.png" alt="Retour vers le haut" style="width: 25px;" />
    </a>
</div>
<div align="left">
    <a href="/README.md">
        <img src="../assets/summary.png" alt="Retour vers le haut" style="width: 100px;" />
    </a>
</div>