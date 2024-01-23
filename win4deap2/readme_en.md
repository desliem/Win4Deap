# **Win4Deap 2**.1.0.1

**Win4Deap 2** provides a convivial Windows front end for **DEAP** written by Tim Coelli. As the name implies, **Win4Deap 2** and its predecessor, **Win4DEAP**, are ***not*** replacements of **DEAP**. It is the latter which performs the numerical calculations required in data envelopment analysis. **Win4Deap 2** cannot make DEA calculations without an installed copy of `DEAP.EXE`. On the other hand`DEAP.EXE`, a DOS console program, will work perfectly well without **Win4Deap 2**.

<!-- TOC -->

- [1. Introduction](#1-introduction)
- [2. Installation](#2-installation)
  - [2.1. Types of installation](#21-types-of-installation)
  - [2.2. Instructions](#22-instructions)
- [3. Example files](#3-example-files)
- [4. Removing **Win4Deap 2**](#4-removing-win4deap-2)
- [5. DISCLAIMER and WARNING](#5-disclaimer-and-warning)
- [6. Acknowledgement](#6-acknowledgement)
- [7. Latest changes](#7-latest-changes)

<!-- /TOC -->

## 1. Introduction

The application provides a grid not unlike a spreadsheet to enter data and writes the necessary instruction and data files for **DEAP**. This means that it is possible to have data files in a folder other than **DEAP**'s. **Win4Deap 2** is a 32-bit Windows application. It has been tested on Windows 7 and 8.1 (64 bit)  but it probably runs on all versions of Windows starting with Windows XP.

## 2. Installation

The installation program for the latest version of ***Win4Deap 2*** is available here: [Win4Deap2Install-2-1-0-1.exe](Win4Deap2Install-2-1-0-1.exe). Click on the link.

![](../img/download_installer.png)

Then click on the `Download raw file` icon as shown above. Once the executable is downloaded, verify its checksum. 

| Hash   |  Win4Deap2Install-2-1-0-1.exe checksum  |
|---   |--- |
| md5  | c6dcf67629b21831c02a000b43ff3546 |
| sha1 | 5fa245f9e3563b7aca4c6e9daedaa54049d08f6c |


### 2.1. Types of installation

**Win4Deap 2** can be run as a "standard" Windows' application or as a "portable" application. 

  - A standard application of **Win4Deap 2** will associate `.wdjson` files to itself which requires modifying Windows' registry. Furthermore, the standard folders will be used to store the application's configuration file and the application's data files.

  - A portable application of **Win4Deap 2** will make no changes to Windows' registry. By default, the application's configuration file and data files will be stored in the folder containing the application.  

    Most often, a portable program is installed on removable media such as thumb drives. But it is entirely possible to choose to perform a portable installation in a hard drive's folder. Just make sure that you have full read and write rights on that folder. In that case, it will be possible to install **DEAP** in the same folder. Conversely, if **DEAP** is already installed, it should be possible to install **Win4Deap 2** in the same folder.

The type of installation is specified at the very end of the installation process.

### 2.2. Instructions

  1. `DEAP.EXE` version 2.1 must be installed and verified to work correctly before trying to install **Win4Deap 2**. Tim Coelli's **DEAP** (containing `DEAP.EXE`, examples and instructions) can be downloaded from the [Centre for Efficiency and Productivity Analysis](https://economics.uq.edu.au/cepa/software) at the University of Queensland. 

  1.  Select the installation language (English or French). This is the language used by the installation program and has nothing to do with the language used in **Win4Deap 2**.

  1.  Read the Welcome screen and click on `Next >`.

  1.  Read the License Agreement, select `I accept the agreement` if you do and then click on `Next >`.

  1.  Select the destination folder.
       -  For a standard installation, you can probably accept the default location.
       -  For a portable installation, browse to a folder where you have full read and write permission. That excludes folders Windows, Program Files and, on 64 bit systems, Program files (x86). 

  1. Select the start menu folder.
       -  For a standard installation, you can probably accept the default location.
       -  For a portable installation, accept the default, it will be ignored in any case as nothing will be added to the Start menu.

  1. Select the type of installation (standard or portable). It is also possible to include national language support or not. Currently **Win4Deap 2** is available in two languages: English and French. It will be possible to translate to other languages if national language support is included.

  1. Finally, click on the Install button and, once the installation is completed `Click` on the `Finish` button.

If a standard installation was chosen, the extension `.wdjson` will be associated with **Win4Deap 2** which will cause `Win4Dep2.exe` to be launched whenever a file with that extension is double clicked. Also an uninstall program will be installed. Finally, a menu item will be added to the Start menu. If a portable installation was selected, the file association will not be performed, a menu item and the uninstall program will not be created.

It is possible to choose **DEAP**'s folder as the destination folder into which **Wind4Deap** is installed. In that case **Win4Deap 2** will find `DEAP.EXE`. Otherwise, it is necessary to specify the location of `DEAP.EXE` in the **Win4Deap 2**'s `Preferences` dialogue.

## 3. Example files

Tim Coelli's four examples are provided in **Win4Deap 2** format (extension .`wdjson`). They are in a folder called, appropriately `Examples`. In a standard installation, that folder will be in a folder called `Win4Deap2` in the user's `Document` folder. In a portable installation, `Examples` will be in the folder containing `Win4Deap2.exe`.

## 4. Removing **Win4Deap 2**

An uninstall program is installed along with Win4Deap2.exe if a standard installation was performed. If a portable installation was chosen, manually delete the installed files. No changes were made to the system in that case.


## 5. DISCLAIMER and WARNING

**Win4Deap 2** is free software that is provided as is. The author of the program accepts no responsibility for any damages that could be caused by this software and makes no warranty, whether implied or implicit, about its fitness for any purpose. The user assumes all risks associated with the program. Please read the copyright notice and license agreement for more.

**Win4Deap 2** should be considered beta software. Backup data often and in both the native `wdjson` format and standard CSV formats.

## 6. Acknowledgement

Thanks to Tim Coelli for **DEAP** without which **Win4Deap 2** is of no use.

Thanks to Jean-Marc Huguenin, Université de Lausane, for helpful comments about **Win4Deap 2** and for mentioning its predecessor, **Win4DEAP**, in the chapter entitled "Data Envelopment Analysis" which he contributed to the book *Multi-criteria Decision Analysis: Methods and Software*, Alessio Ishizaka & Philippe Nemery editors (2013) John Wiley and Sons. See also his paper *Data Envelopment Analysis (DEA) A pedagogical guide for decision makers in the public sector* IDHEAP - Cahier 276/2012, Institut de hautes études en administration publique.

Thanks to Jordan Russell for the Inno Setup Compiler which was used to create the installation program. The setup compiler can be found on the Web at http://www.innosetup.com.

This application was written in Object Pascal with the open source Free Pascal compiler and the free RAD IDE Lazarus:  http://www.freepascal.org/ and http://www.lazarus-ide.org/. Thanks to the team of dedicated volunteers for those excellent open source projects.

Most of the icons are from the Silk icon set by Mark James released under the Creative Commons Attribution 2.5 License: ~~http://www.famfamfam.com/lab/icons/silk/~~ no longer online, but see https://github.com/legacy-icons/famfamfam-silk.

The application's icon was created with the open-source application Greenfish Icon Editor Pro (also written with FreePascal/Lazarus): http://greenfishsoftware.org/.

## 7. Latest changes

Version 2.1.0.1 - Changed version number to 2 to concord with the application's name and fixed many minor bugs.

Version 1.1.2.3 - Fixed errors with filenames containing non-ASCII characters and other minor bug corrections.

Version 1.1.1.3 - various bug corrections, compatibility with MDeap 2 project files completed.

Version 1.1.1.1 - bug correction (i) new project was creating value and price vectors twice the needed size and the saved project file was then not readable (ii) the period when working with panel data was not saved in models. Also modified the (json) file read/write routines to obtain interoperability with upcoming MDeap 2 program.

Version 1.1.0.20 - first released version
