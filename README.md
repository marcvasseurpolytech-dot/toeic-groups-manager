# TOEIC Groups Manager v2.0 — Polytech Lille

Application web de gestion des groupes de niveau TOEIC pour Polytech Lille.

## Fonctionnalités

- **Import étudiants** — coller CSV ou importer un fichier (NOM;PRÉNOM;DEPT;SCORE)
- **15 groupes automatiques** — règle mouvante CECRL, distribution 4+4+4+3
- **Attribution des profs** — niveaux Gr1–Gr4, créneaux Lundi/Jeudi, Booster
- **Export Lundi / Jeudi** — 4 créneaux × 4 groupes avec prof et CECRL
- **Suivi profs** — tableau multi-années des niveaux enseignés
- **Listings TOEIC S7** — répartition par amphi (Appert 70 / Chappe 50 / Lebon 50)
- **PDF** — impression via Ctrl+P / Fichier > Imprimer

## Déploiement Vercel

1. Pusher ce repo sur GitHub
2. Importer sur [vercel.com](https://vercel.com)
3. Framework : **Other** (app statique)
4. Deploy

## Utilisation locale

Ouvrir `index.html` dans un navigateur — aucune installation requise.

## Structure

```
index.html    ← app complète (HTML + CSS + JS)
vercel.json   ← config Vercel
README.md
```

## Format CSV

```
NOM;PRÉNOM;DÉPARTEMENT;SCORE
DUPONT;Lucas;GBA;615
MARTIN;Chloé;MAT;780
```

Séparateurs acceptés : `;` `,` ou tabulation. Ligne d'en-tête ignorée automatiquement.
