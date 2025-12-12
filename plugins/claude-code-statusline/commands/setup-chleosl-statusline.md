Update ~/.claude/settings.json to configure the statusLine setting as follows:

  ```json
  "statusLine": {
    "type": "command",
    "command": "~/.claude/plugins/marketplaces/claude-code-statusline-chleosl/plugins/claude-code-statusline/statusline.sh",
    "padding": 0
  }

If statusLine doesn't exist, add it. If it exists, replace it with the above configuration.
