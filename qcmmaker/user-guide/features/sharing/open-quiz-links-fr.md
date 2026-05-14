# Ouvrir des liens de quiz partagés

QcmMaker peut ouvrir les liens QcmMaker et QcmFile compatibles directement depuis Android. Lorsque QcmMaker est installé, un appui sur l'un de ces liens peut ouvrir le quiz, l'examen, le projet ou la documentation dans l'application. Si l'application n'est pas installée, le même lien peut être pris en charge par le lecteur web lorsque le site le prend en charge.

## Liens pris en charge

Utilisez ces liens pour partager du contenu avec un autre utilisateur de QcmMaker :

| Type de lien | Ce qu'il ouvre |
|--------------|----------------|
| `https://read.qcmfile.com/open?src=...` | Prévisualisation du quiz (par défaut). |
| `https://read.qcmfile.com/open?src=...&mode=quiz` | Lecteur quiz. |
| `https://read.qcmfile.com/open?src=...&mode=exam` | Lecteur examen. |
| `https://preview.qcmfile.com/...` | Prévisualisation du quiz. |
| `https://quiz.qcmmaker.com/open?src=...` | Lecteur quiz. |
| `https://exam.qcmmaker.com/open?src=...` | Lecteur examen. |
| `https://edit.qcmmaker.com/open?src=...` | Visionneuse de projet. |
| `https://doc.qcmmaker.com/...` | Documentation QcmMaker. |

La valeur `src` est l'adresse du quiz, du projet ou du document à ouvrir. Elle doit être encodée en URL lorsqu'elle contient des caractères spéciaux.

## Exemples

Ouvrir un quiz partagé en mode prévisualisation :

```text
https://read.qcmfile.com/open?src=https%3A%2F%2Fexample.com%2Fdemo%2F
```

Lancer le même quiz partagé en mode quiz :

```text
https://read.qcmfile.com/open?src=https%3A%2F%2Fexample.com%2Fdemo%2F&mode=quiz
```

Lancer le même quiz partagé en mode examen :

```text
https://read.qcmfile.com/open?src=https%3A%2F%2Fexample.com%2Fdemo%2F&mode=exam
```

Ouvrir une page de documentation :

```text
https://doc.qcmmaker.com/documentations/play-modes/body.md
```

## Remarques

Certains appareils Android peuvent demander quelle application doit ouvrir le lien la première fois. Choisissez QcmMaker pour continuer dans l'application.

Les fichiers distants ouverts depuis un lien sont destinés à la lecture, la prévisualisation ou le jeu. Pour modifier un quiz partagé de façon permanente, sauvegardez-le ou importez-le d'abord dans votre propre espace de travail.
