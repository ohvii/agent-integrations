# Ohvii MCP Registry metadata

`server.json` describes the hosted Ohvii MCP service using its approved descriptions, six starter prompts, public support links and logo reference. It contains no application source, credentials or buyer records.

The metadata submitted to the [official MCP Registry](https://registry.modelcontextprotocol.io) is dedicated to CC0 under the [Registry terms](https://modelcontextprotocol.io/registry/terms-of-service). Referenced connector packages and artwork retain their own licenses.

The manually dispatched `Publish Ohvii to MCP Registry` workflow requires the SHA-256 of the exact owner-approved metadata. It validates the record, authenticates with the Ohvii repository's short-lived GitHub OIDC identity, publishes and compares the live record with the submitted content. It uses no stored publisher secret. Run it only for an approved release; published versions are immutable.

The canonical source is maintained with Ohvii's approved plugin copy and exported here after validation. Do not replace the wording during packaging or release work. A Registry record does not establish approval in another provider's curated marketplace or authenticated native-host compatibility.
