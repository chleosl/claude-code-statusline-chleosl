# Claude Code Statusline

Custom statusline for Claude Code CLI.

## Features

- Session stats (lines added/removed)
- Git diff stats (unstaged + staged changes)
- Context window usage with gradient progress bar
- Token count with color coding
- Current git branch and last commit
- Weather info with temperature-based coloring
- Current time with timezone

## Output Format

```
Line 1: +added/-removed (session) +added/-removed (git) | usage% [progress] (tokens) | time
Line 2: branch last_commit_hash last_commit_message
Line 3: location: temp condition icon
Line 4: current_working_directory
```

## Progress Indicator States

The progress bar uses a gradient color scheme (gray → red) that cycles twice per 10%:

```
_   _   _   _   _   ▯   ▯   ▯   ▯   ▯
0   1   2   3   4   5   6   7   8   9
```

## Installation

```bash
/plugin install claude-code-statusline@chleosl
```

![Claude Statusline Overview](./assets/claude_statusline_overview.png)
