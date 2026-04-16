# Site Portfolio Moderne

Un site portfolio responsive et collaboratif développé en **HTML5** et **CSS3** par trois développeurs travaillant ensemble via Git.

---

## Table des matières

- [Présentation du projet](#présentation-du-projet)
- [Membres de l'équipe](#membres-de-léquipe)
- [Fonctionnalités](#fonctionnalités)
- [Technologies utilisées](#technologies-utilisées)
- [Structure du projet](#structure-du-projet)
- [Installation et utilisation](#installation-et-utilisation)
- [Workflow collaboratif](#workflow-collaboratif)
- [Comment contribuer](#comment-contribuer)
- [Contact](#contact)

---

## Présentation du projet

Ce projet est un site portfolio moderne et entièrement responsive, conçu et développé en collaboration par **Marouan**, **Yassir** et **Abderrahim**. Il présente un portfolio professionnel avec des sections dédiées à la navigation, l'introduction, les compétences techniques, les projets réalisés et les informations de contact.

Développé en **HTML5** et **CSS3** purs (sans JavaScript), ce projet illustre de bonnes pratiques de code, un design responsive et une collaboration efficace via Git.

**Objectifs :**
- Créer un site portfolio professionnel
- Mettre en valeur les compétences et projets réalisés
- Pratiquer le design web responsive
- Démontrer l'utilisation de Git en équipe
- Produire un code propre et maintenable

---

## Membres de l'équipe

### Abderrahim Bahraoui — [@Abduu898](https://github.com/Abduu898)
**Responsabilité :** Barre de navigation & Footer
- Conception et développement de la barre de navigation responsive
- Création du footer avec copyright et liens
- Accessibilité de la navigation et défilement fluide

### Yassir — [@futkiller](https://github.com/futkiller)
**Responsabilité :** Section Hero
- Conception de la section d'accueil et de la présentation du profil
- Implémentation des boutons d'action (LinkedIn & GitHub)
- Intégration de la photo de profil et du texte d'introduction

### Marouan El Yassini — [@Marouan-el-yassini](https://github.com/Marouan-el-yassini)
**Responsabilité :** Sections Compétences & Projets
- Conception et développement de la section compétences avec barres de progression
- Création du tableau de présentation des projets
- Organisation des descriptions et des technologies utilisées

---

## Fonctionnalités

### Barre de navigation
- En-tête fixe avec liens de défilement fluide
- Bouton de téléchargement du CV
- Logo "Linus."
- Entièrement responsive

### Section Hero
- Photo de profil professionnelle
- Texte d'introduction avec statut étudiant (EMSI 2ème année)
- Boutons d'action vers LinkedIn et GitHub

### Section Compétences
- Barres de progression avec niveau en pourcentage
- Disposition en grille à 2 colonnes

| Compétence | Niveau |
|---|---|
| C | 95% |
| Python | 89% |
| C++ | 100% |
| Git / GitHub | 100% |
| Assembly | 99% |
| Architecture OS | 90% |

### Section Projets

| Projet | Description | Technologies |
|---|---|---|
| Maintenance du noyau Linux | Maintenance et correctifs du noyau | C, Assembly |
| Système Git | Implémentation d'un VCS distribué | C, Bash |
| Linux Kernel 0.01 | Build minimal du noyau original | C, Assembly |

### Section Contact
- Formulaire de contact avec champs nom, email et message

---

## Technologies utilisées

| Catégorie | Outils |
|---|---|
| Frontend | HTML5, CSS3 (Flexbox, Grid) |
| Contrôle de version | Git, GitHub |
| Polices | Google Fonts — Sora & Inter |
| Éditeurs | VS Code / tout IDE |

---

## Structure du projet

```
Webdev-git/
├── index.html                  # Page principale du portfolio
├── style.css                   # Styles et design responsive
├── README.md                   # Ce fichier
├── img/
│   └── images.jpeg             # Photo de profil
└── cv/
    └── linus_torvalds_cv.pdf   # CV téléchargeable
```

**`index.html`** — Organisé en sections sémantiques :
- `<header>` — Barre de navigation
- `<section class="hero">` — Section d'accueil
- `<section id="skills">` — Compétences
- `<section id="projects">` — Projets
- `<section id="contact">` — Formulaire de contact
- `<footer>` — Pied de page

**`style.css`** — Design responsive avec media queries, CSS Grid & Flexbox, variables personnalisées, approche mobile-first.

---

## Installation et utilisation

### Prérequis
- Un navigateur moderne (Chrome, Firefox, Safari, Edge)
- Git (pour le clonage)

### Étapes

```bash
# 1. Cloner le dépôt
git clone https://github.com/Marouan-el-yassini/Webdev-git.git

# 2. Accéder au dossier du projet
cd Webdev-git

# 3. Ouvrir dans le navigateur
# Double-cliquer sur index.html ou l'ouvrir via le menu Fichier du navigateur
```

Aucun outil de build, aucun npm, aucune compilation nécessaire. Il suffit d'ouvrir `index.html`.

---

## Workflow collaboratif

Chaque membre a travaillé sur une branche dédiée :

| Développeur | Branche |
|---|---|
| Abderrahim | `feature/navbar-footer` |
| Yassir | `feature/hero-section` |
| Marouan | `feature/competencies-projects` |

### Commandes Git utilisées

```bash
# Cloner le dépôt
git clone https://github.com/Marouan-el-yassini/Webdev-git.git

# Créer une branche de fonctionnalité
git checkout -b feature/ma-section

# Indexer et valider les modifications
git add .
git commit -m "Ajout du style de la barre de navigation"

# Pousser vers le dépôt distant
git push origin feature/ma-section

# Récupérer les dernières modifications depuis main
git pull origin main

# Fusionner dans main
git merge feature/ma-section
```

---

## Comment contribuer

1. Créer une branche : `git checkout -b feature/ma-fonctionnalite`
2. Effectuer et tester les modifications en local
3. Valider : `git commit -m "Description claire des changements"`
4. Pousser : `git push origin feature/ma-fonctionnalite`
5. Ouvrir une Pull Request sur GitHub et demander une revue

**Conventions de code :**
- Utiliser les balises sémantiques HTML5
- Respecter des conventions de nommage CSS cohérentes
- Commenter les sections complexes
- Tester le responsive sur plusieurs tailles d'écran

---

## Compatibilité navigateurs

Testé et fonctionnel sur Chrome, Firefox, Safari, Edge et navigateurs mobiles (Safari iOS, Chrome Mobile).

---

## Statistiques du projet

| Indicateur | Valeur |
|---|---|
| Membres de l'équipe | 3 développeurs |
| Nombre de commits | 20+ |
| Durée de développement | ~1 semaine |
| Lignes de code | ~500 HTML / ~800 CSS |
| Date de finalisation | Avril 2026 |

---

## Contact

| Nom | GitHub | 
|---|---|
| Abderrahim Bahraoui | [@Abduu898](https://github.com/Abduu898) |
| Yassir | [@futkiller](https://github.com/futkiller) | 
| Marouan El Yassini | [@Marouan-el-yassini](https://github.com/Marouan-el-yassini) | 

---

## Licence

Projet réalisé à des fins pédagogiques dans le cadre du cursus de l'**EMSI** (École Marocaine des Sciences de l'Informatique).

---

*Réalisé par Marouan, Yassir et Abderrahim — workflow collaboratif Git.*
