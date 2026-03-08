# Guide de Création d'un Article

Ce document explique comment créer un nouvel article pour le journal **Info connectée**. Suivez ces étapes pour que votre article s'affiche correctement avec le bon design.

## 1. Créer le fichier
Tous les articles doivent être créés dans le dossier : `content/posts/`
Le nom du fichier doit finir par `.md` (ex: `ma-super-sortie.md`).

## 2. Modèle à copier-coller
Copiez ce bloc au tout début de votre fichier et remplissez les informations :

```markdown
---
title: "Titre de votre article"
date: 2026-03-08
rubriques: ["nom_de_la_rubrique"]
description: "Un court résumé de l'article qui apparaîtra sur la page d'accueil."
image: "images/nom_de_votre_image.png"
draft: false
---

Ici, vous écrivez le contenu de votre article. 
Vous pouvez sauter des lignes pour faire des paragraphes.
```

## 3. Les Rubrivques Valides
Pour que l'article apparaisse dans la bonne catégorie et soit bien surligné dans le menu, utilisez **uniquement** l'un de ces mots (tout en minuscules) entre les crochets `[" "]` :

*   `actualite` (pour Actualité)
*   `sport` (pour Sport)
*   `sante` (pour Santé)
*   `culture` (pour Culture)
*   `social` (pour Social)
*   `planete` (pour Planète)
*   `economie` (pour Économie)
*   `sciences` (pour Sciences)

## 4. Les Images
*   Mettez vos images dans le dossier : `static/images/`
*   Dans l'article, indiquez simplement le chemin : `image: "images/mon-image.jpg"`

## 5. Astuces
*   **Titre** : Mettez-le entre guillemets `" "`.
*   **Date** : Utilisez le format `AAAA-MM-JJ`.
*   **Brouillon** : Si vous mettez `draft: true`, l'article ne sera pas visible sur le site public. Mettez `draft: false` pour le publier.
*   **Gras** : Utilisez des doubles étoiles `**texte en gras**`.
