# ⚡ POLARITÉ

Un jeu d'arcade néon, jouable au doigt, **entièrement généré par Claude Code en autonomie** (code, moteur, audio, art des icônes, tests, déploiement).

> Tu es un noyau instable. Change ta **polarité** pour absorber les particules de ta couleur, esquive celles de la couleur opposée. Plus tu enchaînes, plus ça monte.

🎮 **Jouer :** [polarite](https://polarite.vercel.app)

## Comment jouer
- **Déplacer** : glisse le doigt (mobile) ou la souris (desktop)
- **Inverser la polarité** : touche / clic / `Espace`
- **⚡ Surge** : onde de choc qui pulvérise les particules ennemies quand la jauge est pleine (`Shift` au clavier)
- Absorbe ta couleur → score + combo. Touche la mauvaise → tu perds de l'intégrité.

## Sous le capot
Tout tient dans **un seul `index.html`**, sans dépendance, sans framework, sans assets externes :
- Moteur de jeu canvas 2D (rendu additif, glow néon, particules, trails)
- **Audio 100% synthétisé en temps réel** (WebAudio) : drone ambiant, arpégiateur qui s'intensifie avec le combo, SFX procéduraux
- Game feel : screen shake, hitstop, slow-motion, flash d'impact, combos
- PWA installable (manifest + service worker, jouable hors-ligne)
- Responsive mobile + desktop, contrôles tactiles et souris/clavier

## Qualité
Testé en navigateur headless (Playwright) : zéro erreur JS/console, parcours complet vérifié (menu → partie → absorption → surge → game over → rejouer), titres validés jusqu'à 360px de large.

---
*Conçu, codé, testé et déployé par Claude Code.*
