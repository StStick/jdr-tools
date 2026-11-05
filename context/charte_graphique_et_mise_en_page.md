# Charte Graphique & Règles de Mise en Page — Yeast Eaters

Guide de référence pour la rédaction et la standardisation visuelle des scénarios et documents de la campagne *Yeast Eaters*.

---

## 1. Structure Générale & Paramètres Document (DOCX)

* **Marges de page :** 2 cm (ou 0,8 à 1,0 pouce) sur tous les côtés.
* **Typographie du corps de texte :** 
  * Police : `Calibri`
  * Taille : 10,5 pt à 11 pt
  * Couleur : Gris sombre anthracite (`#222222`)
  * Interligne : 1,15
* **Typographie des titres & en-têtes :**
  * Police : `Arial` (gras)
  * Couleur : Bleu nuit sombre / ardoise (`#111827` ou `#1E293B`)
* **Format des dates in-game :**
  * Exemple : *15 février 2313*
  * Police : `Calibri`, 12-13 pt, italique, couleur sarcelle / cyan foncé (`#008080`).

---

## 2. Système d'Encadrés Thématiques (Cartes & Callouts)

Tous les scénarios officiels utilisent un système de conteneurs (tableaux 1x1) à **fond teinté** et **bordure gauche épaisse** (largeur env. 36 dxa / 4.5 pt), sans bordures supérieure, droite ou inférieure.

| Type de Carte | Code Balise | Fond / Hex | Bordure Gauche / Hex | Label d'en-tête | Finalité en jeu |
| :--- | :---: | :---: | :---: | :--- | :--- |
| **Description** | `desc` | Bleu ciel (`#EAF2F8`) | Bleu soutenu (`#3A7CA5`) | `📖 DESCRIPTION — À LIRE` | Textes d'ambiance et descriptions immersives à lire aux PJ (texte en italique). |
| **Info MJ** | `mj` | Rouge pâle (`#FCEDEA`) | Rouge carmin (`#C0392B`) | `🎲 INFO MJ — SECRET` | Données confidentielles, secrets de l'intrigue et coulisses réservés au MJ. |
| **Dialogue** | `dial` | Gris clair (`#F2F2F2`) | Gris moyen (`#888888`) | `💬 [NOM DU PNJ]` | Répliques et dialogues en italique encadrés de guillemets français « ». |
| **Scène RP** | `rp` | Vert menthe (`#EEF6EF`) | Vert forêt (`#4A7A5C`) | `🎭 SCÈNE RP — ...` | Interactions ouvertes, dilemmes moraux, scènes de négociation et improvisations. |
| **Événement** | `event` | Mauve clair (`#F4EEFB`) | Violet / Améthyste (`#7E57C2`) | `🎲 ÉVÈNEMENT — JET` | Tests de compétences, Seuils de Difficulté (DD) et embranchements de jets de dés. |
| **Combat** | `combat` | Pêche / Orange pâle (`#FDF0E4`) | Brun orangé (`#B5651D`) | `⚔️ COMBAT` | Profils martiaux, initiatives, seuils de fuite/reddition et gestion des renforts. |
| **Préparation** | `prep` | Turquoise pâle (`#EAFBF6`) | Vert canard (`#16A085`) | `🗒️ EN AMONT DE SÉANCE` | Informations, logistique et choix à valider avec les joueurs avant la séance. |
| **Campagne** | `note` | Jaune pastel (`#FFF9DB`) | Ocre / Doré (`#C99A1E`) | `📌 INFO CAMPAGNE` | Faits majeurs, indices critiques et conséquences à archiver pour la suite. |

---

## 3. Codes Couleur des Dialogues & Typographie des Répliques

Pour identifier rapidement les répliques dans les échanges :

* **Raphaël :** Ambre foncé / Cuivré (`#9C6B2E`)
* **Miranda :** Bleu électrique (`#3D6FA8`)
* **Inspecteur de police :** Brun sombre / Brique (`#6B3F3F`)
* **Autres intervenants :** Gris neutre foncé (`#444444`)

### Format standard des répliques :
* Nom de l'orateur en **gras** avec sa couleur dédiée, suivi de deux points.
* Texte de la réplique entre **guillemets français** et en *italique*.
* *Exemple :* **Miranda :** « *Connexion établie, vous avez trois minutes avant traçage.* »

---

## 4. Gestion des Choix et Éléments Variables (Placeholders)

* Tous les éléments dynamiques, improvisés ou nécessitant un arbitrage du MJ doivent être mis en évidence en **gras italique rouge entre crochets** :
  * Syntaxe : `***[Nom de l'informateur]***` ou `***[Lieu de repli choisi]***`