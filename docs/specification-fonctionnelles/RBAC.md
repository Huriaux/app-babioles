# Contrôle d'accès basé sur les rôles (RBAC)

***Le *RBAC* est une méthode pour réguler l'accès aux ressources d'un système informatique. Dans cette approche, les permissions de faire certaines actions sont données à des rôles spécifiques plutôt qu'à des individus.***

*Il va donc servir ici à simplifier la gestion des droits d'accès et permettre aux administrateurs de contrôler qui peut accéder à quoi dans un système, en associant des utilisateurs à des rôles en fonction de leurs responsabilités. Cela aide à sécuriser les données sensibles et à garantir que chaque utilisateur ait uniquement l'accès nécessaire pour effectuer ses tâches.*

<br>

## <u>**Définition des rôles**</u>

- `Administrateur` : C'est la personne qui gère et contrôle l'ensemble du site, incluant la gestion des utilisateurs, des produits et des paramètres de l'application.
    - *Il a des permissions étendues pour la gestion du contenu et des utilisateurs mais n'effectue pas d'achats.*

- `Utilisateur` : C'est un visiteur inscrit sur le site qui peut parcourir les produits, effectuer des achats et gérer son compte personnel.
    - *Il n'a aucun accès aux fonctionnalités administratives ou de développement.*

- `Employé` : C'est le personnel chargé de la gestion quotidienne des opérations relatives aux produits et commandes.
    - *Il peut gérer le stock, mettre à jour les catégories et le statut des commandes, mais ne gère pas les utilisateurs ni les aspects techniques du site.*

- `Développeur` : C'est le professionnel technique chargé du développement, de la maintenance et de l'optimisation du site web.
    - *Il a accès aux outils et à la base de données pour la maintenance et les mises à jour mais ne gère pas les aspects commerciaux ou utilisateur du site.*

<br>

## <u>**Tableau des permissions**</u>
Ce tableau décrit les niveaux d'accès pour chaque rôle défini au sein de l'application, permettant une gestion claire et sécurisée des fonctionnalités selon les responsabilités assignées à chaque rôle.

| **Permissions**                          | `Utilisateur` | `Administrateur` | `Employé` | `Développeur` |
|------------------------------------------|:-------------:|:----------------:|:---------:|:-------------:|
| Parcourir les produits                   | 🟢            | 🟢               | 🟢        | 🟢            |
| Effectuer des achats                     | 🟢            | 🔴               | 🔴        | 🔴            |
| Gérer son compte personnel               | 🟢            | 🔴               | 🔴        | 🔴            |
| Modifier les paramètres du site          | 🔴            | 🟢               | 🔴        | 🔴            |
| Accéder aux rapports de vente            | 🔴            | 🟢               | 🔴        | 🔴            |
| Gérer les utilisateurs                   | 🔴            | 🟢               | 🔴        | 🔴            |
| Gérer les commandes                      | 🔴            | 🟢               | 🔴        | 🔴            |
| Accéder aux outils de développement      | 🔴            | 🔴               | 🔴        | 🟢            |
| Déployer ou mettre à jour le site        | 🔴            | 🔴               | 🔴        | 🟢            |
| Accéder à la base de données             | 🔴            | 🟢               | 🔴        | 🟢            |
| Gérer la sécurité du site                | 🔴            | 🟢               | 🔴        | 🟢            |
| Gérer le stock                           | 🔴            | 🟢               | 🟢        | 🔴            |
| Mettre à jour le statut des commandes    | 🔴            | 🟢               | 🟢        | 🔴            |
| Créer et gérer les catégories            | 🔴            | 🟢               | 🟢        | 🔴            |

<br>

> <u>**Légende :**</u>\
> 🟢 a accès\
> 🔴 n'a pas accès


---
<!-- Bouton 'Retour vers le Sommaire' et Bouton 'Retour vers haut' du document -->
<div align="right">
    <a href="#contrôle-daccès-basé-sur-le-rôle-rbac">
        <img src="../assets/icon-vers-le-haut.png" alt="Retour vers le haut" style="width: 25px;" />
    </a>
</div>
<div align="left">
    <a href="/README.md">
        <img src="../assets/summary.png" alt="Retour vers le sommaire" style="width: 100px;" />
    </a>
</div>
