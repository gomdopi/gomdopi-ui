Simple dark theme with custom colors for IntelliJ products

[IntelliJ Plugin Docs](https://jetbrains.org/intellij/sdk/docs/basics/getting_started.html)

# Installation
- ## Clone git repo
  ```
  $ cd ${local-git-dir}
  $ git clone git@github.com:gomdopi/gomdopi-ui.git
  $ cd gomdopi-ui
  # if keymap file is missing or hasn't been generated check out "generating keymap xml file" section below
  $ cp resources/keymap/gomdopi.xml ~/.config/JetBrains/IdeaIC<version>/keymaps/${custom-keymap.xml}
  ```
  > Reload IntelliJ
  >
  > File -> Settings -> Plugins -> Install Plugin from Disk... -> Choose ${local-plugin-repo-dir}/gomdopi-ui.jar
  >
  > File -> Settings -> Keymap -> ${custom-keymap.xml}
	
- ## Generate keymap xml
  1. Duplicate one of the default keymaps (e.g. GNOME)
  2. Configure keymap as desired for "GNOME duplicate" keymap in IntelliJ
  3. Edit keyboard shortcuts @ File -> Settings -> Keymap
     - Tool Windows
       - Terminal : Ctrl + T
     - Window
       - Editor Tabs
         - Close : Ctrl + W
         - Reopen Closed Tab : Ctrl + Shift + T
         - Select Next Tab : Ctrl + Tab
         - Select Previous Tab : Ctrl + Shift + Tab

  > Store generated file (~/.config/JetBrains/IdeaIC<version>/keymaps/${keymap.xml}) in git repo

  [Docs](https://www.jetbrains.com/help/idea/configuring-keyboard-and-mouse-shortcuts.html#custom_keymap_location)