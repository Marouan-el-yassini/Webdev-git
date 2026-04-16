# Portfolio Web — Navbar & Footer

Un composant HTML/CSS pour afficher une barre de navigation sticky et un footer cohérent.

---

## Aperçu

| Section      | Description                                              |
| ------------ | -------------------------------------------------------- |
| **Navbar**   | Barre de navigation sticky avec liens et bouton CV       |
| **Footer**   | Pied de page centré assorti visuellement à la navbar     |

---

## HTML — Structure

### Navbar

```html
<header class="navbar">
  <div class="nav-inner">
    <span class="nav-logo">Linus<span>.</span></span>
    <nav>
      <a href="#home">Accueil</a>
      <a href="#skills">Compétences</a>
      <a href="#projects">Projets</a>
      <a href="#contact">Contact</a>
    </nav>
    <a href="cv/linus_torvalds_cv.pdf" download class="btn-cv">Télécharger CV</a>
  </div>
</header>
```

### Footer

```html
<footer class="footer">
  <p>© 2026 Linus Torvalds — EMSI</p>
</footer>
```

---

## CSS — Fonctions clés

| Propriété                        | Sélecteur     | Rôle                                        |
| -------------------------------- | ------------- | ------------------------------------------- |
| `position: sticky; top: 0`       | `.navbar`     | Navbar reste visible au scroll              |
| `z-index: 100`                   | `.navbar`     | Passe au-dessus du contenu                  |
| `display: flex`                  | `.nav-inner`  | Aligne logo, liens et bouton horizontalement|
| `justify-content: space-between` | `.nav-inner`  | Répartit les éléments sur toute la largeur  |
| `width: 90%; margin: auto`       | `.nav-inner`  | Centrage responsive                         |
| `transition: 0.2s`               | `.navbar nav a` / `.btn-cv` | Effets hover fluides          |
| `backdrop-filter: blur(6px)`     | `.navbar`     | Flou subtil sur le fond au scroll           |

---

## Compétences techniques mobilisées

| Concept          | Application concrète                        |
| ---------------- | ------------------------------------------- |
| `position: sticky` | Navbar fixée en haut sans JavaScript      |
| Flexbox          | Disposition horizontale des éléments nav    |
| CSS transitions  | Hover fluide sur les liens et bouton CV     |
| Variables CSS    | Couleur principale centralisée en `:root`   |
| Sémantique HTML  | Utilisation de `<header>` et `<footer>`     |

---

## Personnalisation

Pour ajouter un lien dans la navbar :

```html
<a href="#section">Nom section</a>
```

Pour changer la couleur principale :

```css
.navbar { background: #VOTRE_COULEUR; }
.footer { background: #VOTRE_COULEUR; }
```

---

## Auteur

Réalisé par **Bahraoui Abderrahim** dans le cadre d'un projet de portfolio collaboratif.
