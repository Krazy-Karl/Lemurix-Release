# Lemurix — téléchargement et installation

Lemurix est un logiciel de gestion pour les PME malgaches : comptabilité,
clients et fournisseurs, stock et commandes, trésorerie. Il fonctionne
**entièrement hors ligne** — vos données restent sur votre ordinateur, dans un
fichier chiffré, et ne partent jamais sur Internet.

## Quel fichier télécharger ?

| Fichier | Pour qui | Droits administrateur |
|---|---|---|
| **`Lemurix_0.1.10_x64_installateur.exe`** | **Tout le monde. C'est la version à prendre.** | **Aucun** |
| `Lemurix_0.1.0_x64-setup.exe` | Ancienne version Tauri, conservée pour les testeurs qui l'utilisent déjà | Oui |
| `Lemurix_0.1.0_x64_en-US.msi` | Ancienne version, format destiné aux déploiements en entreprise | Oui |

Si vous découvrez Lemurix, prenez **`Lemurix_0.1.10_x64_installateur.exe`** et
ignorez les deux autres.

## Installation

1. Téléchargez `Lemurix_0.1.10_x64_installateur.exe`.
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

**C'est normal, et ce n'est pas un virus.** Windows affiche ce message pour
tout logiciel dont l'éditeur n'a pas acheté de certificat auprès d'une
autorité qu'il reconnaît. Ces certificats coûtent plusieurs centaines
d'euros par an ; Lemurix n'en a pas encore.

Pour continuer :

1. Cliquez sur **« Informations complémentaires »**.
2. Cliquez sur **« Exécuter quand même »**.

### Vérifier que le fichier est bien le bon

Puisqu'il n'y a pas de certificat reconnu, le moyen fiable est de comparer
l'empreinte du fichier téléchargé à celle publiée ici. Ouvrez PowerShell
dans votre dossier de téléchargements et tapez :

```powershell
Get-FileHash .\Lemurix_0.1.10_x64_installateur.exe -Algorithm SHA256
```

L'empreinte affichée doit être **exactement** :

```
17F1DFC45406FC6B16AEADB06F68E27E4E437862C8FF31C3AEB4DC84863854AD
```

Si elle diffère, le fichier a été modifié depuis sa publication : ne
l'installez pas et prévenez-moi.

Chaque version publiée ici indique son empreinte. C'est la seule
vérification qui ait une valeur tant qu'un certificat commercial n'est pas
en place : n'importe qui peut fabriquer un certificat portant mon nom, mais
personne ne peut fabriquer un fichier différent ayant la même empreinte.

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
