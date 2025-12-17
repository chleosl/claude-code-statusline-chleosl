Toggle the statusline extra info (weather, cwd, and git info on main).

Run this command to toggle:
```bash
STATUSLINE_SH="$HOME/.claude/plugins/concise-statusline-chleosl/statusline.sh"
if [ ! -f "$STATUSLINE_SH" ]; then
    echo "Error: statusline.sh not found at $STATUSLINE_SH"
    exit 1
fi
current=$(grep -oP 'show_extra="\K(on|off)' "$STATUSLINE_SH")
if [ "$current" = "on" ]; then
    sed -i 's/show_extra="on"/show_extra="off"/' "$STATUSLINE_SH"
    echo "Statusline extra info: OFF"
else
    sed -i 's/show_extra="off"/show_extra="on"/' "$STATUSLINE_SH"
    echo "Statusline extra info: ON"
fi
```
