
# Manual

### Installation of `tmux` on Linux and configuring.
clone to the repository
```bash
 git clone "https://github.com/parthivkumarnikku/terminal.git" && cd terminal/tmux
```

Install tmux 
```bash
sudo apt install tmux
``` 
Install a Clipboard Integration Tool
#### Linux
```bash
# Install xclip
sudo apt install xclip  # For Ubuntu/Debian
```

copy the configuration file to home directory
```bash
cat .tmux.conf >> ~/.tmux.conf
```

Reload tmux configuration
```bash
tmux source-file ~/.tmux.conf
```
### Copying text in tmux
1. Enter copy mode: Ctrl-b [
2. Navigate and select using `space key` and,
3. Press `y` to `copy` the selection to the system clipboard.
4. Paste is as usual `ctrl + shift + v`
---
## or
### Set Tmux to Automatically Use the Clipboard
To make Tmux always copy to the system clipboard without extra bindings, use this configuration:

```bash
# Automatically use the system clipboard
set-option -g set-clipboard on
```
This tells Tmux to integrate directly with the system clipboard when copying text. Ensure your Tmux version supports this (Tmux 2.6 or newer).


| Column 1 | Column 2 | Column 3 |

|---|---|---|

| Data 1 | Data 2 | Data 3 |

| Data 4 | Data 5 | Data 6 |

# Manual

### Installation of `tmux` on Linux and configuring.
clone to the repository
```bash
 git clone "https://github.com/parthivkumarnikku/terminal.git" && cd terminal/tmux
```

Install tmux 
```bash
sudo apt install tmux
``` 
Install a Clipboard Integration Tool
#### Linux
```bash
# Install xclip
sudo apt install xclip  # For Ubuntu/Debian
```

copy the configuration file to home directory
```bash
cat .tmux.conf >> ~/.tmux.conf
```

Reload tmux configuration
```bash
tmux source-file ~/.tmux.conf
```
### Copying text in tmux
1. Enter copy mode: Ctrl-b [
2. Navigate and select using `space key` and,
3. Press `y` to `copy` the selection to the system clipboard.
4. Paste is as usual `ctrl + shift + v`
---
## or
### Set Tmux to Automatically Use the Clipboard
To make Tmux always copy to the system clipboard without extra bindings, use this configuration:

```bash
# Automatically use the system clipboard
set-option -g set-clipboard on
```
This tells Tmux to integrate directly with the system clipboard when copying text. Ensure your Tmux version supports this (Tmux 2.6 or newer).

## Some basic shortcuts

`<leader> = ctrl + b` will be refered to `lead` in the following context.

| **Shortcut**              | **Description**                                                                          |
|----------------------------|------------------------------------------------------------------------------------------|
| tmux new -t <session_name> | Creates a session along with the window.                                               |
| tmux kill-server         | Kills the tmux server and all associated sessions.                                       |
| `lead` new -s <session_name> | Creates a new tmux session.                                                           |
| `lead` ls                  | Lists available sessions.                                                               |
| `lead` d                  | Detaches from the current session.                                                      |
| `lead` a -t <session_name> | Attaches to the specified session.                                                      |
| `lead` ,                   | Renames the current window.                                                             |
| `lead` %                   | Splits the terminal horizontally into panes.                                            |
| `lead` "                   | Splits the terminal vertically into panes.                                              |
| `lead` q                   | Displays numbers for panes; press the number to switch to the corresponding pane.       |
| `lead` x                   | Closes the current pane.                                                                |
| `lead` c                   | Creates a new window.                                                                   |
| `lead` <arrow keys>        | Navigates between panes using arrow keys.                                               |
| `lead` n                   | Switches to the next window.                                                            |
| `lead` p                   | Switches to the previous window.                                                        |
| `lead` ]                   | Enters copy mode; use `space` to select text and `y` to copy.                           |



**Source:** [tmuxcheatsheet.com](https://tmuxcheatsheet.com/)


