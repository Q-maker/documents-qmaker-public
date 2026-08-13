# Modes de lecture

QcmMaker propose deux expériences pour lire un quiz : le mode **Examen** et le
mode **Challenge**. Le premier reproduit une épreuve que l’on termine avant de
voir la correction ; le second privilégie un entraînement séquentiel avec un
retour immédiat après chaque réponse.

| Choisissez | Lorsque vous souhaitez |
|---|---|
| Examen | Parcourir les questions, modifier vos réponses et gérer le temps de l’épreuve avant de terminer. |
| Challenge | Répondre dans l’ordre, connaître immédiatement le résultat et enchaîner rapidement. |

## Mode Examen

Utilisez **Précédent** et **Suivant** pour parcourir le questionnaire. Vous
pouvez revenir sur une question et modifier sa réponse tant que l’épreuve n’est
pas terminée. Le tableau de navigation permet de repérer les questions
répondues, non répondues ou marquées lorsque ces états sont disponibles.

La dernière action **Suivant** permet de terminer. QcmMaker affiche alors le
score, le temps écoulé et les actions autorisées : revoir la correction,
recommencer ou quitter. La correction n’est visible qu’après la fin et seulement
si l’auteur du quiz l’a autorisée.

![Début d’un examen](images/exam-start.png)

> Les captures détaillées des différents types de questions ont été réalisées
> en mode Examen afin de conserver une présentation visuelle cohérente. Les
> mêmes familles de questions peuvent être utilisées en mode Challenge, mais le
> rythme de navigation et le moment où la correction apparaît diffèrent.

Consultez le [guide visuel des types de questions](exam-question-types/README-fr.md).

## Mode Challenge

Le Challenge présente les questions successivement. Après la sélection ou
l’action de validation, QcmMaker affiche immédiatement une réussite, un échec,
une réussite partielle ou une question passée lorsque cet état existe. Le
passage suivant peut être automatique après un compte à rebours ou manuel,
selon les réglages.

L’en-tête peut afficher les points obtenus et le temps restant pour la question.
Une réponse composée propose **Réinitialiser** et **Valider**. Après validation,
le bandeau de résultat peut afficher une explication avec image ou son, l’action
d’ajout aux favoris, **Pause** et **Suivant**.

Le lecteur peut utiliser un chronomètre, des sons, une vibration et des effets
visuels pour signaler l’action ou le résultat. Leur présence dépend du quiz, des
réglages du lecteur et de l’appareil.

![Début d’un challenge](images/challenge-start.png)

## Temps, médias et interruption

Un quiz peut avoir une limite globale, une limite par question ou aucune limite
visible. Les questions et propositions peuvent contenir des images et des sons :
utilisez les contrôles affichés pour agrandir ou écouter le contenu. Le bouton
Retour d’Android demande confirmation avant d’abandonner une session active.

Après une rotation ou une reprise de l’application, vérifiez la question et le
temps restaurés avant de continuer. La restauration dépend de la disponibilité
du quiz et de l’état de session sauvegardé.

Sur la version Android observée, une rotation pendant un Examen a conservé la
question courante, le tableau de progression ouvert et le chronomètre global en
cours.

Les boutons textuels principaux sont identifiables par les services
d’accessibilité. Sur la version Android observée, certaines actions uniquement
représentées par une image ne possédaient toutefois pas de libellé vocal utile ;
un utilisateur de lecteur d’écran peut avoir besoin d’aide pour ces contrôles.

## Résultat, correction et nouvelle tentative

À la fin, choisissez **Corriger** pour relire les réponses si le quiz l’autorise,
**Rejouer** pour lancer une nouvelle tentative, ou **Quitter**. Les options de
rejeu peuvent cibler tout le test, les réponses échouées, les questions manquées
ou les favoris selon le contenu de la tentative.

![Résultat d’un examen](images/exam-result.png)
