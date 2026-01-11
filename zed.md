```json
// Zed keymap
//
// For information on binding keys, see the Zed
// documentation: https://zed.dev/docs/key-bindings
//
// To see the default key bindings run `zed: open default keymap`
// from the command palette.
[
  {
    "context": "Workspace && vim_mode == normal",
    "bindings": {
      "space space": "file_finder::Toggle",
    },
  },
  {
    "context": "Editor && VimControl",
    "bindings": {
      "ctrl+h": "project_panel::ToggleFocus",
    },
  },
  {
    "context": "Editor && VimControl",
    "bindings": {
      "alt-k": "editor::MoveLineUp",
      "alt-j": "editor::MoveLineDown",
      "ctrl-h": "project_panel::ToggleFocus",
      "ctrl-l": "agent::ToggleFocus",
      "ctrl-j": "terminal_panel::Toggle",
      "shift-h": "pane::ActivatePreviousItem",
      "shift-l": "pane::ActivateNextItem",
    },
  },
  {
    "context": "ProjectPanel && !editing",
    "bindings": {
      "a": "project_panel::NewFile",
      "r": "project_panel::Rename",
      "d": "project_panel::Delete",
      "x": "project_panel::Cut",
      "y": "project_panel::Copy",
      "p": "project_panel::Paste",
      "ctrl-l": "project_panel::ToggleFocus",
    },
  },
  {
    "context": "Terminal",
    "bindings": {
      "ctrl-k": "terminal_panel::ToggleFocus",
    },
  },
  {
    "context": "AsistantPanel",
    "bindings": {},
  },
]
```