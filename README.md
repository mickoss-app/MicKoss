<h1 align="center">MicKoss</h1>
<p align="center"><em>Le karaoké intelligent qui transforme n'importe quelle chanson en outil d'apprentissage du chant.</em></p>

<p align="center">
  <a href="https://mickoss.com/"><img src="https://img.shields.io/badge/Site_officiel-mickoss.com-13233f?style=for-the-badge&labelColor=13233f&color=b8862c" alt="Site officiel"></a>
  <a href="https://github.com/mickoss-app/MicKoss"><img src="https://img.shields.io/badge/GitHub-Projet-13233f?style=for-the-badge&logo=github&logoColor=white&labelColor=13233f&color=b8862c" alt="GitHub Projet"></a>
  <a href="https://github.com/godson-kossi"><img src="https://img.shields.io/badge/GitHub-Profil-13233f?style=for-the-badge&logo=github&logoColor=white&labelColor=13233f&color=b8862c" alt="GitHub Profil"></a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/FastAPI-Python-0b3d2e?style=flat-square" alt="FastAPI">
  <img src="https://img.shields.io/badge/React-Vite-1a1a2e?style=flat-square" alt="React">
  <img src="https://img.shields.io/badge/PostgreSQL-Base_de_données-1a1a2e?style=flat-square" alt="PostgreSQL">
  <img src="https://img.shields.io/badge/Celery-Redis-1a1a2e?style=flat-square" alt="Celery Redis">
  <img src="https://img.shields.io/badge/Statut-Code_privé-b8862c?style=flat-square" alt="Statut">
</p>

---

> **Ce dépôt est une vitrine du projet.** Il ne contient aucun code source : uniquement une présentation, des captures d'écran et de la documentation, à destination des investisseurs, partenaires et recruteurs. Le code (`MicKoss-Source`) reste privé — accès sur demande, sous NDA si nécessaire.

## Sommaire

- [Le problème, la solution](#le-problème-la-solution)
- [Fonctionnalités](#fonctionnalités)
- [Aperçu de l'application](#aperçu-de-lapplication)
- [Stack technique](#stack-technique)
- [Vérification & accès](#vérification--accès)
- [À propos de ce dépôt](#à-propos-de-ce-dépôt)

## Le problème, la solution

Les outils de karaoké existants forcent un choix : **Smule** mise tout sur le divertissement social avec un catalogue sous licence, sans jamais faire progresser la voix de l'utilisateur ; **Yousician** enferme l'apprentissage vocal structuré dans un catalogue d'exercices fermé, loin des chansons que les gens veulent réellement chanter.

**MicKoss** réunit les deux mondes : à partir d'un simple fichier audio ou d'un lien YouTube — n'importe lequel — la plateforme sépare automatiquement la voix de l'instrumental par IA, synchronise les paroles mot à mot, puis ouvre trois usages sur ce même morceau : le karaoké vidéo, l'entraînement vocal structuré, et la compétition entre utilisateurs.

## Fonctionnalités

**Créer**
- Import multi-source — fichier local (audio/vidéo) ou recherche/import YouTube direct.
- Séparation vocale / instrumentale par intelligence artificielle.
- Transcription et synchronisation automatique des paroles, mot à mot.
- Génération de vidéos karaoké avec fond personnalisable.

**S'entraîner**
- Trois modes dédiés : apprentissage guidé, répétition, modulation vocale.
- Lecteur interactif avec suivi en temps réel des paroles.
- Bibliothèque personnelle — historique et progression conservés.

**Rivaliser & partager**
- Mode compétition : défi entre utilisateurs sur un même morceau, enregistrement et classement.
- Comptes utilisateurs, système de crédits et abonnements (Stripe).
- Traitement asynchrone multi-utilisateurs — plusieurs personnes traitent leurs fichiers en parallèle sans se bloquer.

## Aperçu de l'application

### Créer un karaoké

L'utilisateur importe un fichier ou colle un lien YouTube ; la plateforme prend le relais pour la séparation audio et le suivi de traitement, en temps réel.

<p align="center"><img src="screenshots/02-dashboard.png" alt="Tableau de bord" width="800"></p>

### Bibliothèque et découverte

Paroles en vedette, chansons proposées en compétition et créations récentes : un point d'entrée unique vers tout ce que l'utilisateur (et la communauté) a déjà généré.

<p align="center"><img src="screenshots/03-bibliotheque.png" alt="Bibliothèque et compétition" width="800"></p>

### Paroles synchronisées & lecture karaoké

Le cœur technique du produit : une synchronisation mot à mot précise, y compris sur les morceaux avec une longue intro instrumentale — un cas qui met en échec la plupart des outils grand public.

<p align="center"><img src="screenshots/04-karaoke-lecteur.png" alt="Paroles synchronisées et lecteur karaoké" width="800"></p>

### Habillage vidéo automatique

Chaque session peut être exportée en vidéo, dans plusieurs styles visuels générés automatiquement — prête à partager sur les réseaux sociaux.

<p align="center"><img src="screenshots/05-video-styles.png" alt="Génération vidéo" width="800"></p>

### Mode compétition

Deux utilisateurs s'affrontent sur le même morceau : la mécanique sociale qui manque aux outils d'apprentissage purs, empruntée aux jeux de rythme et à la gamification façon Duolingo.

<p align="center"><img src="screenshots/06-competition.png" alt="Mode compétition" width="800"></p>

### Un modèle freemium pensé pour la rétention

Seule la création d'un nouveau contenu consomme des crédits — l'entraînement et la compétition sur du contenu déjà généré restent gratuits à vie, y compris pour un compte à 0 crédit.

<p align="center"><img src="screenshots/07-tarifs.png" alt="Formules d'abonnement" width="800"></p>

## Stack technique

| Composant | Technologies |
| --- | --- |
| Backend | Python, FastAPI |
| Frontend | React, Vite |
| Base de données | PostgreSQL |
| Traitement asynchrone | Celery, Redis |
| Infrastructure | Docker, Nginx, Hetzner |
| Stockage objet | Cloudflare R2 (compatible S3) |
| Supervision | Prometheus, Grafana |

## Vérification & accès

<p align="center"><img src="link-header.png" alt="MicKoss — liens d'accès et de vérification" width="600" align="bottom"><a href="https://mickoss.com/"><img src="link-site.png" alt="Site officiel : mickoss.com" width="600" align="bottom"></a><img src="link-mid.png" alt="" width="600" align="bottom"><a href="https://github.com/mickoss-app/MicKoss"><img src="link-github-projet.png" alt="GitHub Projet" width="300" align="bottom"></a><a href="https://github.com/godson-kossi"><img src="link-github-profil.png" alt="GitHub Profil" width="300" align="bottom"></a></p>

<details>
<summary>Version PDF du document de vérification</summary>
<p><a href="liens-acces-verification.pdf">liens-acces-verification.pdf</a></p>
</details>

## À propos de ce dépôt

Ce dépôt ne contient **aucun code source**. Il sert uniquement à présenter le projet — fonctionnalités, captures d'écran et documentation de haut niveau — à destination des investisseurs, partenaires et recruteurs.

Pour une démonstration en direct ou un accès au code sous NDA, merci de me contacter directement via mon [profil GitHub](https://github.com/godson-kossi).

---

<p align="center">© MicKoss — Tous droits réservés.</p>
