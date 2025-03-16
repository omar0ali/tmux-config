# tmux-config
tmux configuration with mouse support, pane navigation, and custom keybindings.

## setup
Clone this repo and link the config file:

```bash
git clone https://github.com/yourusername/tmux-config.git ~/.config/tmux
ln -s ~/.config/tmux/tmux.conf ~/.tmux.conf
tmux source-file ~/.tmux.conf
```

### hotkeys
Key Binding	Action
| Key Binding         | Action                         |
|---------------------|--------------------------------|
| `h`, `j`, `k`, `l` | Move between panes (Vim-style) |
| `Prefix + H/J/K/L` | Resize panes                   |
| `Prefix + r`       | Reload tmux configuration      |
| `Prefix + c`       | Create new window              |
| `Prefix + &`       | Kill current window            |
| `Prefix + n`       | Switch to next window          |
| `Prefix + p`       | Switch to previous window      |

>[!NOTE]
>The default prefix key is Ctrl + b. You can change this in tmux.conf.

### customization

```bash
set-option -g status-bg blue  # "blue" to another color
set-option -g status-fg white
```

```bash
# update pane navigation keybindings
bind-key h select-pane -L
bind-key j select-pane -D
bind-key k select-pane -U
bind-key l select-pane -R
```

>checkout my [nvim-config](https://github.com/omar0ali/nvim-config)
