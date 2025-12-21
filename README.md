# r-tmux-conf

Minimalistic tmux configuration that does not go into your way.

<img width="960" height="540" alt="r-tmux-conf" src="https://github.com/user-attachments/assets/059771ca-174d-488b-9c99-12a02e41d642" />

## Style

r-tmux-conf displays **process names** in panes. The panes are separated with subtle borders.  
The status bar displays the active **session name** and **window list** on the left and the **time**, **date**, and **username@hostname** on the right.

## Features

r-tmux-conf includes the following features:

- Window numbering starts at 1.
- Sessions are retained across restarts.

## Keybindings

r-tmux-conf uses the following keybindings:

| Key              | Action                    |
| ---------------- | ------------------------- |
| Ctrl + Space     | Prefix key                |
| Prefix + \|      | Split horizontally        |
| Prefix + _       | Split vertically          |
| Prefix + r       | Reload tmux configuration |
| Prefix + h/j/k/l | Vim-style pane navigation |

## Installation

Download, install, and apply r-tmux-conf and its dependencies.

### Prerequisites

1. Clone Tmux Plugin Manager (TPM). See [TPM GitHub](https://github.com/tmux-plugins/tpm?tab=readme-ov-file).  
   **Note:** TPM is required to install plugins used in r-tmux-conf.
1. Install and apply Nerd Fonts. For more information, see [Nerd Fonts GitHub](https://github.com/ryanoasis/nerd-fonts).  
   **Note:** Nerd Fonts are required to display icons used in the theme.  
   **Example:** Install Fire Code Nerd Font on macOS by running `brew install --cask font-fira-code-nerd-font`

### Procedure

1. Download r-tmux-conf by running:

   ```sh
   mkdir -p ~/.config/tmux && curl -o ~/.config/tmux/tmux.conf https://raw.githubusercontent.com/rafalkaron/r-tmux-conf/main/tmux.conf
   ```

2. Reload tmux configuration by running `tmux source-file ~/.config/tmux.conf`
