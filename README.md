# VSCode + Neovim (Pack)

Collection of basic extension to get started with Neovim in VSCode. The purpose of this extension is to enhance navigation in Neovim by leveraging VSCode extensions.

It is recommended to use the configuration in this [repository](https://github.com/AGutierrezR/VSCode-NeoVim), as it includes specific settings for these extensions and adds a list of Neovim plugins to enhance your experience:

- smoka7/hop.nvim
- echasnovski/mini.ai
- echasnovski/mini.surround
- nvim-treesitter/nvim-treesitter
- nvim-treesitter/nvim-treesitter-textobjects

This initial configuration also serves as a great starting point for getting into Vim motions and improving productivity in Neovim.

## Configuration Neovim (Lua)

The Neovim configuration on the system can be found at the following path:

- MacOS & Linux: `~/.config/nvim/`
- Windows: `~/AppData\Local\nvim`

### If you use the recommended respository:

1. Clone this repository:
   
   For MacOS & Linux:

   ```bash
   git clone https://github.com/AGutierrezR/VSCode-NeoVim.git ~/.config/nvim
   ```

   For Windows:

   ```bash
   git clone https://github.com/AGutierrezR/VSCode-NeoVim.git ~\AppData\Local\nvim
   ```

## Configuration VSCode

These VSCode keybindings enhance the user experience. To configure them in VSCode, press `F1` and search for `workbench.action.openGlobalKeybindingsFile`. This will open the `keybindings.json` file. In this file, add the following configuration to the keybindings array.

```json
[
  // Neovim - Normal Mode
  {
    "key": "ctrl+y",
    "command": "vscode-neovim.send",
    "when": "editorTextFocus && neovim.init && neovim.mode == 'normal'",
    "args": "<C-y>"
  },
  {
    "key": "ctrl+e",
    "command": "vscode-neovim.send",
    "when": "editorTextFocus && neovim.init && neovim.mode == 'normal'",
    "args": "<C-e>"
  },
  // NeoVim - Insert Mode
  {
    "key": "ctrl+y",
    "command": "vscode-neovim.send",
    "when": "editorTextFocus && neovim.init && neovim.mode == 'insert'",
    "args": "<C-y>"
  },
  {
    "key": "ctrl+l",
    "command": "vscode-neovim.send",
    "when": "editorTextFocus && neovim.init && neovim.mode == 'insert'",
    "args": "<C-l>"
  },
  {
    "key": "ctrl+e",
    "command": "vscode-neovim.send",
    "when": "editorTextFocus && neovim.init && neovim.mode == 'insert'",
    "args": "<C-e>"
  },
  {
    "key": "ctrl+x",
    "command": "vscode-neovim.send",
    "when": "editorTextFocus && neovim.init && neovim.mode == 'insert'",
    "args": "<C-x>"
  },
  {
    "key": "ctrl+p",
    "command": "vscode-neovim.send",
    "when": "editorTextFocus && neovim.init && neovim.mode == 'insert'",
    "args": "<C-p>"
  },
  {
    "key": "ctrl+n",
    "command": "vscode-neovim.send",
    "when": "editorTextFocus && neovim.init && neovim.mode == 'insert'",
    "args": "<C-n>"
  },
  {
    "key": "ctrl+z",
    "command": "vscode-neovim.send",
    "when": "editorTextFocus && neovim.init && neovim.mode == 'insert'",
    "args": "<C-z>"
  },
  {
    "key": "ctrl+h",
    "command": "vscode-neovim.send",
    "when": "editorTextFocus && neovim.init && neovim.mode == 'insert'",
    "args": "<C-h>"
  },
  {
    "key": "ctrl+m",
    "command": "vscode-neovim.send",
    "when": "editorTextFocus && neovim.init && neovim.mode == 'insert'",
    "args": "<C-m>"
  },
  {
    "key": "ctrl+i",
    "command": "vscode-neovim.send",
    "when": "editorTextFocus && neovim.init && neovim.mode == 'insert'",
    "args": "<C-i>"
  },
  {
    "key": "ctrl+k",
    "command": "vscode-neovim.send",
    "when": "editorTextFocus && neovim.init && neovim.mode == 'insert'",
    "args": "<C-k>"
  },
  {
    "key": "ctrl+b",
    "command": "vscode-neovim.send",
    "when": "editorTextFocus && neovim.init && neovim.mode == 'insert'",
    "args": "<C-b>"
  },
  {
    "key": "ctrl+g",
    "command": "vscode-neovim.send",
    "when": "editorTextFocus && neovim.init && neovim.mode == 'insert'",
    "args": "<C-g>"
  },
  {
    "key": "ctrl+q",
    "command": "vscode-neovim.send",
    "when": "editorTextFocus && neovim.init && neovim.mode == 'insert'",
    "rgs": "<C-q>"
  }
]
```
