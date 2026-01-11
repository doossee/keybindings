```json
// Place your key bindings in this file to override the defaults
[
  // ============================================
  // EDITOR NAVIGATION & ACTIONS
  // ============================================

  // Quick Open (Vim Normal Mode)
  {
    "key": "space space",
    "command": "workbench.action.quickOpen",
    "when": "editorTextFocus && vim.mode == 'Normal'"
  },

  // Move Lines Up/Down
  {
    "key": "alt+k",
    "command": "editor.action.moveLinesUpAction",
    "when": "editorTextFocus"
  },
  {
    "key": "alt+j",
    "command": "editor.action.moveLinesDownAction",
    "when": "editorTextFocus"
  },

  // Navigate Between Tabs (Vim Style)
  {
    "key": "shift+h",
    "command": "workbench.action.previousEditor",
    "when": "editorTextFocus && vim.active && vim.mode == 'Normal'"
  },
  {
    "key": "shift+l",
    "command": "workbench.action.nextEditor",
    "when": "editorTextFocus && vim.active && vim.mode == 'Normal'"
  },

  // ============================================
  // PANEL NAVIGATION
  // ============================================

  // Focus File Explorer from Editor
  {
    "key": "ctrl+h",
    "command": "workbench.files.action.focusFilesExplorer",
    "when": "editorTextFocus"
  },

  // Toggle Terminal
  {
    "key": "ctrl+j",
    "command": "workbench.action.terminal.toggleTerminal",
    "when": "editorTextFocus"
  },
  {
    "key": "ctrl+l",
    "command": "workbench.action.focusActiveEditorGroup",
    "when": "filesExplorerFocus"
  },

  // ============================================
  // FILE EXPLORER (VIM-STYLE)
  // ============================================

  // New File
  {
    "key": "a",
    "command": "explorer.newFile",
    "when": "filesExplorerFocus && !inputFocus"
  },

  // Rename
  {
    "key": "r",
    "command": "renameFile",
    "when": "filesExplorerFocus && !inputFocus"
  },

  // Delete
  {
    "key": "d",
    "command": "deleteFile",
    "when": "filesExplorerFocus && !inputFocus"
  },

  // Cut
  {
    "key": "x",
    "command": "filesExplorer.cut",
    "when": "filesExplorerFocus && !inputFocus"
  },

  // Copy (Yank)
  {
    "key": "y",
    "command": "filesExplorer.copy",
    "when": "filesExplorerFocus && !inputFocus"
  },

  // Paste
  {
    "key": "p",
    "command": "filesExplorer.paste",
    "when": "filesExplorerFocus && !inputFocus"
  },

  // ============================================
  // ANTIGRAVITY AGENT PANEL
  // ============================================

  // Focus Editor from Agent Panel
  {
    "key": "ctrl+h",
    "command": "workbench.action.focusActiveEditorGroup",
    "when": "antigravity.agentPanel.active && !editorTextFocus"
  },

  // Open Agent Chat
  {
    "key": "ctrl+l",
    "command": "antigravity.prioritized.chat.open",
    "when": "!terminalFocus && !filesExplorerFocus"
  },

  // Disable default Agent Chat binding
  {
    "key": "ctrl+l",
    "command": "-antigravity.prioritized.chat.open",
    "when": "!terminalFocus"
  }
]
```