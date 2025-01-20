
# Tmux Cheatsheet (Prefix: Ctrl + x)

## Managing Tabs (Windows)
- **New Tab (Window):** `Ctrl + x, c` - Creates a new tab/window.
- **Switch to Next Tab:** `Ctrl + x, n` - Moves to the next tab/window.
- **Switch to Previous Tab:** `Ctrl + x, p` - Moves to the previous tab/window.
- **Go to Tab (By Index):** `Ctrl + x, <Number>` - Switches to the tab/window with the specified number.
- **List Tabs:** `Ctrl + x, w` - Lists all tabs/windows.
- **Rename Tab:** `Ctrl + x, ,` - Renames the current tab/window.
- **Close Tab:** `Ctrl + x, &` - Closes the current tab/window.

## Managing Panes
- **Horizontal Split:** `Ctrl + x, "` - Splits the pane horizontally.
- **Vertical Split:** `Ctrl + x, %` - Splits the pane vertically.
- **Switch Between Panes:** `Ctrl + x, o` - Moves to the next pane.
- **Rotate Panes:** `Ctrl + x, Ctrl + o` - Rotates panes within the window.
- **Resize Pane:** `Ctrl + x, <Arrow>` - Resizes the pane in the arrow's direction.
- **Close Pane:** `Ctrl + x, x` - Closes the current pane.

## Sessions
- **Detach from Session:** `Ctrl + x, d` - Detaches from the current session.
- **List Sessions:** `tmux list-sessions` - Lists all active sessions.
- **Attach to Session:** `tmux attach-session` - Re-attaches to a specific session.

## Copy and Paste
- **Enter Copy Mode:** `Ctrl + x, [` - Enters scrollback mode to copy text.
- **Scroll in Copy Mode:** `Up/Down` - Scroll up or down.
- **Start Selection:** `Space` - Begins selecting text.
- **Copy Selection:** `Enter` - Copies the selected text.
- **Paste:** `Ctrl + x, ]` - Pastes the copied text.

---

# Installing Tmux

1. **Update your system:**
   ```
   sudo apt update && sudo apt upgrade
   ```

2. **Install Tmux:**
   ```
   sudo apt install tmux
   ```

3. **Verify Installation:**
   ```
   tmux -V
   ```

---

# Downloading and Installing Fonts (Fira Code and Cascadia Code)

## Fira Code
1. **Download Fira Code:**
   - Visit the official GitHub repository: https://github.com/tonsky/FiraCode
   - Download the latest `.ttf` files from the `distr/ttf` folder.

2. **Install Fira Code on Linux:**
   ```
   mkdir -p ~/.local/share/fonts
   cp /path/to/downloaded/fonts/*.ttf ~/.local/share/fonts
   fc-cache -fv
   ```

## Cascadia Code
1. **Download Cascadia Code:**
   - Visit the official GitHub repository: https://github.com/microsoft/cascadia-code
   - Download the latest `.ttf` files from the releases section.

2. **Install Cascadia Code on Linux:**
   ```
   mkdir -p ~/.local/share/fonts
   cp /path/to/downloaded/fonts/*.ttf ~/.local/share/fonts
   fc-cache -fv
   ```

---

Reload Tmux and set the font in your terminal to Fira Code or Cascadia Code for best results.
