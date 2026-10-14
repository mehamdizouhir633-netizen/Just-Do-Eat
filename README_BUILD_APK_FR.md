# Just Do Eat — APK Android

Application de démonstration mobile-first pour l’OFPPT Ifrane. Elle utilise une WebView Android et stocke les commandes localement sur l’appareil avec localStorage.

## Générer et télécharger l’APK avec GitHub Actions

1. Ouvrez l’onglet Actions du dépôt GitHub.
2. Sélectionnez « Build Just Do Eat APK ».
3. Ouvrez l’exécution la plus récente et vérifiez que le job est vert.
4. Dans Artifacts, téléchargez « JustDoEat-debug-APK ».
5. Décompressez le fichier ZIP téléchargé : il contient app-debug.apk.

Le workflow se lance à chaque push sur main/master et peut aussi être exécuté manuellement avec Run workflow.

## Connexion Admin de démonstration

- Adresse : utilisez une adresse Gmail réelle ; elle est enregistrée localement.
- Code de démonstration : admin123.

Ce prototype n’est pas sécurisé pour une mise en production. Les données restent sur l’appareil et ne se synchronisent pas entre téléphones. Le bouton Gmail ouvre un brouillon que l’utilisateur doit envoyer lui-même.

## Build local (facultatif)

Prérequis : JDK 17, Android SDK et Gradle 8.9. À la racine du dépôt, exécutez :

    gradle --no-daemon clean assembleDebug

APK attendu : app/build/outputs/apk/debug/app-debug.apk
