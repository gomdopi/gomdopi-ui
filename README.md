Simple dark theme with custom colors for IntelliJ products.

Also comes with a custom keymap.

[IntelliJ Plugin Docs](https://jetbrains.org/intellij/sdk/docs/basics/getting_started.html)

# Installation
- ## Clone Git Repo
  ```zsh
  $ cd ${local-git-dir}
  $ git clone git@github.com:gomdopi/gomdopi-ui.git
  $ cd gomdopi-ui
  $ cp resources/keymap/gomdopi.xml ~/.config/JetBrains/IdeaIC<version>/keymaps/
  ```
  - Restart IntelliJ
  - File -> Settings -> Plugins -> Install Plugin from Disk... -> Select `gomdopi-ui/gomdopi-ui.jar`
  - File -> Settings -> Keymap -> Select `GNOME/gomdopi`
  
  > If keymap file is missing check out: [Generate Keymap Xml](https://github.com/gomdopi/gomdopi-ui#generate-keymap-xml)
	
- ## Generate Keymap Xml
  1. Duplicate one of the default keymaps (e.g. GNOME)
  2. Configure keymap as desired for "GNOME duplicate" keymap in IntelliJ
  3. Edit keyboard shortcuts @ File -> Settings -> Keymap:
     - Tool Windows
       - Terminal : Ctrl + T
     - Window
       - Editor Tabs
         - Close : Ctrl + W
         - Reopen Closed Tab : Ctrl + Shift + T
         - Select Next Tab : Ctrl + Tab
         - Select Previous Tab : Ctrl + Shift + Tab
     - {...}
     
  > Store generated file (~/.config/JetBrains/IdeaIC<version>/keymaps/${custom-keymap.xml}) in git repo

  [Configuring keyboard shortcuts](https://www.jetbrains.com/help/idea/configuring-keyboard-and-mouse-shortcuts.html#custom_keymap_location)