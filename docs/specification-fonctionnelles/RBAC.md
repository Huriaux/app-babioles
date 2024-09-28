# Contrôle d'accès basé sur le rôle (RBAC)

## Définition des rôles


- `Administrateur` : C'est la personne qui gère et contrôle l'ensemble du site, incluant la gestion des utilisateurs, des produits et des paramètres de l'application.
    - *Il a des permissions étendues pour la gestion du contenu et des utilisateurs mais n'effectue pas d'achats.*

<br>

- `Développeur` : C'est le professionnel technique chargé du développement, de la maintenance et de l'optimisation du site web.
    - *Il a accès aux outils et à la base de données pour la maintenance et les mises à jour mais ne gère pas les aspects commerciaux ou utilisateur du site.*

<br>

- `Utilisateur` : C'est un visiteur inscrit sur le site qui peut parcourir les produits, effectuer des achats et gérer son compte personnel.
    - *Il  n'a aucun accès aux fonctionnalités administratives ou de développement.*

## Tableau des permissions
Ce tableau décrit les niveaux d'accès pour chaque rôle défini au sein de l'application, permettant une gestion claire et sécurisée des fonctionnalités selon les responsabilités assignées à chaque rôle.


| **Permissions**                  | **Utilisateur** | **Administrateur** | **Développeur** |
|----------------------------------|:---------------:|:------------------:|:---------------:|
| Parcourir les produits           | 🟢             | 🟢                | 🟢             |
| Effectuer des achats             | 🟢             | 🔴                | 🔴             |
| Gérer son compte personnel       | 🟢             | 🔴                | 🔴             |
| Ajouter ou retirer des produits du panier  | 🔴             | 🟢                | 🔴             |
| Modifier les paramètres du site  | 🔴             | 🟢                | 🔴             |
| Accéder aux rapports de vente    | 🔴             | 🟢                | 🔴             |
| Gérer les utilisateurs           | 🔴             | 🟢                | 🔴             |
| Accéder aux outils de développement | 🔴          | 🔴                | 🟢             |
| Déployer ou mettre à jour le site | 🔴            | 🔴                | 🟢             |
| Accéder à la base de données     | 🔴             | 🟢                 | 🟢             |
| Gérer la sécurité du site        | 🔴             | 🟢                | 🟢             |

>---
> <u>Légende :</u>\
>🟢 : a accès\
>🔴 : n'a pas accès
>
>---

---
<!-- Bouton 'Retour vers le Sommaire' et Bouton 'Retour vers haut' du document -->
<div align="right">
    <a href="#contrôle-daccès-basé-sur-le-rôle-rbac">
        <img src="../assets/icon-vers-le-haut.png" alt="Retour vers le haut" style="width: 25px;" />
    </a>
</div>
<div align="left">
    <a href="/README.md">
        <img src="../assets/summary.png" alt="Retour vers le haut" style="width: 100px;" />
    </a>
</div>