# Ohvii agent integrations

Buy a California home through the AI you already use. Research homes, compare sales and review disclosures, then prepare offers and counters. Generate purchase agreements, addenda and repair requests, and track deadlines with guidance through closing. You choose the terms, review documents, sign securely and approve delivery.

This repository contains the connector packages and buyer workflow instructions for the hosted Ohvii service. Transaction support is for self-represented California buyers.

| Client | Setup | Distribution status |
| --- | --- | --- |
| OpenClaw | [Plugin and connection setup](openclaw/ohvii/README.md) | [Published on ClawHub](https://clawhub.ai/ohvii/plugins/ohvii) |
| Hermes | [Connection and companion skill](hermes/ohvii/README.md) | [Catalog PR submitted](https://github.com/NousResearch/hermes-agent/pull/134371); awaiting Nous review |

The first OpenClaw release was `1.0.0`; the current source prepares its `1.0.1` copy update. The Hermes catalog candidate remains `1.0.0`. Source availability is separate from marketplace approval. The clients use OAuth to connect to `https://ohvii.com/api/mcp`; sign in through the native flow and review the requested permissions.

## License and service

Exported connector source, manifests, skills and setup documentation are covered by the [scoped MIT license](LICENSE). [Ohvii artwork](openclaw/ohvii/assets/NOTICE.md) has separate permissions. The hosted application, backend and buyer data are outside this repository and license. Service access requires an authorized Ohvii account and remains subject to [Ohvii terms](https://ohvii.com/terms).

## Support

- [Developer guide](https://ohvii.com/developers)
- [Support](https://ohvii.com/support)
- [Privacy](https://ohvii.com/privacy)
