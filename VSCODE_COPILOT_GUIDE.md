# VS Code GitHub Copilot Configuration

## Claude Sonnet Setup Guide

This repository includes VS Code settings to enable Claude 3.5 Sonnet as an available model in GitHub Copilot.

### Prerequisites

1. **GitHub Copilot Subscription**: Ensure you have an active GitHub Copilot subscription with access to premium models
2. **VS Code with GitHub Copilot Extension**: Install the latest version of the GitHub Copilot extension from the VS Code marketplace

### Using Claude Sonnet

The `.vscode/settings.json` file in this repository is pre-configured to enable Claude 3.5 Sonnet. When you open this workspace in VS Code:

1. The settings will automatically be applied to your workspace
2. Open the GitHub Copilot chat panel (usually accessible via the sidebar or with `Ctrl+Shift+I` / `Cmd+Shift+I`)
3. Look for the model selector (typically at the top of the chat panel)
4. You should now see "claude-3.5-sonnet" as an available option
5. Select Claude Sonnet from the dropdown menu

### Troubleshooting

**Issue**: "I don't see Claude Sonnet as an option"
- **Solution**: Verify your GitHub Copilot subscription includes access to premium models
- Check that your GitHub Copilot extension is up to date
- Reload VS Code after opening this workspace

**Issue**: "I'm being asked for API keys when clicking Anthropic"
- **Solution**: This configuration uses GitHub's built-in integration with Anthropic. You should NOT need separate API keys
- Ensure you're using the GitHub Copilot chat interface, not a separate Anthropic extension
- Verify that your GitHub organization has enabled premium model access

**Issue**: "The model selector doesn't show Claude Sonnet"
- **Solution**: Make sure the workspace settings are loaded by:
  1. Opening the Command Palette (`Ctrl+Shift+P` / `Cmd+Shift+P`)
  2. Running "Preferences: Open Workspace Settings (JSON)"
  3. Verifying the settings from `.vscode/settings.json` are present
  4. Reloading the VS Code window

### Configuration Details

The settings in `.vscode/settings.json` enable:

- `github.copilot.chat.models.claude-3.5-sonnet.enabled`: Explicitly enables Claude 3.5 Sonnet
- `github.copilot.advanced.anthropicEnabled`: Enables Anthropic models integration through GitHub

### Additional Resources

- [GitHub Copilot Documentation](https://docs.github.com/en/copilot)
- [VS Code GitHub Copilot Extension](https://marketplace.visualstudio.com/items?itemName=GitHub.copilot)
