# Rapport LaTeX — Système Intelligent de Contrôle Qualité des Impellers

Rapport académique de fin de module (BDIA1, 2025–2026) généré à partir
de la présentation **« Système Intelligent de Contrôle Qualité des Impellers »**.

Le rapport est rédigé dans un style académique de niveau projet de fin de module,
avec **résumé bilingue (FR/EN)**, **liste des figures et tableaux**, **liste des
acronymes**, **bibliographie** (24 références) et chaque figure systématiquement
introduite et commentée.

## Contenu

```
report/
├── main.tex          # Source LaTeX du rapport (français, ~108 KB)
├── main.pdf          # PDF compilé (64 pages, ~14 MB)
├── images/           # 60 images extraites de la présentation .pptx
└── README.md
```

## Structure du rapport (64 pages)

**Front-matter :**
- Page de garde
- Remerciements
- Résumé (français)
- Abstract (anglais)
- Table des matières
- Liste des figures
- Liste des tableaux
- Liste des acronymes

**Chapitres :**
1. **Introduction générale** — contexte, problématique, objectifs, méthodologie, organisation
2. **État de l'art** — vision artificielle, architectures CNN marquantes, EfficientNet, Transfer Learning, travaux relatifs
3. **Procédé de fabrication et typologie des défauts** — fonderie en moule carapace, défauts observés
4. **Acquisition et organisation des données** — dataset *Casting Defect Detection* (Kaggle)
5. **Prétraitement des images** — pipelines TensorFlow et PyTorch détaillés
6. **Modélisation et expérimentations** — MLP / CNN / Transfer Learning (EfficientNetB0)
7. **Évaluation finale et discussion** — métriques industrielles, ROC/PR, analyse d'erreurs, comparaison
8. **Conclusion générale et perspectives**

**Bibliographie :** 24 références (LeCun, Krizhevsky, He, Tan & Le, Ioffe, Srivastava, Kingma, Pan & Yang, etc.)

## Compilation

### Option 1 — Overleaf (recommandé)

1. Créer un nouveau projet sur [Overleaf](https://www.overleaf.com).
2. Téléverser `main.tex` et le dossier `images/`.
3. Définir `main.tex` comme document principal.
4. Compilateur : **pdfLaTeX**.
5. Compiler une fois → puis **lancer makeglossaries** (Menu → Glossaries) → recompiler 2 fois pour les références croisées.

### Option 2 — Local (TeX Live ou MiKTeX)

```bash
pdflatex main.tex
makeglossaries main         # Pour générer la liste des acronymes
pdflatex main.tex           # 2e passe
pdflatex main.tex           # 3e passe pour les références croisées
```

## Packages LaTeX requis

Tous standards et disponibles sur Overleaf :

`inputenc`, `fontenc`, `babel` (french), `lmodern`, `microtype`, `geometry`,
`setspace`, `parskip`, `fancyhdr`, `titlesec`, `enumitem`, `epigraph`, `graphicx`,
`float`, `caption`, `subcaption`, `array`, `booktabs`, `longtable`,
`tabularx`, `multirow`, `makecell`, `xcolor` (dvipsnames), `tcolorbox`, `listings`,
`amsmath`, `amssymb`, `amsfonts`, `glossaries`, `hyperref`.

## Auteurs

- Ayoub El-Moujahid
- Mohamed Errahmouni
- Soulama Doubié Judicael Noé
- Hazem Douzi

**Encadré par :** Prof. Dr Naoual Attaoui

**Filière :** BDIA1 — Année universitaire 2025–2026
