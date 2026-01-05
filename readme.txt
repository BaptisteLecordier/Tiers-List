# Tier List Builder

Application web permettant de créer facilement des tier lists personnalisées avec drag & drop, couleurs de rangs, import CSV et export en PNG.

---

## ✨ Fonctionnalités

- 🧱 **Gestion des tiers**
  - Ajout / suppression de lignes
  - Réorganisation des tiers avec des flèches (haut / bas)
  - Renommage en cliquant directement sur le nom
  - Choix d’une couleur parmi des **préréglages** (y compris un fond spécial “sparkle”)
  - Ligne spéciale **S** avec fond dégradé

- 🖼️ **Gestion des images**
  - Banc d’images non triées
  - Ajout d’images via bouton _“Ajouter des images”_
  - Ajout d’images par **drag & drop** depuis le disque
  - Drag & drop des images :
    - du banc vers un tier
    - entre tiers
    - réorganisation à l’intérieur d’un tier
  - Clone visuel de l’image sous le curseur pendant le drag
  - **Corbeille** dédiée pour supprimer des images

- 🧩 **Interface**
  - Vignettes carrées avec hover (agrandissement léger + ombre portée)
  - Même hauteur pour les tiers et le banc, pas de “sauts” de layout
  - Popups (modales) pour modifier un tier / réinitialiser, avec fond flouté
  - Boutons homogènes (fond gris, texte/pictos blancs)

- 📝 **Titre & sous-titre**
  - Champs éditables en haut de la tier list
  - Affichés comme placeholders :
    - “Titre de la tier list”
    - “Sous-titre”
  - S’ils ne sont pas remplis, ils **n’apparaissent pas dans l’export PNG**
  - Le fichier PNG exporté prend comme nom le titre (slugifié), sinon `tier-list.png`

- 📥 **Import CSV des tiers**
  - Permet de recréer toute la structure de tiers (nom, couleur, style)

- 📤 **Export en PNG**
  - Export de la tier list dans une image PNG
  - Résolution fixe et indépendante de la taille de l’écran
  - La colonne des flèches / roue de réglage n’apparaît pas dans l’export

- ♻️ **Réinitialisation**
  - Bouton “Réinitialiser la tier list”
  - Popup de confirmation
  - Remet les tiers par défaut (S, A, B, C, D) et renvoie toutes les images dans le banc

---

## 🗂 Structure du projet

Selon ton intégration, le projet peut ressembler à :

```text
.
├── index.html
├── assets
│   ├── css
│   │   └── style.css       (si tu sépares le CSS)
│   └── img
│       └── trash.png       (icône de corbeille)
└── README.md
