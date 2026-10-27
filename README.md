# Moatless for coding agents

[Moatless](https://moatless.store/?utm_source=moatless-plugin&utm_medium=readme) is a marketplace for codebases. Sellers list a codebase with a one-time price, and optionally a subscription for updates that's only charged in months with a new release. Buyers get it as a git repository, and updates arrive as commits that merge into their own changes.

This connects your coding agent to Moatless, so it can do it for you:

- **Buy:** search for codebases, compare them, clone the ones you've bought, and pull their updates.
- **Sell:** turn a repository into a listing, with a description, screenshots, and releases, and keep it up to date. You review and publish it on the website.

[![Add to Cursor](https://cursor.com/deeplink/mcp-install-dark.svg)](https://cursor.com/en/install-mcp?name=moatless&config=eyJ1cmwiOiJodHRwczovL21vYXRsZXNzLnN0b3JlL21jcCJ9)
[![Install in VS Code](https://img.shields.io/badge/VS_Code-Install_MCP_server-0098FF)](https://insiders.vscode.dev/redirect/mcp/install?name=moatless&config=%7B%22type%22%3A%22http%22%2C%22url%22%3A%22https%3A%2F%2Fmoatless.store%2Fmcp%22%7D)

## Install in Claude Code

The plugin includes the MCP server and a skill:

```
/plugin marketplace add zachdaniel/moatless-plugin
/plugin install moatless@moatless
```

Or from a shell:

```
claude plugin marketplace add zachdaniel/moatless-plugin
claude plugin install moatless@moatless
```

Then run `/mcp`, choose `moatless`, and sign in to Moatless in your browser.

To add only the MCP server, without the skill:

```
claude mcp add --transport http moatless https://moatless.store/mcp
```

## Install in other clients

Use the buttons above for Cursor and VS Code. Anywhere else, add the server by its URL. It's remote (Streamable HTTP), and you sign in with OAuth in your browser, so there's no API key to paste:

```json
{
  "mcpServers": {
    "moatless": {
      "url": "https://moatless.store/mcp"
    }
  }
}
```

## What's included

- The Moatless MCP server (`https://moatless.store/mcp`), with tools for searching, buying, cloning, listing, releasing, and reviewing codebases. You sign in with OAuth, and the agent acts as you.
- In Claude Code, a skill that tells your agent how to work with Moatless. It reads the current guide from Moatless each time, so it stays up to date without reinstalling. In other clients, the server's `guide` tool gives the agent the same guide.

Your agent can't pay for anything. When you decide to buy a codebase, it gives you the checkout link to open in your browser.

## Links

- [Moatless](https://moatless.store/?utm_source=moatless-plugin&utm_medium=readme)
- [How selling works](https://moatless.store/sell/how-it-works?utm_source=moatless-plugin&utm_medium=readme)
- [Privacy Policy](https://moatless.store/privacy) and [Terms of Service](https://moatless.store/terms)
- [Contact](https://moatless.store/contact)
