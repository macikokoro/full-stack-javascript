# Atom

One of the coolest features of atom.io is to allow you to work in the command line within the same interface. This package comes bundled with keybindings that will help you be faster and more productive.

To install search for term2 in packages within atom or from the terminal run $apm install term2. Once is done installing try this keybinding to open it up.

| Description | Keybinding |
| :--- | :--- |
| term2 | ctrl-alt-arrow-key |

Here is another cool feature worth mentioning, markdown preview is native to atom and will let you preview your README.md from a separate pane within atom.io.

| Description | Keybinding |
| :--- | :--- |
| Markdown | ctrl + shift + m |

## Some cool and useful keyboard shortcuts

| Description | Shortcut |
| :--- | :--- |
| Toggle command palette | shift + ⌘ + p |
| Toggle Sidebar | ⌘ + / |
| Multiple Cursors | ctrl + shift + up |
| Move a line of code up or down | ctrl + ⌘  +  up  or down |

## Update:

**To fix the pty.js install error do the following instead of running `$ apm install`**

```text
git clone https://github.com/svenax/atom-term2.git
cd atom-term2
git checkout update-pty.js 
apm install
sudo apm link .
```

Restart Atom and term2 should be available in your packages list.

**To resolve the newest problem when pressing k on the keyboard**

```text
cd ~/.atom/packages/term2/node_modules
rm -rf atom-term.js
git clone https://github.com/mmckegg/atom-term.js.git atom-term.js
cd atom-term.js
git checkout patch-1
```

… then restart Atom.

