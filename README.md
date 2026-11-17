# Lemurix — téléchargement et installation

Lemurix est un logiciel de gestion pour les petites entreprises de Madagascar :
comptabilité, clients et fournisseurs, stock et commandes, trésorerie. Il
fonctionne **sans internet** : vos données restent sur votre ordinateur, dans un
fichier chiffré.

**C'est une version de test, gratuite pour les testeurs.** La base de données
peut être remise à zéro d'une version à l'autre : n'y mettez pas encore vos
vraies données d'entreprise. Page de présentation :
https://krazy-karl.github.io/Lemurix-Release/

## Quel fichier télécharger ?

Allez sur la page des versions : **[la dernière version](https://github.com/Krazy-Karl/Lemurix-Release/releases/latest)**
et téléchargez le fichier dont le nom se termine par **`installateur.exe`**
(aujourd'hui `Lemurix_0.1.12_x64_installateur.exe`, environ 16 Mo).

Les autres fichiers à la racine de ce dépôt (`Lemurix_0.1.0_…`,
`Lemurix_0.1.10_…`) sont d'anciennes versions conservées pour les testeurs qui
les utilisent déjà : **si vous découvrez Lemurix, ne les prenez pas.**

## Installation

1. Téléchargez `Lemurix_0.1.12_x64_installateur.exe`.
2. Double-cliquez dessus.
3. **Windows peut afficher un avertissement bleu** — voir juste en dessous.
4. Suivez l'assistant, puis lancez Lemurix.

L'installation ne demande **aucun mot de passe administrateur** : le logiciel
s'installe dans votre dossier personnel. Un raccourci est créé sur le bureau et
dans le menu Démarrer. Windows 10 ou 11.

### L'avertissement de Windows, et pourquoi il apparaît

Au lancement de l'installateur, Windows peut afficher un écran bleu :

> **Windows a protégé votre ordinateur**
> Microsoft Defender SmartScreen a empêché le démarrage d'une application non reconnue.

Cela arrive parce que **l'installateur n'est pas signé** : Lemurix n'a pas
encore de certificat d'éditeur reconnu (ils sont payants). Cela ne veut pas
dire que le fichier est dangereux, mais ne vous fiez pas non plus à cet écran
pour juger le fichier : utilisez l'empreinte ci-dessous.

Pour continuer :

1. Cliquez sur **« Informations complémentaires »**.
2. Cliquez sur **« Exécuter quand même »**.

Un antivirus peut aussi réagir à un fichier non signé. **Ne désactivez pas
votre antivirus.** Si le fichier est bloqué, ne l'installez pas et
[écrivez-moi](#un-problème-) : je vous dirai quoi faire.

### Vérifier que le fichier est bien le bon

Comparez l'empreinte du fichier téléchargé à celle publiée ici. Ouvrez
PowerShell dans votre dossier de téléchargements et tapez :

```powershell
Get-FileHash .\Lemurix_0.1.12_x64_installateur.exe -Algorithm SHA256
```

L'empreinte affichée doit être **exactement** :

```
9CD985C8C7F7543C4E62BC63EBD5C04BD9182D0379CA7EA147AD8F201E68580B
```

Si elle diffère, ne l'installez pas et prévenez-moi. Personne ne peut fabriquer
un fichier différent qui aurait la même empreinte.

## Vos données

| | |
|---|---|
| Où sont-elles ? | Dans votre dossier personnel, à l'abri du dossier du programme |
| Sont-elles chiffrées ? | Oui |
| Partent-elles sur Internet ? | Non par défaut. Une option de sauvegarde sur un serveur situé hors de Madagascar existe dans les paramètres ; elle est **désactivée** par défaut. Pour le test, ne l'activez pas. |
| Sont-elles supprimées si je désinstalle ? | **Non.** Le programme part, vos données restent |

Cette dernière ligne compte : vous pouvez désinstaller puis réinstaller une
version plus récente sans rien perdre.

## Désinstallation

**Paramètres** → **Applications** → **Applications installées** → cherchez
« Lemurix » → **Désinstaller**.

## Vous testez Lemurix ?

Le fichier **`Scenario test`** de ce dépôt est un guide qui vous fait monter une
petite entreprise de toutes pièces : créer la société, saisir des clients, des
achats, des ventes, et vérifier que les comptes tombent juste.

Les retours sont précieux, même les petits : une étiquette peu claire, un
chiffre qui vous surprend, un écran où vous ne savez pas quoi faire.

Lemurix ne remplace pas un comptable, ne calcule pas vos impôts et ne fait
aucune déclaration à l'administration.

## Un problème ?

- **L'installation est bloquée** — voir l'avertissement Windows plus haut.
- **Le logiciel ne démarre pas** — redémarrez l'ordinateur et réessayez.
- **Autre chose** — dites-moi où vous étiez, ce que vous avez fait, ce que vous
  attendiez et ce qui s'est passé. N'envoyez jamais votre mot de passe, votre
  clé de récupération ni votre base de données.

Karl Randrianaritiana — WhatsApp : 038 68 817 08
