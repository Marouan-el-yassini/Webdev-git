# 🧑‍💻 Section Hero — Portfolio Personnel

Composant **Hero** statique réalisé en **HTML5** et **CSS3** pur, destiné à la page d'accueil d'un portfolio de développeur.

---

## 📋 Description

La section Hero est la première chose visible sur la page. Elle présente :

- Une **photo de profil** circulaire
- Un **label de rôle** discret (ex. _software engineer_)
- Un **titre de bienvenue** avec le nom mis en valeur
- Une **courte biographie**
- Deux **boutons de liens** vers LinkedIn et GitHub

---

## 📁 Structure des fichiers

```
projet/
├── index.html        # Contient la section hero
├── style.css         # Styles du composant
└── img/
    └── images.jpeg   # Photo de profil
```

---

## 🧱 Structure HTML

```html
<section class="hero" id="home">
  <div class="hero-photo">
    <img src="img/images.jpeg" alt="Photo de profil" />
  </div>
  <div class="hero-text">
    <p class="hero-tag">software engineer</p>
    <h1>Bonjour, je suis <span>Linus Torvalds</span></h1>
    <p class="hero-desc">...</p>
    <div class="hero-links">
      <a href="..." class="btn-primary">LinkedIn</a>
      <a href="..." class="btn-outline">GitHub</a>
    </div>
  </div>
</section>
```

### Description des éléments

| Élément     | Classe / ID     | Rôle                                      |
| ----------- | --------------- | ----------------------------------------- |
| `<section>` | `.hero` `#home` | Conteneur principal de la section         |
| `<div>`     | `.hero-photo`   | Bloc de la photo de profil                |
| `<img>`     | —               | Photo de profil (115px, circulaire)       |
| `<div>`     | `.hero-text`    | Bloc contenant tous les textes            |
| `<p>`       | `.hero-tag`     | Label gris du rôle/métier                 |
| `<h1>`      | —               | Titre principal avec `<span>` pour le nom |
| `<p>`       | `.hero-desc`    | Paragraphe de biographie                  |
| `<div>`     | `.hero-links`   | Conteneur des boutons                     |
| `<a>`       | `.btn-primary`  | Bouton plein — LinkedIn                   |
| `<a>`       | `.btn-outline`  | Bouton contour — GitHub                   |

---

## 🎨 Référence CSS

### `.hero` — Conteneur principal

```css
.hero {
  text-align: center;
  padding: 60px 20px;
  background: linear-gradient(to bottom, #ffffff, #eef1f4);
}
```

> Centre le contenu et applique un dégradé vertical blanc → gris clair.

---

### `.hero img` — Photo de profil

```css
.hero img {
  width: 115px;
  border-radius: 50%;
  margin-bottom: 15px;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
}
```

> Rend la photo circulaire (115px) avec une légère ombre portée.

---

### `.hero-tag` — Label du rôle

```css
.hero-tag {
  font-size: 13px;
  color: #888;
}
```

> Petit texte gris affiché au-dessus du titre.

---

### `.hero-desc` — Biographie

```css
.hero-desc {
  max-width: 500px;
  margin: 10px auto;
  color: #555;
  line-height: 1.5;
}
```

> Paragraphe centré, limité à 500px, avec un interligne agréable à lire.

---

### `.hero-links a` — Base des boutons

```css
.hero-links a {
  margin: 5px;
  padding: 9px 16px;
  border-radius: 6px;
  font-size: 14px;
  transition: 0.2s;
}
```

> Styles communs aux deux boutons : espacement, coins arrondis, transition fluide.

---

### `.btn-primary` — Bouton LinkedIn

```css
.btn-primary {
  background: #38761d;
  color: white;
}

.btn-primary:hover {
  background: #1d4ed8;
}
```

> Fond vert plein. Passe au **bleu** au survol.

---

### `.btn-outline` — Bouton GitHub

```css
.btn-outline {
  border: 1px solid #38761d;
  color: #38761d;
}

.btn-outline:hover {
  background: #38761d;
  color: white;
}
```

> Bouton fantôme avec bordure verte. Se remplit en vert au survol.

---

## 🎨 Palette de couleurs

| Rôle                   | Couleur         | Code hex  |
| ---------------------- | --------------- | --------- |
| Couleur principale     | Vert forêt      | `#38761d` |
| Survol bouton primaire | Bleu            | `#1d4ed8` |
| Texte biographie       | Gris moyen      | `#555`    |
| Label rôle             | Gris clair      | `#888`    |
| Fond dégradé départ    | Blanc           | `#ffffff` |
| Fond dégradé fin       | Gris très clair | `#eef1f4` |

---

## 🚀 Utilisation

1. Copiez le bloc `<section class="hero">` dans votre `index.html`.
2. Liez la feuille de styles dans le `<head>` :
   ```html
   <link rel="stylesheet" href="style.css" />
   ```
3. Remplacez `img/images.jpeg` par votre propre photo.
4. Mettez à jour le **nom**, le **rôle**, la **description** et les **liens** des boutons.

---

## ✏️ Personnalisation

| Ce que vous voulez changer | Où modifier                                  |
| -------------------------- | -------------------------------------------- |
| Couleur principale         | Remplacer `#38761d` dans tout le CSS         |
| Couleur de survol          | Modifier `#1d4ed8` dans `.btn-primary:hover` |
| Taille de la photo         | Changer `width` dans `.hero img`             |
| Fond de la section         | Modifier le `linear-gradient` dans `.hero`   |
| Largeur de la biographie   | Ajuster `max-width` dans `.hero-desc`        |

---

## 🔗 Liens du composant

- **LinkedIn** : [linkedin.com/in/linustorvalds](https://www.linkedin.com/in/linustorvalds/)
- **GitHub** : [github.com/torvalds](https://github.com/torvalds)

---

## 📦 Dépendances

Aucune — le composant utilise uniquement du **HTML5** et **CSS3** natif, sans framework ni bibliothèque externe.
