---
name: scenario-reviewer
description: "Relire un scénario JDR : corriger uniquement l’orthographe et la grammaire, évaluer ses forces, faiblesses et incohérences avec le contexte ou les personnages, ou estimer la durée d’une séance scène par scène."
argument-hint: "[correction | revue | durée | tout] fichier du scénario"
user-invocable: true
---

# Relecture de scénarios JDR

Utilise ce skill pour un ou plusieurs de ces modes : correction, revue de fond
et estimation de durée. Le scénario peut être donné en pièce jointe, par chemin,
ou être le fichier actif.

## Choisir le mode

- **Correction** : corriger directement le fichier fourni, sans demander de
  validation. Ne modifier que l’orthographe, la grammaire, les accords, la
  conjugaison et la ponctuation manifestement fautive. Ne pas reformuler,
  réorganiser, enrichir, supprimer ou modifier le ton, les intentions, les
  mécaniques et les faits. Préserver la structure Markdown et les métadonnées.
  Signaler séparément toute phrase ambiguë qu’une correction stricte ne permet
  pas de réparer sans reformulation.
- **Revue** : ne pas modifier le scénario. Évaluer sa jouabilité, sa structure,
  son rythme, ses choix laissés aux joueurs, ses indices, ses mécaniques et ses
  issues. Examiner sa cohérence avec le contexte et les personnages disponibles
  dans le dépôt. Distinguer une contradiction établie d’une question à clarifier
  ou d’une possibilité d’amélioration.
- **Durée** : ne pas modifier le scénario. Estimer la durée pour un groupe qui
  aime les discussions et le jeu de rôle, en détaillant approximativement chaque
  scène et en indiquant les hypothèses, embranchements et principaux facteurs
  d’allongement ou de raccourcissement.
- **Tout** : effectuer les trois modes dans cet ordre : correction du texte,
  revue du scénario corrigé, puis estimation de durée.

Si l’utilisateur nomme explicitement un mode, le suivre. Sinon, déduire le mode
de sa demande ; si elle reste réellement ambiguë, demander s’il veut une
correction, une revue, une estimation ou les trois.

## Procédure

1. Identifier précisément le fichier du scénario et lire son contenu entier.
   Pour une revue de dépôt, relever les faits utiles dans `context/`, `personnages/`,
   `scenarios/` et, si pertinent, la charte graphique. Ne pas traiter une
   hypothèse comme un fait de campagne.
2. Repérer le nombre de PJ et de scènes, les transitions, les indices, les jets,
   les combats, les décisions et les issues. Noter les éventuelles contradictions
   entre ces éléments et les informations de contexte.
3. Appliquer uniquement les opérations permises par le ou les modes demandés.
   Une revue ou une estimation seule est strictement non destructive. Ne jamais
   réécrire le scénario lors d’une revue.
4. Rapporter des observations précises et utiles. Pour une faiblesse, expliquer
   son effet à la table et proposer une piste d’amélioration sans l’appliquer.
   Référencer les scènes ou passages par leur titre et, si disponible, leur
   numéro de ligne.

## Format de réponse — revue

Commencer par un bilan concis de la jouabilité et du principal enjeu de révision.
Présenter ensuite :

1. **Points forts**
2. **Axes d’amélioration prioritaires**, du plus important au moins important
3. **Cohérence avec le contexte et les personnages**
4. **Durée estimée par scène** seulement si elle est également demandée
5. Un tableau récapitulatif final, toujours présent en mode revue :

| Point fort | Axe d’amélioration | Incohérence ou clarification |
|---|---|---|

Ne pas fabriquer d’incohérence : écrire « Aucune repérée » si nécessaire et
placer les questions ouvertes dans la colonne de clarification.

## Format de réponse — durée

Donner une fourchette totale, puis un tableau des scènes et de leurs durées.
Inclure les combats, pauses de discussion et transitions lorsqu’ils sont
pertinents. Expliquer brièvement ce qui ferait varier la durée. Ne pas présenter
une estimation comme une mesure exacte.

## Fin de correction

Après une correction en place, résumer brièvement les types de corrections
effectuées et confirmer que le sens et le style ont été conservés. Ne pas inclure
de suggestions de réécriture non demandées dans le texte corrigé.
