# MicKoss

**MicKoss** est une application web de création et de pratique du karaoké : à partir d'un simple fichier audio ou d'un lien YouTube, elle sépare la voix de l'instrumental, génère et synchronise les paroles, puis produit une vidéo karaoké prête à chanter.

> Ce dépôt est une **vitrine** du projet (captures d'écran, fonctionnalités, stack). Le code source est privé — accès sur demande pour les investisseurs, partenaires ou recruteurs intéressés.

## Liens de vérification

<p align="center"><img src="link-header.png" alt="MicKoss — liens d'accès et de vérification" width="700" align="bottom"><a href="https://mickoss.com/"><img src="link-site.png" alt="Site officiel : mickoss.com" width="700" align="bottom"></a><img src="link-mid.png" alt="" width="700" align="bottom"><a href="https://github.com/mickoss-app/MicKoss"><img src="link-github-projet.png" alt="GitHub Projet" width="350" align="bottom"></a><a href="https://github.com/godson-kossi"><img src="link-github-profil.png" alt="GitHub Profil" width="350" align="bottom"></a></p>

<p align="center">
  <a href="https://mickoss.com/"><img src="https://img.shields.io/badge/Site_officiel-mickoss.com-13233f?style=for-the-badge&labelColor=13233f&color=b8862c" alt="Site officiel"></a>
  <a href="https://github.com/mickoss-app/MicKoss"><img src="https://img.shields.io/badge/GitHub-Projet-13233f?style=for-the-badge&logo=github&logoColor=white&labelColor=13233f&color=b8862c" alt="GitHub Projet"></a>
  <a href="https://github.com/godson-kossi"><img src="https://img.shields.io/badge/GitHub-Profil-13233f?style=for-the-badge&logo=github&logoColor=white&labelColor=13233f&color=b8862c" alt="GitHub Profil"></a>
</p>

<p align="center"><em><a href="liens-acces-verification.pdf">Version PDF</a></em></p>

---

## Aperçu

![MicKoss en situation d'usage](screenshots/01-hero.png)
*MicKoss utilisé en studio comme sur mobile.*

![Tableau de bord](screenshots/02-dashboard.png)
*Création d'un karaoké : import, recherche YouTube et suivi des versions générées.*

![Bibliothèque et compétition](screenshots/03-bibliotheque.png)
*Paroles en vedette, chansons en compétition et bibliothèque des créations récentes.*

![Paroles synchronisées et lecteur karaoké](screenshots/04-karaoke-lecteur.png)
*Génération des paroles synchronisées puis lecture karaoké en mode "chanter".*

![Génération vidéo](screenshots/05-video-styles.png)
*Habillage vidéo automatique en plusieurs styles, prêt pour les réseaux sociaux.*

![Mode compétition](screenshots/06-competition.png)
*Deux utilisateurs s'affrontent sur le même morceau en mode compétition.*

![Formules d'abonnement](screenshots/07-tarifs.png)
*Offres Free, Pro, Max et B2B.*

---

## Fonctionnalités

- **Import multi-source** — fichier local (audio/vidéo) ou recherche/import YouTube.
- **Séparation audio** — isolation voix / instrumental par IA.
- **Génération de paroles** — transcription et synchronisation automatique sur la piste audio.
- **Génération vidéo karaoké** — rendu vidéo avec paroles animées et fond personnalisable.
- **Lecteur interactif** — lecture karaoké avec suivi en temps réel des paroles.
- **Mode compétition** — scoring et classement entre utilisateurs.
- **Comptes utilisateurs** — authentification, crédits, paiements.
- **Bibliothèque personnelle** — historique et gestion des morceaux traités.
- **Traitement multi-utilisateurs en parallèle** — plusieurs utilisateurs peuvent traiter leurs fichiers simultanément.

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

## À propos de ce dépôt

Ce dépôt ne contient **aucun code source**. Il sert uniquement à présenter le projet : fonctionnalités, captures d'écran et documentation de haut niveau, à destination des investisseurs, partenaires et recruteurs.

Pour une démonstration en direct ou un accès au code sous NDA, merci de me contacter directement.

---

© MicKoss — Tous droits réservés.
