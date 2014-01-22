.. link: 
.. description: 
.. tags: MATE,DConf,GSettings
.. date: 2013/04/27 11:36:00
.. title: How to use GSettings/dconf with dynamic paths
.. slug: 2013-04-27-how-to-use-gsettings-dconf-with-dynamic-paths
.. author: Stefano Karapetsas

As you know, MATE 1.6 migrated to GSettings/dconf and dropped MateConf (the GConf fork). In this post I’ll give you some tips to learn this new configuration system.

dconf-editor

First, I would like to spread this nice guide written by Infirit on our wiki about GSettings and dconf in MATE 1.6:

  * [http://wiki.mate-desktop.org/docs:gsettings](http://wiki.mate-desktop.org/docs:gsettings)

A thing you could miss in dconf-editor is the edit of GSettings values with dynamic paths. Some MATE applications use dynamic paths:

  * mate-panel, for applets and panels configuration
  * mate-terminal, for profiles configuration
  * mate-control-center, for custom keybindings settings

dconf-editor doesnt know the used schema in dynamic paths, so you need to use gsettings tool to change these values:

```
gsettings get SCHEMA[:PATH] KEY
gsettings set SCHEMA[:PATH] KEY VALUE
```

For example:

```
gsettings set org.mate.panel.applet.clock:/org/mate/panel/objects/clock/prefs/ show-seconds false
```
