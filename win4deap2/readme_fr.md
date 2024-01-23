# **Win4Deap 2**.1.0.1

**Win4Deap 2** fournit une interface Windows conviviale pour le programme **DEAP** de Tim Coelli. Comme leur nom l'indique, **Win4Deap 2** et son prédécesseur, **Win4DEAP** , ne remplacent pas **DEAP**. C'est ce dernier qui effectue les calculs numériques nécessaires à l'analyse de l'enveloppement des données (AED). **Win4Deap 2** ne peut pas effectuer de calculs AED sans une copie installée de`DEAP.EXE`. En revanche, `DEAP.EXE`, un programme de console DOS, fonctionne parfaitement sans **Win4Deap 2**.

<!-- TOC -->

- [1. Introduction](#1-introduction)
- [2. Installation](#2-installation)
  - [2.1. Types d'installation](#21-types-dinstallation)
  - [2.2. Instructions](#22-instructions)
- [3. Exemples de fichiers](#3-exemples-de-fichiers)
- [4. Suppression de Win4Deap 2](#4-suppression-de-win4deap-2)
- [5. AVIS DE NON-RESPONSABILITÉ et AVERTISSEMENT](#5-avis-de-non-responsabilité-et-avertissement)
- [6. Remerciement](#6-remerciement)
- [7. Dernières modifications](#7-dernières-modifications)

<!-- /TOC -->

## 1. Introduction
L'application fournit une grille semblable à une feuille de calcul pour saisir les données et écrit les instructions et les fichiers de données nécessaires pour **DEAP**. Cela signifie qu'il est possible d'avoir des fichiers de données dans un dossier autre que celui de **DEAP**. **Win4Deap 2** est une application Windows 32 bits. Testé sur Windows 7, 8.1 et 10 (64 bits), ce logiciel fonctionne probablement sur toutes les versions de Windows à partir de Windows XP.

## 2. Installation
Le programme d'installation de la dernière version de **Win4Deap 2** est disponible ici : [Win4Deap2Install-2-1-0-1.exe](Win4Deap2Install-2-1-0-1.exe). Pour l'obtenir, cliquez sur le lien.

![](../img/download_installer.png)

Puis cliquez sur l'icône `Download raw file` pour lanceer le téléchargement. Après le téléchargement du fichier vérifiez sa somme de contrôle.. 

| Algo.   | somme de contrôle de Win4Deap2Install-2-1-0-1.exe |
|---   |--- |
| md5  | c6dcf67629b21831c02a000b43ff3546 |
| sha1 | 5fa245f9e3563b7aca4c6e9daedaa54049d08f6c |

### 2.1. Types d'installation
**Win4Deap 2** peut être exécuté comme une application Windows « standard » ou comme une application « portable ».

- Les fichiers `.wdjson` seront associés à  **Win4Deap 2** lors de l'installation standard, ce qui nécessite de modifier les informations de configuration sauvegardées dans le registre de Windows. De plus, le fichier de configuration de l'application et les fichiers de données de l'application seront stockés dans les dossiers standards.

- Une application portable de **Win4Deap 2** n'apportera aucune modification à la configuration de Windows. Par défaut, le fichier de configuration et les fichiers de données de l'application seront stockés dans le dossier contenant l'application.

Le plus souvent, un programme portable est installé sur un support amovible tel que des clés USB. Mais il est tout à fait possible de choisir d'effectuer une installation portable dans un dossier d'un disque dur. Assurez-vous simplement que vous disposez des droits de lecture et d’écriture sur ce dossier. Dans ce cas, il sera possible d'installer **DEAP** dans le même dossier. À l'inverse, si **DEAP** est déjà installé, il devrait être possible d'installer **Win4Deap 2** dans le dossier contenant **DEAP**.

Le type d'installation est précisé à la toute fin du processus d'installation.

### 2.2. Instructions

1. La version 2.1 de `DEAP.EXE` doit être installée et doit fonctionner correctement avant d'essayer d'installer **Win4Deap 2**. Le programme **DEAP** de Tim Coelli (contenant`DEAP.EXE`, des exemples et des fichiers d'instructions) peut être téléchargé à partir du [Centre for Efficiency and Productivity Analysis](https://economics.uq.edu.au/cepa/software) de l'Université du Queensland.

1. Sélectionnez la langue d'installation (anglais ou français). Il s'agit de la langue utilisée par le programme d'installation et n'a rien à voir avec la langue utilisée dans **Win4Deap 2**.

1. Lisez l'écran de bienvenue et cliquez sur `Suivant >`.

1. Lisez le contrat de licence, sélectionnez `Je comprends et j'accepte les termes du contrat de licence` si c'est acceptable, puis cliquez sur `Suivant >`.

1. Sélectionnez le dossier de destination.
   - Pour une installation standard, vous pouvez probablement accepter l'emplacement par défaut.
   - Pour une installation portable, accédez à un dossier dans lequel vous disposez des autorisations complètes de lecture et d’écriture. Cela exclut les dossiers `Windows`, `Program Files` et, sur les systèmes 64 bits, `Program files (x86)`.
   
   Cliquez sur  `Suivant >`.

1. Sélectionnez le dossier du menu Démarrer.
   - Pour une installation standard, vous pouvez probablement accepter l'emplacement par défaut.
   - Pour une installation portable, acceptez la valeur par défaut, elle sera ignorée dans tous les cas, car rien ne sera ajouté au menu Démarrer.
   
   Cliquez sur  `Suivant >`.
   
1. Sélectionnez le type d'installation (standard ou portable). Il est également possible d'inclure ou non le support des langues nationales. Actuellement **Win4Deap 2** est disponible en deux langues : anglais et français. Il sera possible de traduire dans d'autres langues si la prise en charge des langues nationales est incluse.  

   Cliquez sur  `Suivant >`.

1. Enfin, cliquez sur le bouton `Installer` et, une fois l'installation terminée, cliquez sur le bouton `Terminer`.

Si une installation standard a été choisie, l'extension `.wdjson` sera associée à **Win4Deap 2** , ce qui provoquera le lancement de `Win4Deap2.exe` chaque fois qu'un fichier avec cette extension sera double-cliqué. Un programme de désinstallation sera également installé. Enfin, un élément de menu sera ajouté au menu Démarrer. Si une installation portable a été sélectionnée, l'association de fichiers ne sera pas effectuée, un élément de menu démarrer et le programme de désinstallation ne seront pas créés.

Il est possible de choisir le dossier **DEAP** comme dossier de destination dans lequel **Wind4Deap 2** est installé. Dans ce cas le programme trouvera`DEAP.EXE`. Sinon, il est nécessaire de préciser l'emplacement de `DEAP.EXE` dans les `Préférences` de **Win4Deap 2**.

## 3. Exemples de fichiers

Les quatre exemples de Tim Coelli sont fournis au format **Win4Deap 2** (extension `.wdjson`). Ils se trouvent dans un dossier appelé, à juste titre `examples`. Dans une installation standard, ce dossier se trouvera dans un dossier appelé `Win4Deap2` dans le dossier `Documents` de l'utilisateur. Dans une installation portable, `examples` sera dans le dossier contenant `Win4Deap2.exe`.

## 4. Suppression de Win4Deap 2

Un programme de désinstallation est installé avec `Win4Deap2.exe` si une installation standard a été effectuée. Si une installation portable a été choisie, il suffit de supprimer manuellement les fichiers installés puisqu'aucune modification n’avait été apportée au système.

## 5. AVIS DE NON-RESPONSABILITÉ et AVERTISSEMENT

**Win4Deap 2** est un logiciel gratuit fourni tel quel. L'auteur du programme n'accepte aucune responsabilité pour les dommages qui pourraient être causés par ce logiciel et n'offre aucune garantie, implicite ou implicite, quant à son adéquation à quelque usage que ce soit. L'utilisateur assume tous les risques associés au programme. Veuillez lire l'avis de droit d'auteur et le contrat de licence pour en savoir plus.

**Win4Deap 2** devrait être considéré comme un logiciel bêta. Sauvegardez les données souvent au format natif `.wdjson` et au format CSV standard.

## 6. Remerciement
Merci à Tim Coelli pour **DEAP** sans lequel **Win4Deap 2** ne sert à rien.

Merci à Jean-Marc Huguenin, Université de Lausanne, pour ses commentaires utiles sur **Win4Deap 2** et pour avoir mentionné son prédécesseur, **Win4DEAP** , dans le chapitre intitulé "Data Envelopment Analysis" qu'il a contribué au livre *Multi-criteria Decision Analysis: Methods and Software*, Alessio Ishizaka & Philippe Nemery éditeurs (2013) John Wiley and Sons. Voir aussi son article *Data Envelopment Analysis (DEA) Un guide pédagogique à l'intention des décideurs du secteur public* IDHEAP - Cahier 276/2012, Institut de hautes études en administration publique.

Merci à Jordan Russell pour le compilateur Inno Setup qui a été utilisé pour créer le programme d'installation. Le compilateur d'installation est disponible sur le Web à l'adresse http://www.innosetup.com.

Cette application a été écrite en Object Pascal avec le compilateur open source Free Pascal et l'IDE RAD gratuit Lazarus : http://www.freepascal.org/ et http://www.lazarus-ide.org/. Merci à l'équipe de bénévoles dévoués pour ces excellents projets open source.

La plupart des icônes proviennent du jeu d'icônes Silk de Mark James publié sous la licence Creative Commons Attribution 2.5 : ~~http://www.famfamfam.com/lab/icons/silk/~~ n'est plus en ligne, mais voir https://github.com/legacy-icons/famfamfam-silk.

L'icône de l'application a été créée avec l'application open source Greenfish Icon Editor Pro (également écrite avec FreePascal/Lazarus) : http://greenfishsoftware.org/.

## 7. Dernières modifications
Version 2.1.0.1 - Changement du numéro de version à 2 pour correspondre au nom de l'application et correction de nombreux bogues mineurs.

Version 1.1.2.3 - Correction d'erreurs avec les noms de fichiers contenant des caractères non ASCII et autres corrections de bogues mineurs.

Version 1.1.1.3 - diverses corrections de bogues, compatibilité avec les fichiers du projet MDeap 2 terminés.

Version 1.1.1.1 - correction de bogue (i) le nouveau projet créait des vecteurs de valeur et de prix deux fois plus grands que nécessaire et le fichier de projet enregistré n'était alors pas lisible (ii) la période de travail avec les données de panel n'était pas enregistrée dans les modèles. J'ai également modifié les routines de lecture/écriture du fichier (json) pour obtenir l'interopérabilité avec le prochain programme MDeap 2.

Version 1.1.0.20 - première version publiée
