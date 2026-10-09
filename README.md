# Ohvii agent integrations

Buy a California home through the AI you already use. Research homes, compare sales and review disclosures, then prepare offers and counters. Generate purchase agreements, addenda and repair requests, and track deadlines with guidance through closing. You choose the terms, review documents, sign securely and approve delivery. Requires a free Ohvii account.

This repository contains the connector packages and buyer workflow instructions for the hosted Ohvii service. Transaction support is for self-represented California buyers.

| Client | Setup | Distribution status |
| --- | --- | --- |
| Cursor / Grok Bot | [Plugin and connection setup](cursor/ohvii/README.md) | Version `1.0.0` submitted October 8, 2026; awaiting provider review |
| OpenClaw | [Plugin and connection setup](openclaw/ohvii/README.md) | [Published on ClawHub](https://clawhub.ai/ohvii/plugins/ohvii) |
| Hermes | [Connection and companion skill](hermes/ohvii/README.md) | [Catalog PR submitted](https://github.com/NousResearch/hermes-agent/pull/134371); awaiting Nous review |
| Gemini CLI | [Extension and connection setup](https://github.com/ohvii/gemini-extension) | [Release 1.0.2 published](https://github.com/ohvii/gemini-extension/releases/tag/v1.0.2); Google gallery indexing not yet verified |

The current published OpenClaw release is `1.0.2`. The Hermes catalog candidate remains `1.0.0` and awaits upstream review. The clients use OAuth to connect to `https://ohvii.com/api/mcp`; sign in through the native flow and review the requested permissions.

The hosted service is also published in the [official MCP Registry](https://registry.modelcontextprotocol.io/?q=io.github.ohvii%2Fohvii) as `io.github.ohvii/ohvii` version `1.0.1`. See the [registry metadata and publication record](registry/README.md).

Gemini CLI requires supported business licensing or paid API access; Google directs consumer Google accounts to Antigravity CLI. See the linked Gemini setup guide for current account requirements. Gemini extension installation has been verified; authenticated buyer workflows and Antigravity compatibility remain unverified.

## License and service

Exported connector source, manifests, skills and setup documentation are covered by the [scoped MIT license](LICENSE). [Ohvii artwork](openclaw/ohvii/assets/NOTICE.md) has separate permissions. The hosted application, backend and buyer data are outside this repository and license. Service access requires an authorized Ohvii account and remains subject to [Ohvii terms](https://ohvii.com/terms).

## Support

- [Developer guide](https://ohvii.com/developers)
- [Support](https://ohvii.com/support)
- [Privacy](https://ohvii.com/privacy)
