# Lemurix — téléchargement et installation

Lemurix est un logiciel de gestion pour les PME malgaches : comptabilité,
clients et fournisseurs, stock et commandes, trésorerie. Il fonctionne
**entièrement hors ligne** — vos données restent sur votre ordinateur, dans un
fichier chiffré, et ne partent jamais sur Internet.

## Quel fichier télécharger ?

| Fichier | Pour qui | Droits administrateur |
|---|---|---|
| **`Lemurix_1.0.0_x64_installateur.exe`** | **Tout le monde. C'est la version à prendre.** | **Aucun** |
| `Lemurix_0.1.0_x64-setup.exe` | Ancienne version, conservée pour les testeurs qui l'utilisent déjà | Oui |
| `Lemurix_0.1.0_x64_en-US.msi` | Ancienne version, format destiné aux déploiements en entreprise | Oui |

Si vous découvrez Lemurix, prenez **`Lemurix_1.0.0_x64_installateur.exe`** et
ignorez les deux autres.

## Installation

1. Téléchargez `Lemurix_1.0.0_x64_installateur.exe`.
2. Double-cliquez dessus.
3. **Windows va afficher un avertissement bleu** — voir juste en dessous.
4. Suivez l'assistant, puis lancez Lemurix.

L'installation ne demande **aucun mot de passe administrateur** : le logiciel
s'installe dans votre dossier personnel. Un raccourci est créé sur le bureau et
dans le menu Démarrer.

### L'avertissement de Windows, et pourquoi il apparaît

Au lancement de l'installateur, Windows affiche un écran bleu :

> **Windows a protégé votre ordinateur**
> Microsoft Defender SmartScreen a empêché le démarrage d'une application non reconnue.

**C'est normal, et ce n'est pas un virus.** Windows affiche ce message pour tout
logiciel qui n'a pas encore été téléchargé par des milliers de personnes, ou
dont l'éditeur n'a pas acheté de certificat commercial. Lemurix est signé, mais
par un certificat créé par son auteur, que Windows ne connaît pas encore.

Pour continuer :

1. Cliquez sur **« Informations complémentaires »**.
2. Cliquez sur **« Exécuter quand même »**.

Vous pouvez vérifier avant d'installer que le fichier est bien celui-ci :
clic droit sur l'installateur → **Propriétés** → onglet **Signatures
numériques**. Le signataire doit être **Karl Randrianaritiana**. Si ce n'est pas
le cas, ne l'installez pas et prévenez-moi.

## Vos données

| | |
|---|---|
| Où sont-elles ? | Dans votre dossier personnel, à l'abri du dossier du programme |
| Sont-elles chiffrées ? | Oui |
| Partent-elles sur Internet ? | Non, jamais |
| Sont-elles supprimées si je désinstalle ? | **Non.** Le programme part, vos données restent |

Cette dernière ligne compte : vous pouvez désinstaller puis réinstaller une
version plus récente sans rien perdre.

## Désinstallation

**Paramètres** → **Applications** → **Applications installées** → cherchez
« Lemurix » → **Désinstaller**.

## Vous testez Lemurix ?

Le fichier **`Scenario test`** de ce dépôt est un guide qui vous fait monter une
petite entreprise de toutes pièces : créer la société, saisir des clients, des
achats, des ventes, et vérifier que les comptes tombent juste. C'est le meilleur
moyen de faire le tour du logiciel en une session.

Les retours sont précieux, même les petits : une étiquette peu claire, un
chiffre qui vous surprend, un écran où vous ne savez pas quoi faire.

## Un problème ?

- **L'installation est bloquée** — voir l'avertissement Windows plus haut. Si
  votre antivirus la bloque, désactivez-le le temps de l'installation.
- **Le logiciel ne démarre pas** — redémarrez l'ordinateur et réessayez.
- **Autre chose** — écrivez-moi avec le message d'erreur exact, ou une photo de
  l'écran.

Karl Randrianaritiana — karlrandrianaritiana@gmail.com
