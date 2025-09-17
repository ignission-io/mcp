<img src="https://ignission.io/ignission-logo.png" alt="Ignission logo" width="100"/>

# Ignission MCP

Tools for content creators and businesses on TikTok

## About this MCP Server

Ignission is a tool kit for content creators and businesses on TikTok.

## Installation Guide

<details>
<summary>Cursor</summary>

#### One-click installation:

[![Add to Cursor](https://cursor.com/deeplink/mcp-install-dark.svg)](cursor://anysphere.cursor-deeplink/mcp/install?name=ignission&config=eyJ1cmwiOiJodHRwczovL21jcC5pZ25pc3Npb24uaW8vbWNwIn0%3D)

#### Manual steps:

- Go to **Settings > Cursor Settings > Tools & Integrations**
- Under **MCP tools**, click **Add Custom MCP**
- Paste the configuration below into **mcp.json**
- Save the file to apply the configuration
- Restart **Cursor** if prompted

#### Configuration:

```json
{
  "mcpServers": {
    "ignission": {
      "url": "https://mcp.ignission.io/mcp"
    }
  }
}
```

</details>
<details>
<summary>VS Code</summary>

#### One-click installation:

[![Install in VS Code](https://img.shields.io/badge/VS_Code-Install_Server-0098FF?style=for-the-badge&logo=visual-studio-code&logoColor=white)](https://insiders.vscode.dev/redirect?url=vscode:mcp/install?%7B%22type%22%3A%22http%22%2C%22name%22%3A%22ignission%22%2C%22version%22%3A%220.0.1%22%2C%22description%22%3A%22Tools%20for%20content%20creators%20and%20businesses%20on%20TikTok%22%2C%22url%22%3A%22https%3A%2F%2Fmcp.ignission.io%2Fmcp%22%2C%22author%22%3A%22Ignission%22%2C%22tags%22%3A%5B%22ignission%22%2C%22mcp%22%2C%22server%22%5D%2C%22categories%22%3A%5B%22mcp%22%5D%7D)

Click on **Install** to complete the setup.


#### Manual steps:

Use the command line:

```bash
code --add-mcp '{"type":"http","name":"ignission","version":"0.0.1","description":"Tools for content creators and businesses on TikTok","url":"https://mcp.ignission.io/mcp","author":"Ignission","tags":["ignission","mcp","server"],"categories":["mcp"]}'
```


Then go to **Extensions**, find the **Ignission** MCP server in the list, open the menu with right-click and click on **Start Server**.

</details>
<details>
<summary>Claude Desktop</summary>


  ### Manual steps

**1. Make sure Node.js is installed**

In your terminal, check if Node.js is installed on your system by running:

```bash
node -v
```

If Node.js isn't installed, download it from [nodejs.org](https://nodejs.org).


**2. Configure Claude Desktop**

- Go to **Settings > Developer**
- Click **Edit config** to open the **claude_desktop_config.json** file
- Add the MCP server configuration to the **mcpServers** section
- Paste the configuration below
- Save the file to apply the configuration
- Restart Claude Desktop

#### Configuration:

```json
{
  "mcpServers": {
    "ignission": {
      "command": "npx",
      "args": [
        "mcp-remote",
        "https://mcp.ignission.io/mcp"
      ]
    }
  }
}
```

</details>
<details>
<summary>Claude Teams</summary>

### Manual steps

_Note: Only workspace owners and admins have permission to add custom connectors_

- Navigate to **Settings > Connectors**
- Toggle to **Organization connectors** at the top of the page
- At the bottom of the page, click on **Add custom connector** and fill the following information:
  - Name: `ignission`
  - Remote MCP server URL: `https://mcp.ignission.io/mcp`
- Click **Add** to finish the setup


</details>
<details>
<summary>OpenAI ChatGPT</summary>

#### Manual steps:

<div class="markdown-alert markdown-alert-important">
  <div class="markdown-alert-title">IMPORTANT</div>
  <div>For now MCP servers are only supported in ChatGPT Plus and Pro versions</div>
</div>

- Navigate to **Settings > Connectors**
- Scroll down and click on **Advanced Settings**
- Enable **Developer mode**
- Go back to the **Settings > Connectors** page, and click on **Create** in the **Browser Connectors** section
- You can now add a custom connector with the server URL: `https://mcp.ignission.io/mcp`
- In the Description field, add the server description: `Tools for content creators and businesses on TikTok`
- click on **Create** to add the MCP server as a Connector


Now, to use the connector in a new chat, just click on **+ > More** and enable the **Developer mode**. This will create a new tab in the chat bar called **Add Sources** where you now should see our MCP server listed.




</details>
<details>
<summary>Claude Code</summary>

#### Manual steps:

Use the command line to add the MCP server:

```bash
claude mcp add --transport http ignission https://mcp.ignission.io/mcp
```


The server should now be available in Claude Code. You should see it by using `claude /mcp` command

</details>
<details>
<summary>Cline</summary>

#### Manual steps:

- Click on the **Cline** icon in the VSCode sidebar
- Click on the **MCP Servers** tab
- Click on the **Remote Servers** tab
- Fill in the required information:
  - Server Name: `ignission`
  - Server URL: `https://mcp.ignission.io/mcp`
- Click **Add Server** to initiate the connection
- Cline will attempt to connect to the server and display the connection status
- If the connection is successful, click on **Done**


</details>
<details>
<summary>Goose</summary>

  #### One-click installation:
  [![Install in Goose](https://block.github.io/goose/img/extension-install-dark.svg)](goose://extension?id=ignission&name=Ignission&description=Tools+for+content+creators+and+businesses+on+TikTok&url=https%3A%2F%2Fmcp.ignission.io%2Fmcp&type=streamable_http)
  #### Manual steps:

- Go to **Extensions**
- Click on **Add custom extension**
- Fill the following information:
  - Extension Name: `ignission`
  - Type: `Streamable HTTP`
  - Description: `Tools for content creators and businesses on TikTok`
  - Endpoint: `https://mcp.ignission.io/mcp`


- Click **Add Extension** to finish the setup

</details>

---

Thank you!


*These installation instructions were generated by the [MCP Install Instructions Generator](https://mcp-install-instructions.alpic.cloud/) by [Alpic.ai](https://alpic.ai)*
