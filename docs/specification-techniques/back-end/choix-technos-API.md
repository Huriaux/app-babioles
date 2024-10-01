## Choix des technos côté API

## Création d'une API en Python avec une architecture en couches

**1. <u>Django**</u> est un framework Python complet qui suit une architecture de type MTV (Model-Template-View), proche de l'architecture en couches :

- ***Couche Présentation*** : Gérée par les vues, qui reçoivent les requêtes HTTP et renvoient des réponses (JSON, HTML).
- ***Couche Métier (Business)*** : Peut être séparée dans des fichiers/services dédiés, pour encapsuler la logique métier.
- ***Couche Persistance*** : Gérée par les modèles via l'ORM intégré, pour interagir avec la base de données.

**2. <u>FastAPI**</u> est un framework léger et rapide pour créer des APIs. Il permet de structurer le projet en couches :

- ***Couche Présentation*** : Les routes gèrent les requêtes HTTP et les réponses, appelant les services métier.
- ***Couche Métier (Business)*** : La logique métier est isolée dans des services pour séparer les règles de gestion.
- ***Couche Persistance*** : Utilisation de SQLAlchemy ou autre ORM pour gérer l'accès aux données, en séparant la logique de persistance.


---
<!-- Bouton 'Retour vers le Sommaire' et Bouton 'Retour vers haut' du document -->
<div align="right">
    <a href="#choix-des-technos-côté-serveur">
        <img src="../../assets/icon-vers-le-haut.png" alt="Retour vers le haut" style="width: 25px;" />
    </a>
</div>
<div align="left">
    <a href="/README.md">
        <img src="../../assets/summary.png" alt="Retour vers le haut" style="width: 100px;" />
    </a>
</div>