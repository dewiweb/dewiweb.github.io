---
title: "nextevents"
weight: 8
description: "Suite de diaporamas d'événements OpenAgenda pour les Champs Libres — serveur Docker, app desktop portable et port PHP"
tags: ["openagenda", "affichage-dynamique", "champs-libres", "python", "qt", "php", "docker"]
---

{{< repo-card repo="nextevents" lang="true" >}}

## Présentation

Suite d'outils générant des **diaporamas des événements des Champs Libres** (Rennes) à partir des données OpenAgenda — diapos UHD prêtes pour OBS, affichage dynamique et kiosks.

Trois déclinaisons selon l'infrastructure :

- **[nextevents](https://github.com/dewiweb/nextevents)** — serveur Debian/Docker : scraping leschampslibres.fr + OpenAgenda, rendu PNG **UHD 3840×2160** dans la charte du site (fonte Oldschool Grotesk, fond pastel par événement), web UI avec galerie et rafraîchissement automatique
- **[nextevents-desktop](https://github.com/dewiweb/nextevents-desktop)** — réécriture en **application portable** PySide6/Qt (zip Windows, AppImage Linux) : même génération de diapos + player plein écran natif, sans Docker ni serveur
- **[nextevents-php](https://github.com/dewiweb/nextevents-php)** — port PHP léger pour kiosk : diapos HTML autonomes (fontes/images en base64), aucun PNG à générer, aucune dépendance — le navigateur du kiosk fait le rendu

## Fonctionnalités communes

- Date, durée, lieu, tarif, **public** et **accessibilité** (LSF, audiodescription, surtitrage) extraits des données OpenAgenda
- Images en résolution native, synchros FTP/SMB/local
- Diapo du jour, planificateur, galerie

## Liens

- [nextevents](https://github.com/dewiweb/nextevents) · [nextevents-desktop](https://github.com/dewiweb/nextevents-desktop) · [nextevents-php](https://github.com/dewiweb/nextevents-php)
- Voir aussi [openagenda-slides](/docs/projets/outils-sceniques/openagenda-slides/) — la version généralisée pour tout agenda OpenAgenda public
