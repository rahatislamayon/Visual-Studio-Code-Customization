# 🌟 My VS Code Settings & Extensions  

This repository contains my personal **Visual Studio Code settings** and a complete list of my installed **extensions**.  
It’s the quickest way to set up my preferred development environment on a new computer. 🚀  

---

## ⚙️ 1. VS Code Settings  

To apply my settings:  

1. Open **Visual Studio Code**.  
2. Press **Ctrl+Shift+P** (Windows/Linux) or **Cmd+Shift+P** (macOS) to open the **Command Palette**.  
3. Search for **“Open Settings (JSON)”** and select it.  
4. Copy everything from the [`settings.json`](.vscode/settings.json) file in this repo.  
5. Paste into your local `settings.json` (replacing existing content).  
6. Save and close the file. 🎉  

---

## 🧩 2. Extensions  

Here’s my full list of extensions. You can install them all at once with a single command.  

### 🔽 Installation Command  

```sh
code --install-extension GitHub.copilot \
--install-extension ms-vscode.cpptools \
--install-extension ms-vscode.cpptools-extension-pack \
--install-extension ms-vscode.cpptools-themes \
--install-extension twxs.cmake \
--install-extension ms-vscode.cmake-tools \
--install-extension formulahendry.code-runner \
--install-extension adpyke.codesnap \
--install-extension upstash.context7-mcp-server \
--install-extension ms-vscode.cpptools-debugger-java \
--install-extension alessandroguerriero.error-lens \
--install-extension redhat.java \
--install-extension google.gemini-cli-companion \
--install-extension google.gemini-code-assist \
--install-extension GitHub.copilot-chat \
--install-extension GitHub.vscode-pull-request-github \
--install-extension ms-vscode.vscode-gradle \
--install-extension oderwat.indent-rainbow \
--install-extension ms-vscode.vscode-intellicode \
--install-extension ms-vscode.vscode-intellicode-completions \
--install-extension Kilo-Code-AI.qodo-gen \
--install-extension redhat.vscode-languageserver-java \
--install-extension ms-vscode.live-preview \
--install-extension PKief.material-icon-theme \
--install-extension ms-vscode.maven \
--install-extension TechER.open-in-browser \
--install-extension vscjava.vscode-java-dependency \
--install-extension ms-python.vscode-pylance \
--install-extension ms-python.python \
--install-extension ms-python.debugpy \
--install-extension ms-python.python-environment-manager \
--install-extension ms-vscode.vscode-java-test








# ⚡ VS Code Setup Backup  

Easily restore my full **VS Code environment** (settings + extensions) on any computer.  
No need to start from scratch — just copy settings and reinstall extensions. 🚀  

---

## 🛠️ My VS Code Settings  

```json
{
    "code-runner.runInTerminal": true,
    "code-runner.saveFileBeforeRun": true,
    "workbench.startupEditor": "none",
    "explorer.confirmDelete": false,
    "C_Cpp.default.compilerPath": "",
    "tabnine.experimentalAutoImports": true,
    "debug.onTaskErrors": "debugAnyway",
    "editor.cursorSmoothCaretAnimation": "on",
    "security.workspace.trust.untrustedFiles": "open",
    "peacock.favoriteColors": [
        { "name": "Angular Red", "value": "#dd0531" },
        { "name": "Azure Blue", "value": "#007fff" },
        { "name": "JavaScript Yellow", "value": "#f9e64f" },
        { "name": "Mandalorian Blue", "value": "#1857a4" },
        { "name": "Node Green", "value": "#215732" },
        { "name": "React Blue", "value": "#61dafb" },
        { "name": "Something Different", "value": "#832561" },
        { "name": "Svelte Orange", "value": "#ff3d00" },
        { "name": "Vue Green", "value": "#42b883" }
    ],
    "window.titleBarStyle": "custom",
    "kilo-code.allowedCommands": [
        "npm test",
        "npm install",
        "tsc",
        "git log",
        "git diff",
        "git show"
    ],
    "editor.mouseWheelZoom": true,
    "terminal.integrated.fontSize": 17,
    "editor.cursorBlinking": "expand",
    "editor.wordWrap": "on",
    "workbench.colorTheme": "Default Dark+",
    "workbench.colorCustomizations": {},
    "window.controlsStyle": "custom",
    "editor.minimap.enabled": false,
    "git.autofetch": true,
    "editor.quickSuggestions": {
        "comments": "on",
        "strings": "inline"
    },
    "github.copilot.enable": {
        "*": true,
        "plaintext": true,
        "markdown": true,
        "scminput": true,
        "python": true
    },
    "editor.quickSuggestionsDelay": 5,
    "github.copilot.nextEditSuggestions.enabled": true,
    "animations.Install-Method": "Custom UI Style",
    "animations.Enabled": true,
    "animations.Command-Palette": "Slide",
    "workbench.iconTheme": "material-icon-theme",
    "redhat.telemetry.enabled": true,
    "git.confirmSync": false
}



