# 🌙 moon.c — Mécanique Lunaire de Précision

**Version 3.2.0** | par [MC88](mailto:mohamed005cheikh@gmail.com)

---

## 📖 À propos

`moon.c` est un simulateur lunaire interactif en temps réel conçu pour offrir une visualisation précise et esthétique des mécaniques orbitales de la Lune. Alliant rigueur scientifique (basée sur les algorithmes astronomiques de Jean Meeus) et design immersif, l'application permet d'explorer la phase actuelle, l'illumination, la distance, la vitesse orbitale, ainsi que les heures de lever et coucher de la Lune adaptées à votre position géographique.

Le projet se veut une **encyclopédie lunaire dynamique**, proposant une vingtaine d'articles scientifiques vulgarisés et des thèmes visuels adaptés aux événements astronomiques rares (Supermoon, Blood Moon, Blue Moon, Eclipse).

---

## ✨ Fonctionnalités Principales

- **🕹️ Moteur Lunaire en Direct** :
  - Calcul de la phase actuelle (Nouvelle Lune, Pleine Lune, etc.).
  - Pourcentage d'illumination et âge lunaire (en jours).
  - Distance Terre-Lune (en km) et vitesse orbitale (km/s).
  - Compte à rebours dynamique pour le prochain événement majeur (Premier Quartier, Pleine Lune, etc.).
- **🌍 Géolocalisation** :
  - Détection automatique de votre position (avec permission) pour afficher les heures précises du lever et coucher de la Lune.
  - Option de repli sur Londres (par défaut) si la géolocalisation est refusée.
- **🖼️ Rendu Visuel Avancé** :
  - Canevas (Canvas) haute résolution représentant la Lune avec sa texture, ses mers (maria), ses cratères et son terminateur ombragé.
  - Effet d'aura lumineuse et champ d'étoiles animé en arrière-plan.
- **📅 Calendrier Lunaire** :
  - Affichage mensuel des phases lunaires avec icônes visuelles, permettant de naviguer dans le passé et le futur.
- **📚 Encyclopédie Scientifique** :
  - 20 articles de fond couvrant la géologie, la physique, l'exploration, la géophysique et l'impact culturel de la Lune.
  - Fenêtre de lecture modale pour une consultation confortable.
- **🎨 Thèmes Visuels** :
  - 4 thèmes d'ambiance (Supermoon, Blood Moon, Blue Moon, Eclipse) modifiant les couleurs de l'interface et de l'aura lunaire.
  - Raccourcis clavier (touches `1`, `2`, `3`, `4`).
- **🛡️ Transparence et Éthique** :
  - Un avertissement clair (Disclaimer) est affiché en haut de la section des sources, précisant que le propriétaire du site est un simple **transmetteur** d'informations et n'endosse pas les théories présentées.

---

## 🧰 Technologies Utilisées

- **HTML5** : Structure sémantique et accessibilité (ARIA).
- **CSS3** : Design system sombre et épuré, Glassmorphism, animations fluides et responsive design (mobile-first).
- **JavaScript (Vanilla ES6)** :
  - Algorithmes astronomiques issus de *"Astronomical Algorithms"* de Jean Meeus.
  - Rendu graphique via `<canvas>` pour la Lune et les étoiles.
  - Gestion des événements, du stockage local (thème), et des Web APIs (Geolocation, Clipboard, Service Worker).
- **Google Fonts** : `Cormorant Garamond` (titres) & `Plus Jakarta Sans` (corps de texte).

---

## 📂 Structure du Projet
> **Note** : L'application est conçue comme une **Single Page Application (SPA)**. Tout le CSS et le JavaScript sont intégrés dans le fichier `index.html` pour faciliter le déploiement.

---

## 🚀 Installation et Lancement

Pour exécuter le projet localement :

1.  **Téléchargez** ou **clonez** ce dépôt.
2.  Assurez-vous que les fichiers `index.html`, `widget.html` et `sw.js` sont dans le même dossier.
3.  **Lancez un serveur local** (recommandé pour éviter les problèmes de CORS avec le Service Worker) :
    - Utilisez l'extension *Live Server* de VS Code.
    - Ou utilisez Python : `python -m http.server 8000`.
4.  Ouvrez votre navigateur à l'adresse indiquée (ex: `http://localhost:8000`).

> **Aucune installation de dépendances npm ou de compilation n'est requise.**

---

## 🌐 API et Sources de Données

Les calculs sont effectués en local (côté client) et ne nécessitent pas d'appels API externes. Les références scientifiques utilisées pour la validation sont :

- **Algorithms** : Jean Meeus (*Astronomical Algorithms*, 2nd ed.).
- **Données de validation** : USNO Moon Phase Data, NASA GSFC Lunar Eclipse Tables, NASA JPL Horizons.
- **Image de texture** : Wikimedia Commons (FullMoon2010.jpg – CC BY-SA 3.0, Gregory H. Revera).

---

## 🔑 Raccourcis Clavier

| Touche | Action                     |
| :----- | :------------------------- |
| `1`    | Activer le thème Supermoon |
| `2`    | Activer le thème Blood Moon|
| `3`    | Activer le thème Blue Moon |
| `4`    | Activer le thème Eclipse   |
| `Esc`  | Fermer les modales / Menus |

---

## 📝 Avertissement Légal (Disclaimer)

Ce site est un projet personnel à but éducatif et informatif. **Je ne suis pas l'auteur des articles scientifiques** référencés, je n'en revendique pas la paternité et je ne soutiens pas nécessairement toutes les théories ou affirmations qu'ils contiennent. Je joue le rôle de **conservateur et traducteur** d'informations disponibles sur internet.

Les sources sont systématiquement citées en bas de page. Je vous encourage vivement à effectuer vos propres recherches et à consulter les références primaires pour vérifier les faits par vous-même.

---

## 👤 Auteur

- **Nom** : MC88
- **Contact** : [mohamed005cheikh@gmail.com](mailto:mohamed005cheikh@gmail.com)
- **Projet** : Développement indépendant, version 3.2.0.

---

## 📜 Licence

Ce projet est fourni à titre d'exemple et d'étude. Les droits d'auteur sur les articles et les images utilisés appartiennent à leurs auteurs respectifs (cités dans la section Sources du site web). Le code JavaScript, HTML et CSS (à l'exception des ressources tierces) est la propriété de l'auteur.

---

**Profitez de l'observation !** 🔭✨
