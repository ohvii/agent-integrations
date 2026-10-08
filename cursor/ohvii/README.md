# Ohvii for Cursor and Grok Bot

<!-- approved-about:start -->
Buy a California home through the AI you already use. Research homes, compare sales and review disclosures, then prepare offers and counters. Generate purchase agreements, addenda and repair requests, and track deadlines with guidance through closing. You choose the terms, review documents, sign securely and approve delivery. Requires a free Ohvii account.
<!-- approved-about:end -->

## Connect

1. Install the Ohvii plugin when it is available in your host's marketplace.
2. Open the Ohvii MCP connection and use the host's browser sign-in flow.
3. Sign in to your free Ohvii account at `ohvii.com` and review the requested permissions.
4. Return to your AI and start with one of the prompts below.

The connection uses `https://ohvii.com/api/mcp`. OAuth keeps credentials out of chat and plugin files. Transaction support is for self-represented California buyers. You choose terms, review documents, sign securely and approve delivery. You can also use [Ohvii directly](https://ohvii.com).

If your host cannot render an Ohvii card, review the tool results in the conversation and use the focused secure Ohvii link for signing or other required handoffs. Do not paste passwords, access tokens or signing links into public messages.

## Try asking

<!-- approved-prompts:start -->
- “Help me find homes that fit my budget and what I’m looking for.”
- “Compare recent sales so I can decide what to offer for this home.”
- “Review this home’s disclosures, explain the risks, and help me plan inspections or repair requests.”
- “Help me prepare an offer for this home.”
- “Help me evaluate this counteroffer and prepare a response.”
- “What do I need to complete before closing, and what’s due next?”
<!-- approved-prompts:end -->

## Local review

Copy this directory into `~/.cursor/plugins/local/ohvii`, then restart Cursor or run **Developer: Reload Window**. Open **Customize** to verify the Ohvii skill and MCP server. Complete OAuth before requesting account data. The repository root's `.cursor-plugin/marketplace.json` points to this package at `cursor/ohvii`.

This package contains a skill, an HTTPS MCP configuration and Ohvii artwork. It runs no local shell commands, hooks or executable dependencies. The hosted service remains separate from the public package.

## Publication status

This is the first Cursor / Grok Bot marketplace candidate, version `1.0.0`. Publication requires provider review. The Cursor Marketplace Team confirmed on October 8, 2026 that its publisher application covers Cursor and Grok Bot. This does not list Ohvii in regular Grok chat's public connector catalog or the separate Grok Build catalog. Local package checks do not establish a complete buyer workflow in either host.

## Support and policies

- [Setup and tool reference](https://ohvii.com/developers)
- [Support](https://ohvii.com/support)
- [Privacy policy](https://ohvii.com/privacy)
- [Service terms](https://ohvii.com/terms)

Connector source, manifests, skills and setup documentation use the [MIT license](LICENSE). [Ohvii artwork](assets/NOTICE.md) has separate permissions. The hosted application, backend and buyer data are outside this repository and license.
