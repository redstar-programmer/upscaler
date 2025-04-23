# upscaler redstar
Puissant outil d'upscaling vidéo utilisant FFmpeg, Real-ESRGAN, Flowframes - supporte maintenant **l'interface multilingue** !

## 🌐 Langue / Paramètres de langue
[한국어](https://github.com/redstar-programmer/upscaler/blob/main/README.md) | [English](https://github.com/redstar-programmer/upscaler/blob/main/README/README.en.md) | [日本語](https://github.com/redstar-programmer/upscaler/blob/main/README/README.ja.md) | [中文](https://github.com/redstar-programmer/upscaler/blob/main/README/README.zh.md) |
[Français](https://github.com/redstar-programmer/upscaler/blob/main/README/README.fr.md) | [Deutsch](https://github.com/redstar-programmer/upscaler/blob/main/README/README.de.md) | [Español](https://github.com/redstar-programmer/upscaler/blob/main/README/README.es.md) | [Português](https://github.com/redstar-programmer/upscaler/blob/main/README/README.pt.md) |
[Русский](https://github.com/redstar-programmer/upscaler/blob/main/README/README.ru.md) | [Italiano](https://github.com/redstar-programmer/upscaler/blob/main/README/README.it.md) | [Tiếng Việt](https://github.com/redstar-programmer/upscaler/blob/main/README/README.vi.md) | [Bahasa Indonesia](https://github.com/redstar-programmer/upscaler/blob/main/README/README.id.md) |
[ภาษาไทย](https://github.com/redstar-programmer/upscaler/blob/main/README/README.th.md) | [العربية](https://github.com/redstar-programmer/upscaler/blob/main/README/README.ar.md)

<p align="centre">
  <img src="https://github.com/user-attachments/assets/632c3a83-5416-46c3-8d38-0e1bf153b633" height="250"/>
</p>

<p align="centre">
  <strong>Outil d'upscaling vidéo basé sur fmpeg, realesrgan, flowframes</strong><br><br>.
  <em>Moderne, basé sur une interface graphique, paramètres prédéfinis, prise en charge du traitement multi-fichier</em>.
</p>

---.

Télécharger : [Release](https://github.com/redstar-programmer/upscaler/releases/)

## ✨ Please support 'redstar' upscaler

Vous aimez ce projet ou souhaitez soutenir son développement ?
Faites un petit don pour nous aider à développer de meilleures fonctionnalités et des mises à jour fiables !

- <img src="https://img.shields.io/badge/Donate-PayPal-blue.svg?logo=paypal" height="20"/><br>**PayPal** : [https://paypal.me/redstarprogrammer?country.x=KR&locale.x=ko_KR](https://paypal.me/redstarprogrammer?country.x=KR&locale.x=ko_KR)
- <img src="https://img.shields.io/badge/Sponsor-GitHub%20Sponsors-ff69b4?logo=githubsponsors" height="20"/><br>**GitHub Sponsors** : [https://github.com/sponsors/redstar-programmer](https://github.com/sponsors/redstar-programmer)


> 💡 Votre parrainage des coûts du serveur, du temps de développement et d'une tasse de café est très utile. Nous vous remercions !

## Table des matières

- 👋 Introduction](#Introduction)
- 💾 Installation et préparation](#Installation-et-préparation)
- 🔧 Caractéristiques principales](#Main-Features)
- 🚀 Mode d'emploi (démarrage rapide)](#Mode d'emploi-démarrage rapide)
- [⚙️ Description détaillée des fonctionnalités](#detailed-feature-description)
- 🙏 Remerciements](#Remerciements)
- 📜 Historique](#histoire)

## 👋 Introduction
**L'upscaler de Redstar est un outil GUI basé sur Python qui permet d'upscaler automatiquement des vidéos vers des résolutions plus élevées en utilisant `ffmpeg`, `Real-ESRGAN` et `Flowframes`.

- Extraire des images vidéo → upscale → fusionner des vidéos en une seule étape
- Prise en charge de divers modèles de realesrgan
- Interpolation optionnelle via Flowframes
- Extraction et traitement automatiques des codecs audio
- Travail sur l'emplacement de la source ou sur un chemin spécifié

> ⚠️ Développé et testé dans un environnement Windows.

Vous trouverez ci-dessous une démonstration d'utilisation simple, cliquez dessus pour être dirigé vers YouTube:<br>
[ ![Regarder la démo](https://img.youtube.com/vi/G-JTWRws3co/0.jpg)](https://youtu.be/G-JTWRws3co "Regarder sur YouTube")

## 💾 Installation et préparation

1. installez et localisez les outils externes suivants (notez que le fichier de distribution inclut les fichiers d'installation de ffmpeg, Real-ESRGAN et Flowframes (voir le dossier Programs dans le chemin d'accès))
   - [ffmpeg](https://www.ffmpeg.org/download.html)
   - Real-ESRGAN](https://github.com/xinntao/Real-ESRGAN/releases)
   - Flowframes](https://github.com/n00mkrad/flowframes) *(optionnel)*.
2. décompressez et exécutez le fichier upscaler.exe de readstar
3. dans le cas de Flowframes, les modèles chargés peuvent être différents en fonction de l'environnement de l'utilisateur ; veillez donc à exécuter Flowframes et à vous assurer que l'IA d'interpolation et le modèle d'IA dans l'onglet Interpolation correspondent à la version de resources/flowframes_models.ini de l'upscaler redstar. <br>Commentez les modèles qui ne sont pas chargés en les marquant d'un # et assurez-vous que l'ordre des modèles dans la fenêtre des paramètres de l'upscaler redstar correspond à l'ordre des modèles dans <br>Flowframes> avant de poursuivre.

## 🔧 Principales caractéristiques.

![Image](https://github.com/user-attachments/assets/93dc232e-8742-4ae3-b335-9395c26a61f4)
- ✅ Sélection multiple d'images et fonctionnement séquentiel
- ✅ Ajout de vidéos par glisser/déposer
- ✅ Disponibilité des programmes principaux et sélection directe
- Mode d'économie de disque
- ✅ Prise en charge multilingue (15 langues)
<br><br>
![Image](https://github.com/user-attachments/assets/3341f4ca-af20-4647-93d0-484146dc6757)
- Sauvegarde des préréglages et application automatique
- Détection automatique des codecs audio et réglage du débit binaire
- Détection et sélection automatiques des modèles de realesrganes
- ✅ Paramètres détaillés pour FFMPEG, real-ESRGAN et Flowframes
- ✅ Modification des paramètres des options en fonction de la version de Flowframes<br>(la version peut être modifiée en spécifiant le chemin de la version dans Flowframes sur la page principale)
<br><br>
![Image](https://github.com/user-attachments/assets/25d60d82-53a2-4064-bbef-d439d9a9d3d6)
- ✅ Vérifier la commande d'exécution de la mise à l'échelle (peut être copiée et exécutée séparément sur CMD).
<br><br>
![Image](https://github.com/user-attachments/assets/2fd69862-d038-401d-a9a6-83dc84c769f0)
- Contrôler la progression générale de l'opération de mise à l'échelle
- Vérifier la journalisation de la montée en gamme (les fichiers journaux sont créés par date dans le dossier journal du dossier live).
- Nettoyer automatiquement les livrables à la fin de la tâche (préfixés par [REDSTAR])
- ✅ Définir l'action après la fin de la tâche<br>( Ne rien faire / Quitter le programme / Sommeil / Mode hibernation / Fermer la fenêtre)
<br><br>
## 🚀 Comment utiliser (Démarrage rapide)

1. ajouter des fichiers vidéo (MP4, MKV, AVI, MOV, FLV, WMV, MPG, WEBM, 3GP, OGV pris en charge)
2. spécifiez l'emplacement de travail ou cochez la case "Utiliser le chemin d'accès d'origine".
3. cliquez sur le bouton "Paramètres" de la vidéo ajoutée
4. paramètres détaillés de ffmpeg, realESRGAN, Flowframes
5. cliquez sur Appliquer par lots à tous les fichiers / Appliquer aux fichiers sélectionnés uniquement
6. cliquez sur le bouton "Confirmer
7. vérifiez les commandes à exécuter et cliquez sur le bouton "Démarrer la tâche

> Le résultat de la tâche sera deux fichiers : la vidéo upscalée et la vidéo interpolée dans le dossier sélectionné.
> Les fichiers terminés seront enregistrés avec le préfixe [REDSTAR].
---]

## ⚙️ Description détaillée de la fonction

| Description de l'article | Description de l'article
|------|------|
| Définir le chemin d'accès** | Fournir le chemin d'accès par défaut ou l'option "Utiliser le chemin d'accès du fichier d'origine".
| La plupart des formats sont pris en charge, y compris MP4, MKV, AVI, MOV, FLV, WMV, MPG, WEBM, 3GP, OGV, etc.
| Les modèles de mise à l'échelle sont détectés automatiquement par realesr-animevideov3, realesr-general, 4xplus, etc.
| Le traitement audio*** prend en charge l'encodage de divers formats tels que `aac`, `mp3`, `flac`, etc.
| L'interpolation (FPS ×2, ×4, ×8) peut être réglée.
| Mode d'économie de disque** | Suppression automatique des images intermédiaires

## 🙏 Remerciements

- realesrgan par [xinntao](https://github.com/xinntao/Real-ESRGAN)
- flowframes par [n00mkrad](https://github.com/n00mkrad/flowframes)
- Si vous souhaitez contribuer à ce projet ou suggérer une fonctionnalité, veuillez laisser un commentaire sur [Issues](https://github.com/redstar-javscraper/redstar_upscaler/issues).

# 📜 History

v 1.1.0
 > 1. configuration du menu (ouvrir le fichier, fermer le fichier, paramètres du journal, paramètres de la langue)
 > 2. ajout de paramètres multilingues (langues disponibles : coréen, anglais, 日本語, 中文, français, allemand, espagnol, portugais, Русский, Tiếng Việt, Bahasa Indonesia, ไทย, Italiano, العربية)
 > 3. modification des messages et d'une partie du code pour tenir compte de l'ajout des paramètres linguistiques
 > 4. quelques changements dans la configuration de l'interface utilisateur
 > 5. affichage des informations sur la version de ffmpeg, real-ESRGAN et Flowframes (écran principal)
 > 6. prise en charge de la version 1.41.0 de Flowframes (actuellement, seules les versions 1.40.0 et 1.36.0 sont disponibles en raison d'un problème de commande cmd dans la version 1.41.0)
 > 7. correction d'un problème où les éléments des modèles AI étaient affichés en lettres minuscules
 > Ajout d'options FFMPEG (Pixel, codec vidéo) - les options sont affichées en fonction du PC de l'utilisateur
 > Amélioration de la vérification CUDA pour chaque PC de l'utilisateur - vérification de la disponibilité et du type de GPU (écran principal)

v 1.0.0
 > 1. réécriture complète du code
 > 2. modifications de l'interface utilisateur
 > Augmentation de la gamme de vidéos/audios pouvant être traités
 > 4. ajout d'un mode d'économie de disque
 > 5. distribution incluant les principaux programmes

v 0.1.92
 > 1. correction d'un problème qui provoquait l'échec de l'interpolation en raison de la duplication des entrées dans la liste déroulante du modèle AI lors de la modification du chemin d'accès aux images de flux (Flowframes)
 > Ajout d'un code de vérification de l'état de sélection de la liste déroulante lors de l'interpolation.

v 0.1.91
 > Ajout de quelques fonctions de rafraîchissement des combobox liées à Flowframes.
 > Ajustement de certains fichiers de distribution

v 0.1.9
 > Appliquer les changements du modèle Flowframes
 > 2. nouveau modèle Flowframes 1.36.0, implémentation du modèle 1.40.0
 > L'échec de la ligne de commande Flowframes ne se produit plus.
 Les fichiers peuvent maintenant être ajoutés par glisser/déposer > 5.
 > Correction des paramètres de Flowframes qui ne sont pas appliqués

v 0.1.8
 Correction de l'erreur de vérification de la nouvelle version lors de la vérification de la version > 2.
 > Si flowframes est installé dans le chemin d'accès par défaut (ex. C:³Users³Administrator³AppData³Local³Flowframes³), définissez le chemin d'accès par défaut avant de démarrer.
 > Lors de l'ajout de sélections de fichiers multiples, l'application se bloque en raison d'une erreur.
 > Correction d'une erreur lors du démarrage de la tâche après l'ajout de plusieurs fichiers.

v 0.1.7
 > La taille du programme peut être modifiée
 > Correction d'une erreur lors de l'utilisation de fichiers sans voix
 > 3. modification de la configuration de l'interface utilisateur (reconfigurée pour s'adapter au changement de taille)

v 0.1.6
 > 1. correction d'un problème lié à la différence de taille des polices en fonction de la résolution de l'écran
 > 2. correction d'un problème où le titre du programme n'affichait pas les informations de version comme une nouvelle version
 > 3. correction d'un problème où le fichier config.ini était sauvegardé dans un chemin différent
 > 4. lors de la modification du multiplicateur de mise à l'échelle de l'organe réel, la liste déroulante du modèle de mise à l'échelle est également modifiée.
 > Ajout d'une fonction de vérification de la mise à jour
 > 6. correction d'une partie de la logique
 > 7. modification de la couleur des tableaux de résolution et de fps
 > Permettre à l'utilisateur de modifier la résolution (doit être saisie comme 1024x768)

v 0.1.5
 > Correction d'un problème où le modèle AI n'est pas automatiquement modifié lors de la sélection de l'interpolation FLOWFRAMES AI.
 > Correction d'un problème où l'interpolation des images de flux n'était pas interpolée en fonction de l'option sélectionnée.
 > Ajout d'une liste déroulante "Méthode de calcul du FPS" pour éviter un calcul incorrect du FPS pour certaines vidéos.
        -> r_frame_rate / avg_frame_rate, par défaut r_frame_rate
 > 4. afficher la progression de la récupération des informations vidéo lors de la sélection d'un fichier vidéo
 > 5. changer la valeur par défaut pour ouvrir le dernier dossier sélectionné lors de la sélection d'un fichier après l'ouverture de ce dernier.

v 0.1.4
 > 1. modification de la lecture du fichier config.ini
 > 2. modification de la façon de récupérer les informations vidéo de Python AV vers ffmpeg
 > 3. ajout de la fermeture de la fenêtre lorsque la tâche est terminée
 > 4. afficher le nom complet du fichier comme info-bulle au passage de la souris dans la liste des tâches
 > 5. affichage de la résolution (avant) / résolution (après) / FPS (avant) / FPS (après) pour chaque fichier dans la liste des tâches
 > 6. supprimer le champ de saisie du FPS (en raison de l'étiquetage ci-dessus pour chaque fichier)
 > 7. supprimer la taille estimée du FPS de sortie (supprimée en raison de l'étiquetage ci-dessus spécifique à chaque fichier)
 > 8. afficher la progression sous forme de deux barres de progression pour tous les fichiers/travaux

v 0.1.3
 > Correction de l'erreur de calcul du FPS du fichier, où certaines informations sur le FPS étaient erronées lors du chargement des fichiers.

v 0.1.2
 > 1. modifications de la configuration de l'interface utilisateur
 > 2. modifications de la logique interne
 > 3. correction du problème qui faisait que le modèle realesrgan ne fonctionnait pas lorsque l'on sélectionnait deux des modèles suivants
 > 4. modification de la façon d'utiliser les modèles realesrgan
 > Copiez le nouveau fichier de modèle (*.param) dans le dossier models du dossier d'installation de realesrgan et vous pourrez l'utiliser.
 > 5. afficher les informations sur la largeur, la hauteur et la taille estimée de l'échelle supérieure du dernier fichier de l'image cible à utiliser
 > 6. écrire le code pour migrer le fichier config.ini
 > 7. changer l'image de décomposition FFMPEG AAC -> FLAC
 > 8. autres corrections de bogues

v 0.1.1
 > 1. première écriture d'un programme d'upscaling vidéo avec ffmepg, realesrgan et flowframes