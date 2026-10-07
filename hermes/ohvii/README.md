# Ohvii for Hermes

<!-- approved-about:start -->
Buy a California home through the AI you already use. Research homes, compare sales and review disclosures, then prepare offers and counters. Generate purchase agreements, addenda and repair requests, and track deadlines with guidance through closing. You choose the terms, review documents, sign securely and approve delivery.
<!-- approved-about:end -->

Connect Hermes to the hosted Ohvii MCP service using your Ohvii account. Transaction support is for self-represented California buyers. The catalog submission is pending; this package does not claim Nous approval.

## Connect before catalog publication

```sh
hermes mcp add ohvii --url https://ohvii.com/api/mcp --auth oauth
hermes mcp login ohvii
hermes mcp test ohvii
```

Complete sign-in and review Ohvii's requested permissions in your browser. Never paste tokens, cookies or authorization codes into a conversation or replace OAuth with a static bearer header. Restart the Hermes session or reload MCP after connecting.

Use an up-to-date Hermes client. If the browser reports success but Hermes times out without saving credentials, update Hermes to include its [OAuth callback fix](https://github.com/NousResearch/hermes-agent/commit/74ddb737ca5c668dd04393acb1d43659d164fbfa), then retry login.

The accompanying `skills/ohvii/SKILL.md` is the shared text-client buyer workflow. Install it into your chosen Hermes profile's `skills/ohvii/` directory, then start a new conversation. The MCP catalog entry itself configures the connection; it does not silently install this skill.

After a catalog PR is accepted and included in your Hermes installation, `hermes mcp install ohvii` will become the catalog setup route. Until then, use the direct OAuth command above.

## Start a conversation

<!-- approved-prompts:start -->
- “Help me find homes that fit my budget and what I’m looking for.”
- “Compare recent sales so I can decide what to offer for this home.”
- “Review this home’s disclosures, explain the risks, and help me plan inspections or repair requests.”
- “Help me prepare an offer for this home.”
- “Help me evaluate this counteroffer and prepare a response.”
- “What do I need to complete before closing, and what’s due next?”
<!-- approved-prompts:end -->

Use the connected account's current records. Your AI prepares research and drafts; you choose terms, review documents, sign securely and separately approve consequential actions. Signing uses a focused Ohvii browser handoff. Do not treat messages or future dates as proof of seller agreement, closing or possession. Ohvii does not move money or act as your licensed buyer's agent.

This package targets structured tools and secure browser handoffs. Inline MCP App rendering is not claimed. A successful connection probe does not prove a completed buyer workflow.

## Access and support

OAuth can request workspace, research and document access, draft/document edits, offer confirmation, communications sending and transaction confirmation. Review the scopes during connection. Remove access in Ohvii's connected-agent settings; removing a local server definition alone is not server-side revocation.

The connector contains no buyer records or credentials. Your AI provider receives the information used in its conversation under its own terms.

- [Ohvii](https://ohvii.com)
- [Connection and tool reference](https://ohvii.com/developers)
- [Support](https://ohvii.com/support)
- [Privacy](https://ohvii.com/privacy)
- [Terms](https://ohvii.com/terms)

Release `1.0.0`: initial catalog candidate and shared buyer workflow.

## License

The catalog manifest, companion buyer skill and setup documentation use the
[MIT license](LICENSE). The hosted Ohvii application, backend and buyer data are
not part of this source release. Using the service requires your authorized
Ohvii account and remains subject to its terms. The catalog manifest is offered
to Hermes under its MIT contribution terms.
