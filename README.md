# Convocations EPS — PWA

Générateur de convocations EPS pour enseignants — fonctionne 100% en local, sans serveur, sans installation.

## Fonctionnalités

- **2 modèles** : UNSS / Compétition (avec coupon parental) et DNB EPS / Examen
- **Import Excel ou CSV** avec détection automatique des colonnes Nom / Prénom / Classe
- **Logos personnalisables** : logo gauche (collège / EN) et logo droit (AS / UNSS) — sauvegardés localement
- **Sauvegarde automatique** des paramètres (localStorage)
- **Impression** : 2 par page A5 ou 1 par page A4
- **Tri** par classe puis par nom
- **PWA** : installable sur tablette et smartphone, fonctionne hors ligne

## Déploiement sur GitHub Pages

1. Créer un repo GitHub (ex: `convocations-eps`)
2. Uploader tous les fichiers à la racine
3. Activer GitHub Pages : Settings → Pages → Source: main branch / root
4. Accéder à `https://[username].github.io/convocations-eps/`

## Fichiers

```
index.html      Application principale
sw.js           Service Worker (offline)
manifest.json   PWA manifest
icon-192.png    Icône PWA
icon-512.png    Icône PWA
```

## Format du fichier élèves

Le fichier Excel/CSV doit contenir au minimum les colonnes :
- **Nom** (ou NOM, nom_famille, etc.)
- **Prénom** (ou PRENOM, prenom, etc.)  
- **Classe** (ou CLASSE, classe, etc.)

Les colonnes sont associées automatiquement mais peuvent être ajustées manuellement.

## Usage

1. Choisir le type (UNSS ou DNB)
2. Importer le fichier élèves
3. Remplir les paramètres (date, lieu, activité…)
4. Ajouter les logos si souhaité
5. Cliquer sur "Imprimer"
