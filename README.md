# Zed Editor Configuration

This file describes the settings used in the Zed editor for a simple and efficient experience.

## User Settings (`settings.json`)

```json
{// settings.json, generated at Thu Nov 07 2024 18:01:50 GMT+0800 (Singapore Standard Time)
// Zed settings
//
// For information on how to configure Zed, see the Zed
// documentation: https://zed.dev/docs/configuring-zed
//
// To see all of Zed's default settings without changing your
// custom settings, run the `open default settings` command
// from the command palette or from `Zed` application menu.
{
  "base_keymap": "VSCode",
  "theme": "Catppuccin Mocha",
  "ui_font_size": 16,
  "buffer_font_size": 16,
  // NOTE: Change the font family to your preference
  "buffer_font_family": "Hack Nerd Font Mono",
  "show_inline_completions": true,
  "auto_update_extensions": {
    "discord-presence": false
  },
  // Vim mode settings
  "vim_mode": true,
  // use relative line numbers
  "relative_line_numbers": true,
  "tab_bar": {
    "show": true
  },
  "scrollbar": {
    "show": "never"
  },
  // Indentation, rainbow indentation
  "indent_guides": {
    "enabled": true
  },
  // NOTE: Zen mode, refer https://github.com/zed-industries/zed/issues/4382 when it's resolved
  "centered_layout": {
    "left_padding": 0.15,
    "right_padding": 0.15
  },
  // Use Copilot Chat AI as default
  "assistant": {
    "default_model": {
      "provider": "copilot_chat",
      "model": "gpt-4o"
    },
    "version": "2"
  },
  // Uncomment below to use local AI with Ollama, refer https://zed.dev/docs/language-model-integration?highlight=ollama#using-ollama-on-macos
  // "assistant": {
  //   "default_model": {
  //     "provider": "ollama",
  //     "model": "llama3.1:latest"
  //   },
  //   "version": "2",
  //   "provider": null
  // },
  "language_models": {
    "ollama": {
      "api_url": "http://localhost:11434"
    }
  },
  // Inlay hints preconfigured by Zed: Go, Rust, Typescript and Svelte
  "inlay_hints": {
    "enabled": true
  },
  // LSP
  "lsp": {
    "vtsls": {
      "settings": {
        "typescript": {
          "tsdk": "/home/dinihz/.nvm/versions/node/v18.20.5/lib/node_modules/typescript/lib"
        }
      }
    }
  },
  "languages": {
    // Refer https://zed.dev/docs/languages/javascript and https://zed.dev/docs/languages/typescript for more info
    "TypeScript": {
      // Refer https://github.com/jellydn/ts-inlay-hints for how to setup for Neovim and VSCode
      "inlay_hints": {
        "enabled": true,
        "show_parameter_hints": false,
        "show_other_hints": true,
        "show_type_hints": true
      }
    },
    "Markdown": {
      "show_inline_completions": true
    }
  },
  // Use zed commit editor
  "terminal": {
    "env": {
      "EDITOR": "zed --wait"
    }
  },
  // File syntax highlighting
  "file_types": {
    "Dockerfile": ["Dockerfile", "Dockerfile.*"],
    "JSON": ["json", "jsonc", "*.code-snippets"]
  },
  // File scan exclusions, hide on the file explorer and search
  "file_scan_exclusions": [
    "**/.git",
    "**/.svn",
    "**/.hg",
    "**/CVS",
    "**/.DS_Store",
    "**/Thumbs.db",
    "**/.classpath",
    "**/.settings",
    // above is default from Zed
    "**/out",
    "**/dist",
    "**/.husky",
    "**/.turbo",
    "**/.vscode-test",
    "**/.vscode",
    "**/.next",
    "**/.storybook",
    "**/.tap",
    "**/.nyc_output",
    "**/report",
    "**/node_modules"
  ],
  // Turn off telemetry
  "telemetry": {
    "diagnostics": false,
    "metrics": false
  },
  // Move all panel to the right
  "project_panel": {
    "button": true,
    "dock": "right",
    "git_status": true
  },
  "outline_panel": {
    "dock": "right"
  },
  "collaboration_panel": {
    "dock": "left"
  },
  // Move some unnecessary panels to the left
  "notification_panel": {
    "dock": "left"
  },
  "chat_panel": {
    "dock": "left"
  }
}
}
```

## Keyboard Shortcuts (`keybindings.json`)

```json
// settings.json, generated at Thu Nov 07 2024 18:01:50 GMT+0800 (Singapore Standard Time)
// Zed settings
//
// For information on how to configure Zed, see the Zed
// documentation: https://zed.dev/docs/configuring-zed
//
// To see all of Zed's default settings without changing your
// custom settings, run the `open default settings` command
// from the command palette or from `Zed` application menu.
{
  "base_keymap": "VSCode",
  "theme": "Catppuccin Mocha",
  "ui_font_size": 16,
  "buffer_font_size": 16,
  // NOTE: Change the font family to your preference
  "buffer_font_family": "Hack Nerd Font Mono",
  "show_inline_completions": true,
  "auto_update_extensions": {
    "discord-presence": false
  },
  // Vim mode settings
  "vim_mode": true,
  // use relative line numbers
  "relative_line_numbers": true,
  "tab_bar": {
    "show": true
  },
  "scrollbar": {
    "show": "never"
  },
  // Indentation, rainbow indentation
  "indent_guides": {
    "enabled": true
  },
  // NOTE: Zen mode, refer https://github.com/zed-industries/zed/issues/4382 when it's resolved
  "centered_layout": {
    "left_padding": 0.15,
    "right_padding": 0.15
  },
  // Use Copilot Chat AI as default
  "assistant": {
    "default_model": {
      "provider": "copilot_chat",
      "model": "gpt-4o"
    },
    "version": "2"
  },
  // Uncomment below to use local AI with Ollama, refer https://zed.dev/docs/language-model-integration?highlight=ollama#using-ollama-on-macos
  // "assistant": {
  //   "default_model": {
  //     "provider": "ollama",
  //     "model": "llama3.1:latest"
  //   },
  //   "version": "2",
  //   "provider": null
  // },
  "language_models": {
    "ollama": {
      "api_url": "http://localhost:11434"
    }
  },
  // Inlay hints preconfigured by Zed: Go, Rust, Typescript and Svelte
  "inlay_hints": {
    "enabled": true
  },
  // LSP
  "lsp": {
    "vtsls": {
      "settings": {
        "typescript": {
          "tsdk": "/home/dinihz/.nvm/versions/node/v18.20.5/lib/node_modules/typescript/lib"
        }
      }
    }
  },
  "languages": {
    // Refer https://zed.dev/docs/languages/javascript and https://zed.dev/docs/languages/typescript for more info
    "TypeScript": {
      // Refer https://github.com/jellydn/ts-inlay-hints for how to setup for Neovim and VSCode
      "inlay_hints": {
        "enabled": true,
        "show_parameter_hints": false,
        "show_other_hints": true,
        "show_type_hints": true
      }
    },
    "Markdown": {
      "show_inline_completions": true
    }
  },
  // Use zed commit editor
  "terminal": {
    "env": {
      "EDITOR": "zed --wait"
    }
  },
  // File syntax highlighting
  "file_types": {
    "Dockerfile": ["Dockerfile", "Dockerfile.*"],
    "JSON": ["json", "jsonc", "*.code-snippets"]
  },
  // File scan exclusions, hide on the file explorer and search
  "file_scan_exclusions": [
    "**/.git",
    "**/.svn",
    "**/.hg",
    "**/CVS",
    "**/.DS_Store",
    "**/Thumbs.db",
    "**/.classpath",
    "**/.settings",
    // above is default from Zed
    "**/out",
    "**/dist",
    "**/.husky",
    "**/.turbo",
    "**/.vscode-test",
    "**/.vscode",
    "**/.next",
    "**/.storybook",
    "**/.tap",
    "**/.nyc_output",
    "**/report",
    "**/node_modules"
  ],
  // Turn off telemetry
  "telemetry": {
    "diagnostics": false,
    "metrics": false
  },
  // Move all panel to the right
  "project_panel": {
    "button": true,
    "dock": "right",
    "git_status": true
  },
  "outline_panel": {
    "dock": "right"
  },
  "collaboration_panel": {
    "dock": "left"
  },
  // Move some unnecessary panels to the left
  "notification_panel": {
    "dock": "left"
  },
  "chat_panel": {
    "dock": "left"
  }
}
```

### Keep these settings updated to ensure maximum productivity with Zed!
