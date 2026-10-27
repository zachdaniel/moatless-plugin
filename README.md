# Moatless for Claude Code

[Moatless](https://moatless.store) is a marketplace for codebases. Sellers list a codebase with a one-time price, and optionally a subscription for updates that's only charged in months with a new release. Buyers get it as a git repository, and updates arrive as commits that merge into their own changes.

This plugin connects Claude Code to Moatless, so your agent can do it for you:

- **Buy:** search for codebases, compare them, clone the ones you've bought, and pull their updates.
- **Sell:** turn a repository into a listing, with a description, screenshots, and releases, and keep it up to date. You review and publish it on the website.

## Install

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

## What's included

- The Moatless MCP server (`https://moatless.store/mcp`), with tools for searching, buying, cloning, listing, releasing, and reviewing codebases. You sign in with OAuth, and the agent acts as you.
- A skill that tells your agent how to work with Moatless. It reads the current guide from Moatless each time, so it stays up to date without reinstalling.

Your agent can't pay for anything. When you decide to buy a codebase, it gives you the checkout link to open in your browser.

## Links

- [Moatless](https://moatless.store)
- [How selling works](https://moatless.store/sell/how-it-works)
- [Privacy Policy](https://moatless.store/privacy) and [Terms of Service](https://moatless.store/terms)
- [Contact](https://moatless.store/contact)
