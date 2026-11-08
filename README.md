# Semainier du prof

Emploi du temps en semaines A et B, journal de chaque cours relié à la séquence de référence, et tâches (sorties, conseils de classe, administratif). Conçu pour iPad et téléphone.

## Mettre en ligne avec GitHub Pages

1. Créez un dépôt sur GitHub (par exemple `semainier-prof`).
2. Déposez tout le contenu de ce dossier à la racine du dépôt : *Add file → Upload files*.
3. Dans *Settings → Pages*, choisissez *Deploy from a branch*, branche `main`, dossier `/ (root)`, puis *Save*.
4. Après une ou deux minutes, l'appli est en ligne à l'adresse `https://<votre-identifiant>.github.io/semainier-prof/`.

## Installer sur l'iPad

1. Ouvrez l'adresse dans **Safari**.
2. Touchez le bouton Partager, puis **Sur l'écran d'accueil**.
3. L'appli s'ouvre alors en plein écran et fonctionne sans connexion.

## Où sont les données

Les données restent dans l'iPad, dans le stockage de l'appli. Rien n'est envoyé sur GitHub.

- Chaque appareil a ses propres données : l'iPad et le téléphone ne se synchronisent pas.
- Effacer les données de Safari efface aussi le semainier.
- Utilisez régulièrement **Réglages → Télécharger la sauvegarde** (fichier `.json`, à garder dans Fichiers ou iCloud Drive). **Restaurer un fichier** recharge une sauvegarde, par exemple pour passer de l'iPad au téléphone.

## Importer une séquence

L'IA n'est pas intégrée à cette version. Dans l'onglet *Séquences → Importer une fiche* :

1. copiez la consigne ;
2. collez-la dans Claude en joignant votre fiche de séquence ou de pilotage ;
3. collez la réponse de Claude dans l'appli, vérifiez les étapes et enregistrez.

## Fichiers

- `index.html` : l'application complète
- `manifest.webmanifest`, `icons/` : installation sur l'écran d'accueil
- `sw.js` : fonctionnement hors ligne

Après une modification de `index.html`, changez `semainier-v1` en `semainier-v2` dans `sw.js` pour que les appareils récupèrent la nouvelle version.
