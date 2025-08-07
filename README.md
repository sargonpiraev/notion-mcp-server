# Notion API MCP Server 🔧

![npm version](https://img.shields.io/npm/v/@sargonpiraev/notion-mcp-server)
![npm downloads](https://img.shields.io/npm/dw/@sargonpiraev/notion-mcp-server)
![license](https://img.shields.io/github/license/sargonpiraev/notion-mcp-server)
![pipeline status](https://gitlab.com/sargonpiraev/notion-mcp-server/badges/main/pipeline.svg)
![smithery badge](https://smithery.ai/badge/@sargonpiraev/notion-mcp-server)
![MCP Compatible](https://img.shields.io/badge/MCP-Compatible-blue)
[![Join Discord](https://img.shields.io/discord/1331631275464671347?color=7289da&label=Discord&logo=discord)](https://discord.gg/ZsWGxRGj)

## Features

- 🔌 **Seamless AI Integration**: Direct Notion API API access from Claude, Cursor, and VS Code
- 🤖 **Automated Workflows**: Automate Notion API operations and data access
- 📊 **Complete API Coverage**: 19+ tools covering all major Notion API features
- ⚡ **Real-time Access**: Access Notion API data instantly from AI assistants
- 🔧 **Professional Integration**: Error handling, validation, and comprehensive logging

## Get Your Credentials

Before installation, you'll need a Notion API API key:

1. Open Notion API app or web interface
2. Go to **Settings → Account → API Access**
3. Generate new API key or copy existing one
4. Save this key for the installation steps below

## Requirements

- Node.js >= v18.0.0
- Notion API API key
- Cursor, VS Code, Claude Desktop or another MCP Client

## Installation

<details>
<summary><b>Installing via Smithery</b></summary>

To install Notion API MCP Server for any client automatically via [Smithery](https://smithery.ai):

```bash
npx -y @smithery/cli@latest install @sargonpiraev/notion-mcp-server --client <CLIENT_NAME>
```

</details>

<details>
<summary><b>Install in Cursor</b></summary>

#### Cursor One-Click Installation

[![Install MCP Server](https://cursor.com/deeplink/mcp-install-dark.svg)](https://cursor.com/install-mcp?name=@sargonpiraev/notion-mcp-server&config=eyJjb21tYW5kIjoibnB4IiwiYXJncyI6WyIteSIsIkBzYXJnb25waXJhZXYvbm90aW9uLW1jcC1zZXJ2ZXIiXSwiZW52Ijp7Ik5PVElPTl9BUElfVE9LRU4iOiJ5b3VyX25vdGlvbl9hcGlfdG9rZW5faGVyZSJ9fQ==)

#### Manual Configuration

Add to your Cursor `~/.cursor/mcp.json` file:

```json
{
  "mcpServers": {
    "notion-mcp-server": {
      "command": "npx",
      "args": ["-y", "@sargonpiraev/notion-mcp-server"],
      "env": {
        "NOTION_API_TOKEN": "your-notion_api_token"
      }
    }
  }
}
```

</details>

<details>
<summary><b>Install in VS Code</b></summary>

[![Install in VS Code](https://img.shields.io/badge/VS_Code-Install_MCP-0098FF)](vscode:mcp/install?%7B%22name%22%3A%22notion-mcp-server%22%2C%22command%22%3A%22npx%22%2C%22args%22%3A%5B%22-y%22%2C%22@sargonpiraev/notion-mcp-server%22%5D%7D)

Or add manually to your VS Code settings:

```json
"mcp": {
  "servers": {
    "notion-mcp-server": {
      "type": "stdio",
      "command": "npx",
      "args": ["-y", "@sargonpiraev/notion-mcp-server"],
      "env": {
        "NOTION_API_TOKEN": "your-notion_api_token"
      }
    }
  }
}
```

</details>

<details>
<summary><b>Install in Claude Desktop</b></summary>

Add to your `claude_desktop_config.json`:

```json
{
  "mcpServers": {
    "notion-mcp-server": {
      "command": "npx",
      "args": ["-y", "@sargonpiraev/notion-mcp-server"],
      "env": {
        "NOTION_API_TOKEN": "your-notion_api_token"
      }
    }
  }
}
```

</details>

## Available Tools

- **`get-user`**: Retrieve a user
- **`get-users`**: List all users
- **`get-self`**: Retrieve your token&#x27;s bot user
- **`post-database-query`**: Query a database
- **`post-search`**: Search by title
- **`get-block-children`**: Retrieve block children
- **`patch-block-children`**: Append block children
- **`retrieve-a-block`**: Retrieve a block
- **`update-a-block`**: Update a block
- **`delete-a-block`**: Delete a block
- **`retrieve-a-page`**: Retrieve a page
- **`patch-page`**: Update page properties
- **`post-page`**: Create a page
- **`create-a-database`**: Create a database
- **`update-a-database`**: Update a database
- **`retrieve-a-database`**: Retrieve a database
- **`retrieve-a-page-property`**: Retrieve a page property item
- **`retrieve-a-comment`**: Retrieve comments
- **`create-a-comment`**: Create comment

**Total: 19 tools available** 🎯

## Support This Project

Hi! I'm Sargon, a software engineer passionate about AI tools and automation. I create open-source MCP servers to help developers integrate AI assistants with their favorite services.

Your support helps me continue developing and maintaining these tools, and motivates me to create new integrations that make AI assistants even more powerful! 🚀

[![Support on Boosty](https://img.shields.io/badge/Support-Boosty-orange?logo=data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjQiIGhlaWdodD0iMjQiIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHBhdGggZD0iTTEyIDJMMTMuMDkgOC4yNkwyMCA5TDEzLjA5IDE1Ljc0TDEyIDIyTDEwLjkxIDE1Ljc0TDQgOUwxMC45MSA4LjI2TDEyIDJaIiBmaWxsPSJ3aGl0ZSIvPgo8L3N2Zz4K)](https://boosty.to/sargonpiraev)

## Connect with Author

- 🌐 Visit [sargonpiraev.com](https://sargonpiraev.com)
- 📧 Email: [sargonpiraev@gmail.com](mailto:sargonpiraev@gmail.com)
- 💬 Join [Discord](https://discord.gg/ZsWGxRGj)
