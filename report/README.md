# Rapport LaTeX — Système Intelligent de Contrôle Qualité des Impellers

Rapport académique généré à partir de la présentation
**« Système Intelligent de Contrôle Qualité des Impellers »** (BDIA1, 2025–2026).

## Contenu

```
report/
├── main.tex          # Source LaTeX du rapport (français)
├── images/           # 60 images extraites de la présentation .pptx
└── README.md
```

Le rapport couvre :

1. **Introduction** — contexte industriel de la fonderie et étapes de fabrication
2. **Problématique et objectif** — détection automatique des défauts (fissures, déformations, bavures)
3. **Solution proposée** — architecture globale du système de contrôle qualité
4. **Données** — dataset *Casting Defect Detection* (Kaggle, R. Dabhi)
5. **Prétraitement** — pipelines TensorFlow et PyTorch (reproductibilité, augmentations, normalisation ImageNet, gestion du déséquilibre)
6. **Modélisation** — comparaison MLP / CNN / Transfer Learning (EfficientNetB0)
7. **Évaluation finale** — métriques, matrice de confusion, courbes ROC et Precision-Recall, analyse des erreurs
8. **Conclusion et perspectives**

## Compilation

### Option 1 — Overleaf (recommandé)

1. Créer un nouveau projet sur [Overleaf](https://www.overleaf.com).
2. Téléverser `main.tex` et le dossier `images/`.
3. Définir `main.tex` comme document principal.
4. Compilateur : **pdfLaTeX**.
5. Compiler — le PDF est généré automatiquement.

### Option 2 — Local (TeX Live ou MiKTeX)

```bash
pdflatex main.tex
pdflatex main.tex   # 2e passe pour la table des matières et les références
```

## Packages LaTeX requis

Tous standards et disponibles sur Overleaf :

`inputenc`, `fontenc`, `babel` (french), `lmodern`, `microtype`, `geometry`,
`setspace`, `parskip`, `fancyhdr`, `titlesec`, `enumitem`, `graphicx`,
`float`, `caption`, `subcaption`, `array`, `booktabs`, `longtable`,
`tabularx`, `multirow`, `xcolor` (dvipsnames), `tcolorbox`, `listings`,
`amsmath`, `amssymb`, `amsfonts`, `hyperref`.

## Auteurs

- Ayoub El-Moujahid
- Mohamed Errahmouni
- Soulama Doubié Judicael Noé
- Hazem Douzi

**Encadré par :** Prof. Dr Naoual Attaoui

**Filière :** BDIA1 — Année universitaire 2025–2026
