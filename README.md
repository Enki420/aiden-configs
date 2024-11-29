AIDEN Platform Configs
AIDEN Mode
To set up a custom sync link for the AIDEN Platform, follow these steps:

Step 1: Open the settings (on macOS: cmd+,, on Windows: ctrl+,)
Step 2: Locate and edit the URL in the Mode Sync field.
Step 3: Click the Sync button to start synchronizing data.
[!NOTE]
Your custom URL will not be overwritten during updates. If you plan to use your own URL as a data source, ensure it follows the data format in aiden.mode.json.

Sync URL
AIDEN Platform Configs: A collection of AI tools, development platforms, and other resources (e.g., ChatGPT, Gemini, Copilot, Figma, Discord, etc.).


https://raw.githubusercontent.com/ENKI420/aiden-configs/main/aiden.mode.json
Data Format: aiden.mode.json
Below is a detailed description of the configuration file fields:

name: The name of the configuration set (optional, purely for display purposes).
version: The version of the configuration file (used for updates).
sync: The URL where the configuration file is hosted (optional, for reference).
modes[]: Contains individual entries for tools or folders:
id: A unique identifier for the entry (use a format like aiden:xxx or aiden@xxx for consistency).
parent: Indicates the parent folder for this entry (supports nesting).
text: The display name of the tool or folder.
url: The link to the tool or resource (optional for folders).
dir: Specifies whether the entry is a folder (true or false).
Proxy
To configure proxies for the AIDEN Platform, refer to the Electron documentation.

proxyRules: Defines which proxies to use for network requests.
proxyBypassRules: Specifies URLs that bypass proxy settings.
Customizations
Ensure your configuration file follows the above structure and upload it to a publicly accessible URL.
Update the Mode Sync URL in your AIDEN Platform settings to point to your custom file.
For example:

bash
Copy code
https://raw.githubusercontent.com/ENKI420/YourRepo/main/custom.mode.json
Let me know if you need further enhancements or additional examples!
