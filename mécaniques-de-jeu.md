# Mécaniques de jeu

## Vue d'Ensemble

Hybride entre wave defense et typing game — architecture similaire à Z-Type, mais avec substitution de l'input textuel par une interface musicale. Des vagues d'ennemis convergent vers le joueur ; chacun doit être éliminé avant impact en jouant l'intervalle ou accord (ou séquence de) qu'il porte.

Le jeu n'est pas un jeu de rythme. La pression temporelle existe — proximité des ennemis — mais l'inexactitude rythmique n'est pas sanctionnée. Le focus est entièrement harmonique.

## Boucle de gameplay

```
Ennemi porteur d'un symbole d'intervalle approche
  → reconnaissance visuelle du symbole (stimulus visuel)
    → reproduction du pattern spatial sur l'interface instrument (réponse motrice)
      → élimination de l'ennemi
        → Répétition 
          →	Association auditive émergente (sous-produit)
```
Boucle = visuel → spatial → moteur → auditif

Aucune capacité d'écoute préalable requise. Aucune théorie musicale prérequise. L'oreille se développe par exposition répétée — conditionnement pavlovien : même geste, même son, association progressive.

## Isomorphisme

Le jeu propose prioritairement des GUI d'instruments isomorphiques.
Sur un instrument isomorphique, tout intervalle correspond à une forme spatiale unique, invariante quelle que soit la note de départ.

Implémentations :
- **Guitare** — accordage régulier en quartes (et autres accordages réguliers: quintes, tierces majeures, mineures)
- **Piano** — clavier symétrique 6/6 (6 touches noires, 6 touches blanches, répartition intervallique constante)

La conséquence pédagogique: Sur un substrat irrégulier, un même intervalle se présente sous des formes multiples. Ici : une seule. Pas de transformation nécessaire. L'invariance spatiale supprime une couche de traduction dans la chaîne perception → geste. L'interface est transparente.

## Inputs

**Interface GUI à l'écran** — mode principal

- PC (clavier/souris) ou tablette (tactile/stylet)
- Aucun hardware spécifique requis

**Contrôleur MIDI externe** — mode optionnel, accès délibéré

- Difficulté significativement plus élevée : les claviers MIDI standards ne sont pas isomorphiques
- 12 cartes d'intervalles distinctes à intérioriser au lieu d'une seule
- Réservé aux joueurs qui font ce choix en connaissance de cause

Le joueur ayant essayé les deux modes devrait percevoir dans le corps la supériorité du layout isomorphique pour l'apprentissage de l'harmonie relative.

## Symboles

- **Défaut** — représentation géométrique abstraite, propre au jeu. 
- **Option** — notation intervallique standard (b3, 5, etc.) pour transfert vers le vocabulaire musical conventionnel.

## Progression

Les intervalles sont introduits un à un ; le pool actif s'élargit par paliers. 
Les collections sont sélectionnées intentionnellement — gammes, modes, arpèges, et arrangées suivant une logique de curriculum.

Deux modes de jeu principaux :

- **Mode vertical** — intervalle mesuré par rapport à une note de référence fixe (harmonique)
- **Mode horizontal** — intervalle mesuré par rapport à la dernière note jouée (mélodique)

La difficulté est fonction de trois variables : diversité des intervalles du niveau, fréquence et densité des vagues, et vitesse des ennemis.
Certains ennemis portent des séquences d'intervalles plutôt qu'un intervalle isolé — résistance accrue, élimination conditionnée à l'exécution sans accroc d'une chaîne complète.
Horizon de progression : polyphonie — accords, inversions.

# Hors scope

Un sommet de la maîtrise de l'harmonie relative serait la compréhension des progressions d'accords comme suites de vecteurs — chacun orienté d'un accord vers un autre, porteur d'une couleur émotionnelle propre, recombinables selon l'intention compositionnelle. Cette logique, avec sa nomenclature, est enseignée par le compositeur Jjay Berthume sous le nom _Chord Relationships_.

Ce volet est délibérément omis. Le risque de perdre le joueur avant d'atteindre ce niveau de maîtrise est jugé trop élevé pour en justifier l'inclusion.