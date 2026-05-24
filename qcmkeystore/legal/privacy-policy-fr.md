# Politique de Confidentialité — Qcm Locker

**Dernière mise à jour : 2026-05-24**

Cette Politique de Confidentialité explique comment QmakerTech (« nous ») collecte,
utilise et protège les informations lorsque vous utilisez **Qcm Locker**
(identifiant : `com.qmaker.qcm.keystore`), une application Android qui permet aux
auteurs de quiz de créer des loquets, de générer des PassCodes et de protéger des
fichiers quiz `.qcm`.

En utilisant Qcm Locker, vous acceptez les pratiques décrites dans cette politique.

---

## 1. Qui Sommes-Nous

Qcm Locker est développé et exploité par **QmakerTech**.  
Contact : contact@qmakertech.com

---

## 2. Données Collectées

### 2.1 Informations du compte Google

Qcm Locker nécessite un compte Google pour se connecter. Lors de l'authentification,
nous recevons de Google les informations suivantes :

| Donnée | Finalité |
|---|---|
| Nom d'affichage | Identifier votre compte dans l'application |
| Adresse e-mail | Associer de manière unique vos loquets et PassCodes à votre compte |
| URL de la photo de profil | Afficher votre avatar dans le menu de navigation |

Nous ne recevons pas votre mot de passe Google.

### 2.2 Données des loquets

Lorsque vous créez ou modifiez un loquet, les informations suivantes sont envoyées
et stockées sur les serveurs QcmKeyStore exploités par QmakerTech :

| Donnée | Finalité |
|---|---|
| Nom du loquet | Afficher et identifier le loquet |
| Mot de passe du loquet (chiffré) | Protéger le contenu des fichiers `.qcm` |
| Date d'expiration (optionnel) | Imposer un accès limité dans le temps |
| Limite d'usage (optionnel) | Limiter le nombre total d'utilisations autorisées |
| Paramètre multi-propriétaire | Contrôler si un PassCode peut être utilisé sur plusieurs appareils |
| Date de création | Trier et afficher les loquets dans la liste principale |

### 2.3 Données des PassCodes

Lorsque vous générez des PassCodes, les informations suivantes sont stockées sur les
serveurs QcmKeyStore :

| Donnée | Finalité |
|---|---|
| Valeurs des PassCodes | Distribuées aux utilisateurs autorisés pour déverrouiller les quiz protégés |
| Compteur d'utilisation | Suivre le nombre d'utilisations de chaque code |
| Expiration par code (optionnel) | Imposer des codes limités dans le temps |
| Limite d'usage par code | Limiter le nombre d'utilisations par code |

### 2.4 Accès aux fichiers quiz

Lorsque vous appuyez sur **Protéger un fichier .qcm**, Qcm Locker lit le fichier
`.qcm` source que vous sélectionnez et écrit le fichier protégé dans le stockage
de votre appareil. Ce traitement s'effectue entièrement **sur votre appareil**. Le
contenu du fichier quiz n'est jamais téléchargé vers les serveurs QmakerTech.

### 2.5 Données Non Collectées

Qcm Locker n'accède pas et ne collecte **pas** :

- Les données de localisation
- La caméra ou le microphone
- Les contacts ou les journaux d'appels
- Les identifiants d'appareil au-delà de ce que Firebase Authentication nécessite

---

## 3. Utilisation de Vos Données

| Donnée | Utilisation |
|---|---|
| Informations du compte Google | Vous authentifier et associer vos loquets à votre compte |
| Données des loquets et PassCodes | Fournir le service QcmKeyStore — valider les PassCodes lorsqu'un lecteur ouvre un fichier protégé |
| Accès aux fichiers | Protéger les fichiers quiz localement sur votre appareil |

Nous ne vendons, ne louons et ne partageons pas vos données personnelles avec des
tiers à des fins commerciales.

---

## 4. Services Tiers

### Google Sign-In / Firebase Authentication

L'authentification est gérée par **Firebase Authentication**, un service Google.
Lorsque vous vous connectez, vos données sont traitées conformément à :

- [Politique de confidentialité Google](https://policies.google.com/privacy?hl=fr)
- [Conditions d'utilisation Firebase](https://firebase.google.com/terms)

### QcmKeyStore

Les données des loquets et des PassCodes sont stockées sur **QcmKeyStore**, un service
backend exploité exclusivement par QmakerTech. Aucun tiers n'a accès à ces données.

---

## 5. Conservation des Données

| Donnée | Durée de conservation |
|---|---|
| Informations du compte Google | Gérées par Google ; nous conservons uniquement ce que Firebase Authentication fournit par session |
| Données des loquets | Conservées jusqu'à la désactivation du loquet ou une demande de suppression |
| Données des PassCodes | Conservées jusqu'à la désactivation du loquet associé ou une demande de suppression |
| Fichiers `.qcm` protégés | Stockés uniquement sur votre appareil ; nous n'en conservons aucune copie |

---

## 6. Sécurité des Données

Les mots de passe des loquets sont stockés chiffrés sur les serveurs QcmKeyStore.
L'accès au service nécessite un jeton d'authentification Google valide. Nous
appliquons des pratiques de sécurité standard pour protéger les données en transit
(HTTPS) et au repos.

---

## 7. Vos Droits

Vous disposez des droits suivants :

- **Accès** aux données que nous détenons vous concernant.
- **Suppression** de vos loquets, PassCodes et données de compte à tout moment en
  nous contactant.
- **Déconnexion** de Qcm Locker à tout moment via le menu de navigation.
- **Retrait du consentement** en désinstallant l'application et en demandant la
  suppression de vos données.

Pour exercer l'un de ces droits, contactez-nous à : **contact@qmakertech.com**

---

## 8. Mineurs

Qcm Locker n'est pas destiné aux enfants de moins de 13 ans. Nous ne collectons pas
sciemment de données personnelles auprès d'enfants. Si vous pensez qu'un enfant nous
a fourni des données personnelles, veuillez nous contacter et nous les supprimerons
dans les meilleurs délais.

---

## 9. Modifications de Cette Politique

Nous pouvons mettre à jour cette Politique de Confidentialité ponctuellement. Nous
mettrons à jour la date « Dernière mise à jour » en haut de cette page. L'utilisation
continue de Qcm Locker après les modifications vaut acceptation de la politique mise
à jour.

---

## 10. Contact

**QmakerTech**  
E-mail : contact@qmakertech.com

---

*Cette politique s'applique exclusivement à l'application Android Qcm Locker
(`com.qmaker.qcm.keystore`). Les autres applications QmakerTech sont régies par
leurs propres politiques de confidentialité.*
