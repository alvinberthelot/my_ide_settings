
Petite technique pour sauvegarder et versionner votre configuration sur les préférences de vos IDE.

Cela concerne :

- Sublime Text
- Visual Studio Code

# 1. Pré-requis

Avoir installé [Sublime Text 2](http://www.sublimetext.com/2) ou [Sublime Text 3](http://www.sublimetext.com/3) sur votre OS.

Avoir installé [Visual Studio Code](https://code.visualstudio.com/)

# 2. Installation

## 2.1 Cloner le repository

On clone le repository suivant où on le souhaite, par exemple dans `~/work/config`

	cd ~/work/config

	git clone https://github.com/alvinberthelot/my_ide_settings.git

## 2.2 Identifier le répertoire Sublime Text approprié

Il faut désormais connaître le chemin du répertoire approprié à chaque IDE qui doit contient votre configuration.

⚠ **Attention** le chemin du répertoire peut évidemment varier selon les OS, les IDE et leurs versions.

Un exemple sous Mac OS avec Sublime Text 3 : `~/Library/Application\ Support/Sublime\ Text\ 3/Packages/User`

Un exemple sous Mas OS avec Visual Studio Code : `~/Library/Application\ Support/Code/User`

## 2.3 Réaliser les liens

Sublime Text

	ln -s ~/work/config/my_sublime_text_settings/*.sublime-settings  ~/Library/Application\ Support/Sublime\ Text\ 3/Packages/User

Visual Studio Code

  ln -s ~/work/config/my_ide_settings/visual_studio_code/settings.json  ~/Library/Application\ Support/Code/User

On démarre/redémarre chaque IDE pour bien appliquer les configurations.

On tient à jour ses configurations dans GitHub, c'est tout et c'est déjà pas mal :)
