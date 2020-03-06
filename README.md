# Clavier fr-sci

## Description
Configuration d'un clavier azerty. La principale différence est l'ajout des lettres grecques.

![Disposition clavier](https://github.com/hadrien-lem/clavier-fr-sci/blob/master/keyboard-layout.png)

Le fichier `keyboard-layout.json` est à utiliser sur http://www.keyboard-layout-editor.com/

## Installation
Pour Linux via xkb.

* Ajouter le contenu de `fr-sci.txt` à la fin de `/usr/share/X11/xkb/symbols/fr` ;
* Ajouter le code ci-dessous à l'intérieur de `/usr/share/X11/skb/rules/evdev.xml` ;
```xml
<variant>
  <configItem>
    <name>fr-sci</name>
    <description>French (fr-sci)</description>
  </configItem>
</variant>
```
* Se déconnecter/redémarrer ;
* Changer la configuration clavier dans les paramètres.


Testé sur Arch Gnome-Wayland.
