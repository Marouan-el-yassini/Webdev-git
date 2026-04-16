# Portfolio Web — Section Compétences & Projets

Un composant HTML/CSS pour afficher les compétences techniques sous forme de barres de progression dynamiques et les projets dans un tableau structuré.

---

## Aperçu

| Section         | Description                                                        |
| --------------- | ------------------------------------------------------------------ |
| **Compétences** | Grille de barres de progression colorées avec pourcentages         |
| **Projets**     | Tableau récapitulatif des réalisations avec technologies utilisées |

---

## Structure des fichiers

```
portfolio/
├── index.html        # Markup des sections Skills & Projects
└── style.css         # Styles associés
```

---

## HTML — Structure

### Section Compétences

Chaque compétence suit ce modèle :

```html
<div class="skill-item">
  <div class="skill-header">
    <span class="skill-name">C++</span>
    <span class="skill-pct">100%</span>
  </div>
  <div class="skill-bar">
    <div class="skill-fill" style="--fill: 100%"></div>
  </div>
</div>
```

> La valeur `--fill` est une **variable CSS inline** qui contrôle la largeur de la barre sans dupliquer de classes CSS.

### Section Projets

Tableau sémantique `<thead>` / `<tbody>` pour l'accessibilité et le SEO.

---

## CSS — Fonctions clés

| Propriété                        | Sélecteur                    | Rôle                                        |
| -------------------------------- | ---------------------------- | ------------------------------------------- |
| `display: grid`                  | `.skills-grid`               | Disposition en grille responsive            |
| `repeat(2, 1fr)`                 | `.skills-grid`               | 2 colonnes de largeur égale                 |
| `gap: 18px`                      | `.skills-grid`               | Espacement uniforme entre les items         |
| `display: flex`                  | `.skill-header`              | Alignement horizontal nom / %               |
| `justify-content: space-between` | `.skill-header`              | Nom à gauche, % à droite                    |
| `border-radius: 6px`             | `.skill-bar` / `.skill-fill` | Coins arrondis pour un rendu moderne        |
| `width: var(--fill)`             | `.skill-fill`                | Lit la variable CSS pour définir la largeur |
| `border-collapse: collapse`      | `table`                      | Fusionne les bordures des cellules          |
| `overflow: hidden`               | `table`                      | Permet le border-radius sur le tableau      |
| `width: 90%; margin: auto`       | `.container`                 | Centrage responsive                         |

### Variable CSS `--fill` — point clé

```css
/* Dans le CSS */
.skill-fill {
  width: var(--fill); /* lit la variable */
}
```

```html
<!-- Dans le HTML -->
<div class="skill-fill" style="--fill: 89%"></div>
```

Grâce à cette technique, **une seule règle CSS** gère toutes les barres. La valeur est passée directement depuis le HTML, sans JavaScript.

---

## Compétences affichées

| Langage / Outil | Niveau |
| --------------- | ------ |
| C               | 95%    |
| Python          | 89%    |
| C++             | 100%   |
| Git / GitHub    | 100%   |
| Assembly        | 99%    |
| OS Architecture | 90%    |

---

## Projets

| Projet   | Description                                  | Technologies          |
| -------- | -------------------------------------------- | --------------------- |
| Projet 1 | Application mobile de gestion de tâches      | Dart, Flutter         |
| Projet 2 | Site vitrine pour une entreprise locale      | HTML, CSS, JavaScript |
| Projet 3 | Application desktop de finances personnelles | Java, JavaFX          |

---

## Personnalisation

Pour ajouter une compétence, copier-coller ce bloc dans `.skills-grid` :

```html
<div class="skill-item">
  <div class="skill-header">
    <span class="skill-name">Nom</span>
    <span class="skill-pct">XX%</span>
  </div>
  <div class="skill-bar">
    <div class="skill-fill" style="--fill: XX%"></div>
  </div>
</div>
```

Pour changer la couleur principale, modifier la valeur `#38761d` dans le CSS :

```css
/* Couleur principale (vert) */
.skill-fill {
  background: #38761d;
}
th {
  background: #38761d;
}
```

---

## Auteur

Réalisé par **Maroun** dans le cadre d'un projet de portfolio collaboratif.
