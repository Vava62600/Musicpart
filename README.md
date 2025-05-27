# 🎼 MusicPart

MusicPart est une application Android permettant de gérer et lire des partitions musicales, tablatures et fichiers MIDI, avec support pour la synchronisation entre partition visuelle et audio.

## ✨ Fonctionnalités principales
- Lecture de partitions en image ou PDF
- Lecture de fichiers MIDI avec choix d'instrument
- Génération automatique de tablatures à partir de fichiers MIDI et inversement
- Création automatique de groupes et partitions depuis le dossier local
- Transfert sans fil ou par câble depuis un PC
- Interface intuitive avec thème sombre/clair

## 📱 Plateformes supportées
- Android 7.0+
- Smartphones et tablettes

## 📌 Features

🎵 Gestion des Groupes & Partitions

- Création automatique des groupes/partitions si ajout manuel ou détection dans un dossier défini.

- Support des formats de partition : .jpg, .jpeg, .png, .pdf, .mid, formats tablatures.

- Réinitialisation de l'application avec système de confirmation (double prompt ou saisie d’un mot de passe).

🎧 Lecture MIDI & Tablature

- Si une tablature existe sans fichier MIDI → génération automatique à partir de la tablature.

- Si un fichier MIDI existe sans tablature → génération de la tablature via une bibliothèque dédiée.

- Interface permettant de choisir l'instrument s’il y a plusieurs pistes dans un fichier .mid.

- Contrôles : lecture/pause, synchronisation avec la partition, navigation (avant/arrière).

🌐 Transfert depuis PC

- Support du transfert via câble USB ou réseau local.

- Affichage d’un QR Code pour simplifier la connexion et l’envoi de fichiers.

🎨 Interface

- Thème sombre / clair.

- Splash screen avec logo au démarrage.

- Interface responsive adaptée aux tablettes et smartphones Android (7.0+).

🔧 Technologies & Dépendances

## 📚 Librairies nécessaires :
```txt
  // Kotlin Extensions
  implementation 'androidx.core:core-ktx:1.12.0'

  // Material Design
  implementation 'com.google.android.material:material:1.11.0'

  // JSON Handling
  implementation 'com.google.code.gson:gson:2.10.1'

  // File Chooser / File API
  implementation 'androidx.documentfile:documentfile:1.0.1'

  // MIDI
  implementation 'androidx.media:media:1.6.0'
  implementation 'org.billthefarmer:mididriver:1.30'

  // PDF Reader (pour affichage des partitions PDF)
  implementation 'com.github.barteksc:android-pdf-viewer:3.2.0-beta.1'

  // Image loader
  implementation 'com.github.bumptech.glide:glide:4.16.0'

  // QR Code
  implementation 'com.journeyapps:zxing-android-embedded:4.3.0'
```
