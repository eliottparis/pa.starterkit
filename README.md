# StarterKit

Kit de démarrage pour le [cours de programmation en C/C++](https://github.com/paccpp/paccpp)

Ce répertoire contient:
- Un script CMake permettant de générer des projets.
- Un projet de départ nommé "[helloworld](source/projects/helloworld)".

### Installation

- Commencez par [configurer votre environnement de travail](https://github.com/paccpp/paccpp/blob/master/setup/readme.md).

- Télécharger ensuite ce répertoire en local sur votre machine.

- Se rendre dans le répertoire téléchargé (`cd "path_to_directory"`)

- Créer un dossier nommé "build" : `mkdir build`

- Se rendre dans le répertoire "build" : `cd build`

- La génération de projet est ensuite spécifique à chaque plateforme:

- Sur **OSX**
  - Taper `cmake -G Xcode ..` pour générer un projet Xcode.


- Sur **Windows**
  - La ligne de commande exacte à taper va dépendre de votre version de Visual Studio.
  - tapez `cmake --help` pour avoir une liste des options disponibles.
  - Si vous avez Visual Studio 2013 par exemple, la commande à lancer ressemblera à:
    - 32 bit: `cmake -G "Visual Studio 12" ..`
    - 64 bit: `cmake -G "Visual Studio 12 Win64" -DWIN64:Bool=True ..`


- Pour générer un **MakeFile**

  - Taper `cmake ..`
  - Vous pourrez ensuite compiler en tapant simplement `make`
