# Organiser, valider et enregistrer les questions

La barre supérieure regroupe les actions d'édition, le tiroir droit affiche la liste des questions et la barre inférieure permet la navigation séquentielle ou numérique.

## Comprendre les erreurs de validation

QcmMaker valide la page lorsque vous avancez ou enregistrez. La consigne du type devient rouge et précise ce qui manque.

### Sélection sans bonne réponse

![Erreur de validation d'une sélection](./assets/selection-validation-error.png)

Avec au moins deux choix remplis, cochez au moins une bonne réponse. Si vous vouliez une réponse libre, choisissez explicitement le type Réponse à saisir.

### Mise en ordre avec trop peu d'éléments

![Erreur de mise en ordre](./assets/order-validation-error.png)

Saisissez au moins deux éléments dans leur ordre de référence.

Les autres types structurés refusent aussi les ensembles incomplets : une association exige des paires complètes, un texte à trous exige les valeurs de ses trous et une réponse ouverte exige un texte accepté. Complétez ou retirez toute page inachevée.

## Utiliser la barre d'actions

![Menu d'enregistrement](./assets/actionbar-save-menu.png)

| Commande | Rôle |
|---|---|
| Retour | Quitte l'éditeur et demande quoi faire si des changements sont en attente. |
| Enregistrer | Enregistre, enregistre et lance, ou permet de choisir un mode. |
| Supprimer (X) | Efface ou supprime la question courante. |
| Insérer | Duplique, insère avant/après, colle ou importe des questions. |
| Liste | Ouvre le tiroir des questions. |

## Naviguer et réordonner avec le tiroir

![Tiroir des questions](./assets/question-drawer.png)

- Touchez le texte d'une question pour l'ouvrir.
- Maintenez puis faites glisser une ligne pour changer sa position.
- Touchez le numéro à gauche pour ouvrir son menu contextuel.

![Menu du numéro d'index](./assets/question-index-popup.png)

**Move / Déplacer** explique le glisser-déposer. **Delete / Supprimer** retire la question ; vérifiez l'index sélectionné avant de confirmer.

## Aller directement à une page

![Dialogue de navigation rapide](./assets/fast-navigation.png)

Touchez l'index central de la barre inférieure, par exemple `15/16`, saisissez un numéro et validez. Utilisez **Previous/Next** pour les questions voisines et ce dialogue pour une destination éloignée.

## Avant de quitter

1. Corrigez toute consigne rouge.
2. Enregistrez le quiz.
3. Choisissez **Save & play using** pour vérifier un mode particulier.
4. Contrôlez l'énoncé, les réponses, les médias, le commentaire, le temps et le score comme les verra le participant.

Quitter sans enregistrer abandonne la session d'édition, y compris les nouveaux médias.

**Précédent :** [Images, sons et commentaires](media-and-comments-fr.md)

**Suivant :** [Tester le quiz dans un mode de jeu](../play-modes/README-fr.md)
