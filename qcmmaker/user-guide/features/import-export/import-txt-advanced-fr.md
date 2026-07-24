# Import TXT avancé

Utilisez le format TXT avancé lorsque le format standard ne suffit pas. Il permet de déclarer des types de questions, d'attacher des médias par URL, d'ajouter des métadonnées et d'utiliser du contenu Markdown ou HTML.

Avant d'utiliser cette page, assurez-vous de comprendre [l'import TXT standard](import-txt-standard-fr.md).

Bon à savoir : le format avancé est plus puissant parce qu'il donne des instructions à QcmMaker avant l'import de la question. Utilisez-le lorsque l'import doit préserver l'intention de l'auteur, et pas seulement le texte visible.

## Types de questions avancés

Ajoutez un type de question au début d'une section de question avec `@type`.

```text
@open
Quel est le résultat de (10 + 1) x 2 ?
*22
> 11 x 2 = 22.
```

Les libellés de type documentés incluent :

| Type | À utiliser pour |
|---|---|
| `auto` | Laisser QcmMaker détecter le type de question. Peut être omis pendant l'édition. |
| `select_all` | Questions de sélection avec plusieurs réponses possibles. Peut être omis pendant l'édition. |
| `open` | Réponse courte saisie au clavier. |
| `put_in_order` | Éléments à remettre dans l'ordre. |
| `fill_in_all_blank` | Remplir plusieurs blancs dans un même texte. |
| `enumerate_all` | Énumérer toutes les réponses attendues. |
| `match_all_column` | Associer des éléments entre colonnes. |
| `jumbled_words` | Reconstruire une phrase à partir de mots mélangés. |

L'exemple avancé montre aussi des variantes pratiques comme `fill_in_each_blank`, `enumerate_each` et `match_each_column`.

## Ajouter des métadonnées

Placez les métadonnées entre crochets après le type de question.

```text
@select_all[
question.image = https://example.com/question-picture.png
question.sound = https://example.com/question-audio.mp3
]
Ce son correspond-il à cet animal ?
*Oui
-Non
> C'est le son de l'animal.
```

Le bloc de métadonnées commence par `[` et se termine par `]`. Chaque ligne de métadonnée utilise cette structure :

```text
target.property = value
```

À quoi servent les métadonnées : elles décrivent un comportement ou des ressources supplémentaires pour la question. Par exemple, elles peuvent attacher une image à l'énoncé, ajouter un son ou configurer la manière dont une réponse doit être interprétée.

## Ajouter des médias aux réponses

Utilisez les index de propositions pour attacher un média ou des options à une réponse précise. Les index commencent à `0`, donc `proposals[0]` est la première réponse, `proposals[1]` la deuxième, et ainsi de suite.

```text
@put_in_order[
proposals[0].image = https://example.com/child.png
proposals[1].image = https://example.com/adult.png
]
Classez ces visages du plus jeune au plus âgé.
*
*
> Faites glisser les réponses dans le bon ordre.
```

Les métadonnées courantes des propositions incluent :

| Métadonnée | Objectif |
|---|---|
| `proposals[index].image` | Attacher une image à une réponse. |
| `proposals[index].sound` | Attacher un son à une réponse. |
| `proposals[index].clue` | Ajouter un indice pour une réponse. |
| `proposals[index].case_sensitive` | Contrôler si les réponses saisies doivent respecter la casse. |

Utilisez des URL téléchargeables pour les médias. Les URI de données peuvent aussi être utilisées lorsqu'elles sont prises en charge par l'application.

## Ajouter des médias aux commentaires

QcmMaker prend en charge une section de commentaire par question. Utilisez `comments[0]` pour les métadonnées du commentaire.

```text
@open[
comments[0].image = https://example.com/explanation.png
]
Citez une couleur de l'arc-en-ciel.
*violet
*bleu
*vert
> L'image montre l'arc-en-ciel complet.
```

## Mettre en forme le contenu avec Markdown ou HTML

Entourez une section de question avec `$md{}` lorsque vous voulez une mise en forme Markdown.

```text
$md{
@select_all
**Quelle planète est la plus proche du soleil ?**
*Mercure
-Vénus
-Terre
> Mercure est la première planète du système solaire.
}
```

Entourez une section de question avec `$html{}` lorsque vous avez besoin de HTML.

```text
$html{
@open
<h3>Nommez une planète du système solaire</h3>
*Terre
*Mars
> La Terre et Mars sont des planètes.
}
```

## Liste de vérification avancée

- Commencez par `@type` lorsque vous voulez imposer un type de question.
- Ajoutez `[...]` uniquement lorsque vous avez besoin de métadonnées.
- Gardez les index de propositions alignés avec l'ordre des réponses.
- Utilisez `comments[0]` pour les médias de commentaire.
- Séparez les sections de questions par une ligne vide.
- Préférez l'encodage UTF-8.

Si un import échoue, simplifiez d'abord le fichier : retirez les métadonnées, gardez une seule question, confirmez que la structure de base fonctionne, puis rajoutez les instructions avancées une par une.

Vous pouvez partir du fichier d'exemple ici : [demo_advanced-fr.txt](../../../../resources/qxt/demo_advanced-fr.txt).

Pour un premier import plus simple, revenez à [l'import TXT standard](import-txt-standard-fr.md).
