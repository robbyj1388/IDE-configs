
# 🧠 My Dev Setup: NvChad + Tmux

This is my personal development environment built on top of [NvChad](https://github.com/NvChad/NvChad) and [Tmux](https://github.com/tmux/tmux). It includes support for multiple languages, smart navigation, and a lightweight, fast Neovim configuration.

---

## 🔧 Features

### 🖥️ Tmux

- Seamless pane navigation with **Vim-like keys** (`Ctrl-h/j/k/l`)
- Easy Tmux **window management** with familiar keybindings:
  | Action               | Keybinding      |
  |----------------------|-----------------|
  | Previous window      | `prefix + p`    |
  | Next window          | `prefix + n`    |
  | New window           | `prefix + c`    |
  | Rename window        | `prefix + ,`    |
  | Close pane           | `prefix + x`    |

- Integrated with Neovim via `vim-tmux-navigator`

### 📝 Neovim (NvChad)

- Built with **Lua**, based on NvChad’s modular system
- 🔌 Plugin system with `custom/plugins.lua`
- ✨ LSP support (with `nvim-lspconfig` and `mason.nvim`)
  - Python: Pyright
  - Rust: Rust Analyzer
- 🌈 Treesitter for advanced syntax highlighting
- 🧼 Crystal language auto-formatting
- 📄 Markdown Treesitter parser
- 🐁 Optional mouse support

---

🚀 Getting Started
1. Install NvChad

    git clone https://github.com/NvChad/NvChad ~/.config/nvim --depth 1 && nvim

2. Add Custom Config

Copy your plugins.lua and lspconfig.lua files into:

    ~/.config/nvim/lua/custom/

3. Open Neovim and install LSPs

    :Mason

Use the UI to install pyright, rust-analyzer.
4. Install Treesitter parsers

    :TSInstall lua python rust markdown


