# Partager et ouvrir des liens vers des quiz hébergés

Un lien HTTP est une adresse qui pointe vers un quiz ou une ressource QcmMaker hébergée à distance. Le lien n'est pas le fichier `.qcm` lui-même : il indique à QcmMaker ou au lecteur web où trouver le contenu hébergé.

Le partage par lien est une possibilité supplémentaire destinée aux personnes dont les fichiers `.qcm` sont déjà hébergés en ligne, ou qui souhaitent les héberger afin que les destinataires accèdent au quiz distant au moyen d'une adresse.

## Quand partager un lien ?

Utilisez un lien hébergé lorsque :

- le fichier `.qcm` ou la ressource de quiz compatible est disponible depuis un emplacement en ligne ;
- vous préférez transmettre une adresse plutôt que joindre une copie du fichier ;
- les destinataires doivent pouvoir toucher une adresse ouvrant une prévisualisation, un mode quiz ou un mode examen ;
- vous acceptez que l'accès dépende de la disponibilité de l'emplacement distant.

Contrairement au partage natif du fichier `.qcm`, un lien ne remet pas à lui seul une copie locale autonome au destinataire. L'ouverture du contenu distant nécessite normalement une connexion réseau et le maintien de l'accès à l'emplacement d'hébergement.

## Comment s'ouvrent les liens compatibles ?

QcmMaker peut ouvrir les liens QcmMaker et QcmFile compatibles directement depuis Android. Lorsque QcmMaker est installé, un appui sur un lien compatible peut ouvrir le quiz, l'examen, le projet ou la documentation dans l'application. Si l'application n'est pas installée, le lecteur web peut prendre en charge les liens de quiz compatibles.

Certains appareils Android peuvent demander quelle application doit ouvrir le lien la première fois. Choisissez QcmMaker pour continuer dans l'application.

## Liens pris en charge

| Type de lien | Ce qu'il ouvre |
|--------------|----------------|
| `https://read.qcmfile.com/open?src=...` | Prévisualisation du quiz par défaut. |
| `https://read.qcmfile.com/open?src=...&mode=quiz` | Lecteur quiz. |
| `https://read.qcmfile.com/open?src=...&mode=exam` | Lecteur examen. |
| `https://preview.qcmfile.com/...` | Prévisualisation du quiz. |
| `https://quiz.qcmmaker.com/open?src=...` | Lecteur quiz. |
| `https://exam.qcmmaker.com/open?src=...` | Lecteur examen. |
| `https://edit.qcmmaker.com/open?src=...` | Visionneuse de projet. |
| `https://doc.qcmmaker.com/...` | Documentation QcmMaker. |

La valeur `src` est l'adresse distante du quiz, du projet ou du document à ouvrir. Elle doit être encodée en URL lorsqu'elle contient des caractères spéciaux.

## Exemples

Ouvrir un quiz hébergé en mode prévisualisation :

```text
https://read.qcmfile.com/open?src=https%3A%2F%2Fexample.com%2Fdemo%2F
```

Lancer le même quiz hébergé en mode quiz :

```text
https://read.qcmfile.com/open?src=https%3A%2F%2Fexample.com%2Fdemo%2F&mode=quiz
```

Lancer le même quiz hébergé en mode examen :

```text
https://read.qcmfile.com/open?src=https%3A%2F%2Fexample.com%2Fdemo%2F&mode=exam
```

Ouvrir une page de documentation :

```text
https://doc.qcmmaker.com/documentations/play-modes/body.md
```

## Accès et copies locales

Le contenu distant reste dépendant de son emplacement d'hébergement. Si cet emplacement devient indisponible, restreint, déplacé ou supprimé, le lien peut cesser de fonctionner.

Lorsque QcmMaker permet d'enregistrer ou d'importer un quiz distant dans votre espace de travail, l'occurrence enregistrée devient une copie locale. Les modifications apportées à cette copie locale ne modifient pas la source hébergée, sauf si vous contrôlez et mettez séparément à jour l'emplacement distant.

## Vous préférez le partage natif par fichier ?

Si vous souhaitez que le destinataire reçoive le fichier `.qcm` lui-même, conserve une copie locale et l'utilise sans dépendre de l'adresse d'hébergement d'origine, consultez [Partager un quiz sous forme de fichier `.qcm`](share-a-qcm-file-fr.md).
