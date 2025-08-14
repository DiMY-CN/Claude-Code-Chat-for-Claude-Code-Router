# Claude Code Chat for Claude Code Router
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Claude Code](https://img.shields.io/badge/Powered%20by-Claude%20Code-orange?style=for-the-badge)](https://claude.ai/code)
[![TypeScript](https://img.shields.io/badge/Built%20with-TypeScript-3178C6?style=for-the-badge&logo=typescript)](https://www.typescriptlang.org/)

A VSCode extension for Claude Code Chat, modified from [andrepimenta/claude-code-chat](https://github.com/andrepimenta/claude-code-chat), supporting invocation of Claude Code Router via [musistudio/claude-code-router](https://github.com/musistudio/claude-code-router), providing a more flexible code interaction experience.

🤖 **Built by Claude Code for Claude Code** - This extension was entirely developed using Claude Code itself. Claude Code created its own chat interface!
---

## Features

- Integrates Claude Code chat interface within VSCode  
- Supports Claude Code Router as the underlying model backend  
- Modified the original calls to Claude Code to adapt to Claude Code Router  
- Provides a user-friendly interface supporting code interaction and suggestions  
- Retains other features from [andrepimenta/claude-code-chat](https://github.com/andrepimenta/claude-code-chat)


---

## ✨ **Why Choose Claude Code Chat?**

🖥️ **No Terminal Required** - Beautiful chat interface replaces command-line interactions  
⏪ **Restore Checkpoints** - Undo changes and restore code to any previous state   
🔌 **MCP Server Support** - Complete Model Context Protocol server management   
💾 **Conversation History** - Automatic conversation history and session management  
🎨 **VS Code Native** - Claude Code integrated directly into VS Code with native theming and sidebar support  
🧠 **Plan and Thinking modes** - Plan First and configurable Thinking modes for better results  
⚡ **Smart File/Image Context and Custom Commands** - Reference any file, paste images or screenshots and create custom commands  
🤖 **Model Selection** - Choose between Opus, Sonnet, or Default based on your needs  
🐧 **Windows/WSL Support** - Full native Windows and WSL support

---

## Installation

1. Install prerequisites  
- Make sure [Claude Code](https://github.com/anthropics/claude-code) is installed  
- Ensure [Claude Code Router](https://github.com/musistudio/claude-code-router) is installed and configured  
- Download the .vsix file from the releases  
- Run `code --install-extension claude-code-chat-x.x.x.vsix`  

2. Open Claude Code Chat  
- Press `Ctrl+Shift+C` (or `Cmd+Shift+C` on Mac)  
- Or click the Claude icon in your status bar  
- Or use the Command Palette: type `Claude Code: Open Chat`

---

## Usage

- After starting the extension, the chat sidebar will open  
- Enter questions or code requests; the extension sends them to Claude Code Router and returns results  
- Supports multi-turn conversation for easier code debugging and coding assistance  
- You can adjust Claude Code Router access parameters in the extension settings

---

## Project Structure

- `src/` - extension source code  
- `package.json` - extension configuration and command definitions  
- `README.md` - project documentation  
- Other resources  

---

## Contributing

Contributions are welcome! Please submit issues and pull requests. Follow the code style guidelines.

---

## License

This project is licensed under the MIT License. See the LICENSE file for details.

---

## Related Links

- Claude Code Router Repository: [musistudio/claude-code-router](https://github.com/musistudio/claude-code-router)  
- Claude Code Chat Repository: [andrepimenta/claude-code-chat](https://github.com/andrepimenta/claude-code-chat)

---

## Contact

If you have any questions or suggestions, please open an issue or contact the maintainers.

---

Thank you for using this extension, and happy coding!
