<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width,initial-scale=1" />
<title>⚡ VS Code Setup Backup</title>
<style>
  :root{
    --bg:#0f1220; --panel:#171a2b; --panel-2:#1f2340; --text:#e7e9f5; --muted:#a7acc7;
    --brand:#7c5cff; --brand-2:#1ec8a5; --accent:#ff7b72; --border:#2a2e4a; --code:#0b0e1a;
    --link:#8ab4ff;
    --mono: ui-monospace, SFMono-Regular, Menlo, Consolas, "Liberation Mono", monospace;
    --round: 12px;
  }
  @media (prefers-color-scheme: light) {
    :root{ --bg:#f7f8fc; --panel:#ffffff; --panel-2:#f1f3fb; --text:#111; --muted:#5a5f7a; --border:#e6e8f2; --code:#0b1020; }
  }
  *{box-sizing:border-box}
  body{margin:0;background:linear-gradient(120deg,var(--bg),#0b0d18 60%);color:var(--text);font:16px/1.6 Inter,system-ui,Segoe UI,Roboto,Helvetica,Arial,sans-serif;}
  .wrap{max-width:1024px;margin:auto;padding:32px; }
  .hero{background:linear-gradient(135deg,var(--panel),var(--panel-2));border:1px solid var(--border);padding:28px;border-radius:18px;position:relative;overflow:hidden}
  .hero h1{margin:0 0 10px;font-size:28px;display:flex;gap:10px;align-items:center}
  .hero p{margin:0;color:var(--muted)}
  .badge-row{margin-top:16px;display:flex;flex-wrap:wrap;gap:10px}
  .badge{background:#1112;border:1px solid var(--border);color:var(--text);padding:6px 10px;border-radius:999px;font-size:12px}
  h2{margin-top:36px}
  section{background:linear-gradient(180deg,var(--panel),transparent);border:1px solid var(--border);padding:22px;border-radius:16px;margin-top:18px}
  .grid{display:grid;gap:18px}
  @media(min-width:880px){ .grid{grid-template-columns:2fr 1fr} }
  pre{background:#0b0f22;border:1px solid var(--border);border-radius:12px;padding:14px;overflow:auto}
  code{font-family:var(--mono);font-size:13px}
  .toolbar{display:flex;justify-content:space-between;align-items:center;margin-bottom:8px}
  .btn{border:1px solid var(--border);background:linear-gradient(180deg,var(--panel-2),var(--panel));color:var(--text);padding:8px 12px;border-radius:10px;cursor:pointer;font-weight:600}
  .btn.small{padding:6px 10px;font-size:12px}
  .btn.brand{border-color:#6f63ff;background:linear-gradient(180deg,#6f63ff20,#6f63ff10)}
  .btn:active{transform:translateY(1px)}
  table{width:100%;border-collapse:separate;border-spacing:0;overflow:hidden;border-radius:12px;border:1px solid var(--border)}
  th,td{padding:10px 12px;border-bottom:1px solid var(--border);text-align:left;font-size:14px}
  th{background:var(--panel-2)}
  tr:last-child td{border-bottom:0}
  a{color:var(--link);text-decoration:none}
  a:hover{text-decoration:underline}
  .paths{display:grid;gap:6px}
  .pill{display:inline-block;background:#1113;border:1px solid var(--border);padding:4px 8px;border-radius:8px;font-family:var(--mono);font-size:12px}
  .muted{color:var(--muted)}
  footer{opacity:.8;text-align:center;padding:24px 0}
</style>
</head>
<body>
<div class="wrap">

  <div class="hero">
    <h1>⚡ VS Code Setup Backup</h1>
    <p>Easily restore my entire <strong>VS Code environment</strong> — extensions, settings, and themes — on any computer.</p>
    <div class="badge-row">
      <span class="badge">AI&nbsp;Tools</span>
      <span class="badge">C++ / Java / Python</span>
      <span class="badge">GitHub &amp; Gradle/Maven</span>
      <span class="badge">Material Icons</span>
    </div>
  </div>

  <section id="install">
    <div class="toolbar">
      <h2>📦 Install All Extensions</h2>
      <button class="btn small brand" data-copy="#install-script">Copy Script</button>
    </div>
    <pre id="install-script"><code>code --install-extension GitHub.copilot \
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
--install-extension ms-vscode.vscode-java-test</code></pre>
    <p class="muted">Tip: Paste into your terminal after installing VS Code.</p>
  </section>

  <section id="links">
    <h2>🔗 Extensions (with Marketplace Links)</h2>
    <table>
      <thead>
        <tr><th>Extension</th><th>Identifier</th><th>Link</th></tr>
      </thead>
      <tbody>
        <tr><td>GitHub Copilot</td><td><code>GitHub.copilot</code></td><td><a href="https://marketplace.visualstudio.com/items?itemName=GitHub.copilot" target="_blank" rel="noopener">Marketplace</a></td></tr>
        <tr><td>C/C++</td><td><code>ms-vscode.cpptools</code></td><td><a href="https://marketplace.visualstudio.com/items?itemName=ms-vscode.cpptools" target="_blank" rel="noopener">Marketplace</a></td></tr>
        <tr><td>C/C++ Extension Pack</td><td><code>ms-vscode.cpptools-extension-pack</code></td><td><a href="https://marketplace.visualstudio.com/items?itemName=ms-vscode.cpptools-extension-pack" target="_blank" rel="noopener">Marketplace</a></td></tr>
        <tr><td>C/C++ Themes</td><td><code>ms-vscode.cpptools-themes</code></td><td><a href="https://marketplace.visualstudio.com/items?itemName=ms-vscode.cpptools-themes" target="_blank" rel="noopener">Marketplace</a></td></tr>
        <tr><td>CMake</td><td><code>twxs.cmake</code></td><td><a href="https://marketplace.visualstudio.com/items?itemName=twxs.cmake" target="_blank" rel="noopener">Marketplace</a></td></tr>
        <tr><td>CMake Tools</td><td><code>ms-vscode.cmake-tools</code></td><td><a href="https://marketplace.visualstudio.com/items?itemName=ms-vscode.cmake-tools" target="_blank" rel="noopener">Marketplace</a></td></tr>
        <tr><td>Code Runner</td><td><code>formulahendry.code-runner</code></td><td><a href="https://marketplace.visualstudio.com/items?itemName=formulahendry.code-runner" target="_blank" rel="noopener">Marketplace</a></td></tr>
        <tr><td>CodeSnap</td><td><code>adpyke.codesnap</code></td><td><a href="https://marketplace.visualstudio.com/items?itemName=adpyke.codesnap" target="_blank" rel="noopener">Marketplace</a></td></tr>
        <tr><td>Context7 MCP Server</td><td><code>upstash.context7-mcp-server</code></td><td><a href="https://marketplace.visualstudio.com/items?itemName=upstash.context7-mcp-server" target="_blank" rel="noopener">Marketplace</a></td></tr>
        <tr><td>C/C++ Debugger (Java)</td><td><code>ms-vscode.cpptools-debugger-java</code></td><td><a href="https://marketplace.visualstudio.com/items?itemName=ms-vscode.cpptools-debugger-java" target="_blank" rel="noopener">Marketplace</a></td></tr>
        <tr><td>Error Lens</td><td><code>alessandroguerriero.error-lens</code></td><td><a href="https://marketplace.visualstudio.com/items?itemName=alessandroguerriero.error-lens" target="_blank" rel="noopener">Marketplace</a></td></tr>
        <tr><td>Language Support for Java™ by Red Hat</td><td><code>redhat.java</code></td><td><a href="https://marketplace.visualstudio.com/items?itemName=redhat.java" target="_blank" rel="noopener">Marketplace</a></td></tr>
        <tr><td>Gemini CLI Companion</td><td><code>google.gemini-cli-companion</code></td><td><a href="https://marketplace.visualstudio.com/items?itemName=google.gemini-cli-companion" target="_blank" rel="noopener">Marketplace</a></td></tr>
        <tr><td>Gemini Code Assist</td><td><code>google.gemini-code-assist</code></td><td><a href="https://marketplace.visualstudio.com/items?itemName=google.gemini-code-assist" target="_blank" rel="noopener">Marketplace</a></td></tr>
        <tr><td>GitHub Copilot Chat</td><td><code>GitHub.copilot-chat</code></td><td><a href="https://marketplace.visualstudio.com/items?itemName=GitHub.copilot-chat" target="_blank" rel="noopener">Marketplace</a></td></tr>
        <tr><td>GitHub Pull Requests and Issues</td><td><code>GitHub.vscode-pull-request-github</code></td><td><a href="https://marketplace.visualstudio.com/items?itemName=GitHub.vscode-pull-request-github" target="_blank" rel="noopener">Marketplace</a></td></tr>
        <tr><td>Gradle for Java</td><td><code>ms-vscode.vscode-gradle</code></td><td><a href="https://marketplace.visualstudio.com/items?itemName=ms-vscode.vscode-gradle" target="_blank" rel="noopener">Marketplace</a></td></tr>
        <tr><td>Indent Rainbow</td><td><code>oderwat.indent-rainbow</code></td><td><a href="https://marketplace.visualstudio.com/items?itemName=oderwat.indent-rainbow" target="_blank" rel="noopener">Marketplace</a></td></tr>
        <tr><td>IntelliCode</td><td><code>ms-vscode.vscode-intellicode</code></td><td><a href="https://marketplace.visualstudio.com/items?itemName=ms-vscode.vscode-intellicode" target="_blank" rel="noopener">Marketplace</a></td></tr>
        <tr><td>IntelliCode Completions</td><td><code>ms-vscode.vscode-intellicode-completions</code></td><td><a href="https://marketplace.visualstudio.com/items?itemName=ms-vscode.vscode-intellicode-completions" target="_blank" rel="noopener">Marketplace</a></td></tr>
        <tr><td>Qodo Gen (Kilo Code AI)</td><td><code>Kilo-Code-AI.qodo-gen</code></td><td><a href="https://marketplace.visualstudio.com/items?itemName=Kilo-Code-AI.qodo-gen" target="_blank" rel="noopener">Marketplace</a></td></tr>
        <tr><td>Java Language Server (Red Hat)</td><td><code>redhat.vscode-languageserver-java</code></td><td><a href="https://marketplace.visualstudio.com/items?itemName=redhat.vscode-languageserver-java" target="_blank" rel="noopener">Marketplace</a></td></tr>
        <tr><td>Live Preview</td><td><code>ms-vscode.live-preview</code></td><td><a href="https://marketplace.visualstudio.com/items?itemName=ms-vscode.live-preview" target="_blank" rel="noopener">Marketplace</a></td></tr>
        <tr><td>Material Icon Theme</td><td><code>PKief.material-icon-theme</code></td><td><a href="https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme" target="_blank" rel="noopener">Marketplace</a></td></tr>
        <tr><td>Maven for Java</td><td><code>ms-vscode.maven</code></td><td><a href="https://marketplace.visualstudio.com/items?itemName=ms-vscode.maven" target="_blank" rel="noopener">Marketplace</a></td></tr>
        <tr><td>Open in Browser</td><td><code>TechER.open-in-browser</code></td><td><a href="https://marketplace.visualstudio.com/items?itemName=TechER.open-in-browser" target="_blank" rel="noopener">Marketplace</a></td></tr>
        <tr><td>Project Manager for Java</td><td><code>vscjava.vscode-java-dependency</code></td><td><a href="https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-java-dependency" target="_blank" rel="noopener">Marketplace</a></td></tr>
        <tr><td>Pylance</td><td><code>ms-python.vscode-pylance</code></td><td><a href="https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance" target="_blank" rel="noopener">Marketplace</a></td></tr>
        <tr><td>Python</td><td><code>ms-python.python</code></td><td><a href="https://marketplace.visualstudio.com/items?itemName=ms-python.python" target="_blank" rel="noopener">Marketplace</a></td></tr>
        <tr><td>Debugpy</td><td><code>ms-python.debugpy</code></td><td><a href="https://marketplace.visualstudio.com/items?itemName=ms-python.debugpy" target="_blank" rel="noopener">Marketplace</a></td></tr>
        <tr><td>Python Environment Manager</td><td><code>ms-python.python-environment-manager</code></td><td><a href="https://marketplace.visualstudio.com/items?itemName=ms-python.python-environment-manager" target="_blank" rel="noopener">Marketplace</a></td></tr>
        <tr><td>Test Runner for Java</td><td><code>ms-vscode.vscode-java-test</code></td><td><a href="https://marketplace.visualstudio.com/items?itemName=ms-vscode.vscode-java-test" target="_blank" rel="noopener">Marketplace</a></td></tr>
      </tbody>
    </table>
    <p class="muted">All links go straight to the official VS Code Marketplace.</p>
  </section>

  <section id="settings" class="grid">
    <div>
      <div class="toolbar">
        <h2>⚙️ settings.json</h2>
        <button class="btn small" data-copy="#settings-json">Copy JSON</button>
      </div>
      <pre id="settings-json"><code>{
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
}</code></pre>
    </div>
    <div>
      <h2>🧭 Restore Guide</h2>
      <ol>
        <li>Install <strong>Visual Studio Code</strong>.</li>
        <li>Run the extension install script above.</li>
        <li>Copy <code>settings.json</code> to:</li>
      </ol>
      <div class="paths">
        <div><span class="pill">Windows</span> <code>%APPDATA%\Code\User\settings.json</code></div>
        <div><span class="pill">macOS</span> <code>~/Library/Application Support/Code/User/settings.json</code></div>
        <div><span class="pill">Linux</span> <code>~/.config/Code/User/settings.json</code></div>
      </div>
      <p class="muted" style="margin-top:10px">Restart VS Code for all changes to take effect.</p>
      <h3>✨ Features</h3>
      <ul>
        <li><strong>AI assistance</strong>: GitHub Copilot &amp; Copilot Chat, Gemini</li>
        <li><strong>Language stacks</strong>: C/C++, Java (Gradle/Maven), Python</li>
        <li><strong>Utilities</strong>: Code Runner, Error Lens, CodeSnap, Indent Rainbow, Live Preview</li>
        <li><strong>Visuals</strong>: Material Icon Theme + Peacock color set</li>
      </ul>
    </div>
  </section>

  <footer>
    <small class="muted">Cross-platform • Minimal steps • Easily portable</small>
  </footer>
</div>

<script>
  // Simple copy-to-clipboard
  document.querySelectorAll('[data-copy]').forEach(btn=>{
    btn.addEventListener('click',()=>{
      const target = document.querySelector(btn.getAttribute('data-copy'));
      if(!target) return;
      const text = target.innerText;
      navigator.clipboard.writeText(text).then(()=>{
        const prev = btn.textContent;
        btn.textContent = 'Copied ✓';
        setTimeout(()=>btn.textContent = prev, 1200);
      });
    });
  });
</script>
</body>
</html>
