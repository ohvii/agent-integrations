# Ohvii for OpenClaw

<!-- approved-about:start -->
Buy a California home through the AI you already use. Research homes, compare sales and review disclosures, then prepare offers and counters. Generate purchase agreements, addenda and repair requests, and track deadlines with guidance through closing. You choose the terms, review documents, sign securely and approve delivery. Requires a free Ohvii account.
<!-- approved-about:end -->

This plugin connects OpenClaw to the hosted Ohvii service and includes the buyer workflow skill. It requires a free Ohvii account. Transaction support is for self-represented California buyers.

## Install

Install the published plugin from [ClawHub](https://clawhub.ai/ohvii/plugins/ohvii):

```sh
openclaw plugins install clawhub:@ohvii/ohvii --accept-capabilities
openclaw plugins inspect ohvii
```

The plugin includes the Ohvii MCP connection, buyer workflow skill and logo. Start the OpenClaw Gateway and open its Control UI. If the Ohvii plugin detail page shows **Accounts → Connect**, use it to authorize the connection. Complete Ohvii sign-in and review the permissions in your browser, then return to OpenClaw and verify **Connected**. Reload or restart an existing agent session. Never paste credentials or bearer tokens into chat or configuration.

If Accounts is absent, as observed with this local plugin on OpenClaw 2026.9.8, use the supported CLI setup:

```sh
openclaw mcp add ohvii --url https://ohvii.com/api/mcp --transport streamable-http --auth oauth
openclaw mcp login ohvii
openclaw mcp probe ohvii
```

This explicit server configuration overrides the same named plugin declaration; it does not create a second server. `mcp login` and `mcp list` require that explicit configuration in the tested release.

Use a current OpenClaw release supporting plugin-bundled HTTP MCP and OAuth. Installation and tool discovery alone do not establish a successful buyer workflow.

## Start a conversation

<!-- approved-prompts:start -->
- “Help me find homes that fit my budget and what I’m looking for.”
- “Compare recent sales so I can decide what to offer for this home.”
- “Review this home’s disclosures, explain the risks, and help me plan inspections or repair requests.”
- “Help me prepare an offer for this home.”
- “Help me evaluate this counteroffer and prepare a response.”
- “What do I need to complete before closing, and what’s due next?”
<!-- approved-prompts:end -->

Your AI supplies the conversation and its available research capabilities. Ohvii keeps the saved transaction, documents, permissions and history. Review the AI's sources and conclusions. Consequential actions require the current prepared details and your separate approval; signing uses a secure Ohvii handoff. Planned closing dates and third-party messages do not establish completed closing or possession. Ohvii does not move money or act as your licensed buyer's agent.

The initial package uses structured tools and secure browser handoffs. It does not claim verified inline MCP App rendering in OpenClaw.

## Access and data

OAuth can request workspace, research and document access, draft/document edits, offer confirmation, communications sending and transaction confirmation. Review the scopes shown during connection. Connecting does not sign documents or approve delivery. Disconnect access through Ohvii's connected-agent settings and remove the saved connection through OpenClaw's account controls.

Buyer data stays in the authorized Ohvii account. Your chosen AI provider also receives the information supplied to its conversation and tools under that provider's terms. The package contains no buyer records or credentials and does not bundle the Ohvii server.

## Support

- [Ohvii](https://ohvii.com)
- [Connection and tool reference](https://ohvii.com/developers)
- [Support](https://ohvii.com/support)
- [Privacy](https://ohvii.com/privacy)
- [Terms](https://ohvii.com/terms)

Release `1.0.2`: descriptions now explicitly identify the required Ohvii account as free. Native OAuth and the shared buyer workflow are unchanged.

## License

The connector source, manifest, bundled buyer skill and setup documentation use
the [MIT license](LICENSE). [Bundled artwork](assets/NOTICE.md) has separate
permissions. The hosted Ohvii application, backend and buyer data are not part of
this source release. Using the service requires your authorized Ohvii account
and remains subject to its terms.

This is a native plugin package. A separate ClawHub skill-registry publication
would require that registry's MIT-0 terms and is not included in this release.
