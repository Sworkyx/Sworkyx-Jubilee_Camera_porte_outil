# 📷 README — Installation et utilisation d’une caméra Raspberry Pi Module 3 sur une Jubilee

## Application : Détection de lentilles d’eau

---

## 📌 Description

Ce github vise à intégrer une **caméra Raspberry Pi Module 3** sur la machine Jubilee afin de capturer des images exploitables pour la **détection automatisée de lentilles d’eau**.

Le système repose sur :

* une caméra Raspberry Pi,
* une carte Raspberry Pi (avec OctoPi ou équivalent),
* un accès réseau pour le flux vidéo,
* un script de capture d’images pour traitement ultérieur.

---

## 🛠️ 1. Installation matérielle

### 🔧 Composants nécessaires

* Caméra Raspberry Pi Module 3
* Carte Raspberry Pi
* Carte micro-SD configurée
* Support mécanique - porte outil -
  * https://www.printables.com/model/1679222-pieces-porte-outil-jubilee-raspberry-module-3
  * https://www.printables.com/model/1276113-jubilee-toolhead-adapter-for-enderscope
* Vis de fixation
* Câble nappe (CSI)

---

### ✔️ Vérifications préalables

Avant toute installation :

* Vérifier la qualité d’impression des pièces mécaniques
* S’assurer que la caméra s’insère correctement dans son logement
* Effectuer un montage à blanc pour valider les ajustements

⚠️ **Important :**
Ne pas installer la caméra dès le début du montage — cela peut empêcher le vissage correct des pièces.

---

### 🔩 Étapes de montage

1. Installer la pièce centrale du support
2. Insérer la caméra dans son logement
3. Fixer la caméra avec 1 à 2 vis
4. Positionner correctement l’objectif dans l’emplacement prévu
5. Connecter le câble nappe à la carte Raspberry Pi
6. Vérifier la connexion (test rapide recommandé)
7. Installer la pièce arrière du support :

   * Vérifier le passage correct du câble
8. Finaliser l’assemblage du support

---

## 💻 2. Configuration logicielle

### ⚙️ Préparation de la carte SD

1. Installer une distribution compatible (ex : OctoPi)
2. Configurer :

   * réseau Wi-Fi
   * nom d’hôte (recommandé)

👉 Dépôt recommandé :
[https://github.com/Alienor134/OctoPi_timelapse](https://github.com/Alienor134/OctoPi_timelapse)

---

### 🌐 Accès au flux vidéo

Depuis un navigateur web :

* Via l’adresse IP de la Raspberry Pi

  ```
  http://<IP>
  ```
* Ou via le nom d’hôte :

  ```
  http://<hostname>.local
  ```

📌 En cas de problème :

* Connecter un écran à la Raspberry Pi pour récupérer l’IP
* Vérifier la connexion réseau

---

## 🌿 3. Application : Détection de lentilles d’eau

Les images capturées peuvent être utilisées pour :

* Segmentation d’image (OpenCV, TensorFlow, etc.)
* Détection de zones couvertes par les lentilles
* Suivi de l’évolution dans le temps
* Analyse écologique ou agronomique

### 📊 Pipeline typique

1. Capture d’image
2. Prétraitement (filtrage, correction couleur)
3. Segmentation (seuils, ML, deep learning)
4. Extraction de caractéristiques
5. Visualisation / stockage

---

## ⚠️ Bonnes pratiques

* Fixer solidement la caméra pour éviter les vibrations
* Assurer un éclairage stable (important pour la détection)
* Utiliser un nom d’hôte fixe pour éviter les changements d’IP
* Tester régulièrement le flux vidéo
* Sauvegarder les images capturées

---

## 🚀 Améliorations possibles

* Ajout d’un modèle de détection automatique (IA)
* Capture périodique (timelapse)
* Interface web de visualisation

---

## 📎 Ressources

* Jubilee : [https://github.com/leosabatie-eng/science-jubilee](https://github.com/leosabatie-eng/science-jubilee)
* OctoPi : [https://octoprint.org/download/](https://octoprint.org/download/)
* Dépôt utilisé : [https://github.com/Alienor134/OctoPi_timelapse](https://github.com/Alienor134/OctoPi_timelapse)
* Documentation Raspberry Pi Camera : [https://www.raspberrypi.com/documentation/](https://www.raspberrypi.com/documentation/)

---
