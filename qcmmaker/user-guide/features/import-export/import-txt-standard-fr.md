# Import TXT standard

Utilisez le format TXT standard lorsque vous voulez créer rapidement des questions depuis un téléphone ou un ordinateur. Vous écrivez les questions dans un fichier `.txt` normal, vous l'enregistrez, puis vous l'importez dans QcmMaker.

C'est le format recommandé pour votre premier import texte, car il se concentre sur l'essentiel : la question, les bonnes réponses, les mauvaises réponses et l'explication facultative.

Quand l'utiliser : choisissez le format standard lorsque votre quiz est principalement textuel et que vous voulez préparer beaucoup de questions plus vite qu'en les saisissant une par une dans l'éditeur.

## Structure de base

Chaque section de question contient :

| Élément | Comment l'écrire |
|---|---|
| Question | Écrivez d'abord le texte de la question. Il peut utiliser plusieurs lignes. |
| Bonne réponse | Commencez la ligne de réponse par `*`. |
| Mauvaise réponse | Commencez la ligne de réponse par `-`. |
| Explication | Commencez la ligne de commentaire par `>`. Cette partie est facultative. |

Exemple :

```text
Parmi les animaux suivants,
lequel vit dans l'eau ?
-Chat
-Chien
*Poisson
-Cheval
> Les poissons sont des animaux aquatiques.
```

## Ajouter plusieurs questions

Séparez chaque section de question par une ligne vide.

```text
Parmi les animaux suivants,
lequel vit dans l'eau ?
-Chat
-Chien
*Poisson
-Cheval
> Les poissons sont des animaux aquatiques.

Lesquels de ces animaux volent ?
*Pigeon
-Chien
*Corbeau
*Aigle
> Les pigeons, les corbeaux et les aigles sont des oiseaux.
```

## Règles rapides

- Placez la question avant les réponses.
- Utilisez `*` avant chaque bonne réponse.
- Utilisez `-` avant chaque mauvaise réponse.
- Utilisez `>` avant l'explication lorsque vous voulez en ajouter une.
- Laissez une ligne vide entre deux questions.
- Enregistrez le fichier au format `.txt`.
- Préférez l'encodage UTF-8, surtout si votre fichier contient des accents, des symboles ou du texte non anglais.

Bon à savoir : les symboles au début des lignes de réponse indiquent à QcmMaker comment interpréter le fichier. `*` signifie que cette réponse doit être traitée comme correcte, `-` signifie qu'il s'agit d'une proposition incorrecte, et `>` devient le texte d'explication affiché pendant la correction quand il est disponible.

## Modèles utiles

Une question avec une seule bonne réponse devient une question simple à réponse unique.

```text
Quelle est l'extension de fichier d'un quiz QcmMaker ?
*qcm
-docx
-xls
> Les quiz QcmMaker sont enregistrés sous forme de fichiers .qcm.
```

Une question avec plusieurs bonnes réponses peut être utilisée pour une sélection multiple.

```text
QcmMaker vous permet de :
*Créer des quiz
*Jouer des quiz
*Partager des quiz
-Modifier des feuilles de calcul
> QcmMaker est conçu pour créer, jouer et partager des fichiers de quiz.
```

Vous pouvez partir du fichier d'exemple ici : [demo_standard-fr.txt](../../../../resources/qxt/demo_standard-fr.txt).

Lorsque vous êtes à l'aise avec cette structure, vous pouvez utiliser [l'import TXT avancé](import-txt-advanced-fr.md) pour ajouter des types de questions, des médias et des métadonnées.
