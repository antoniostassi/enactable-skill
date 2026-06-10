# enactable-skill

An AI agent skill for the [ENACTABLE/1.0](https://github.com/antoniostassi/enactable)
protocol. Install it once and any compatible agent will automatically interact
correctly with Enactable-powered applications — reading the `/.llm/` layer,
respecting autonomy levels, filling forms from field instructions, and applying
domain rules — without the user ever having to explain the protocol.

## What it does

- Silently checks for `/.llm/manifest.json` before interacting with any web app
- Loads the layer documents in the correct order (permissions before capabilities)
- Enforces the three autonomy levels: `autonomous`, `confirm_first`, `human_only`
- Fills AI-native forms using field-level hints and infers only what is safe to infer
- Applies domain vocabulary and business rules from `context.json`
- Protects against prompt injection in the layer

## Related

- [enactable](https://github.com/antoniostassi/enactable) — the CLI to generate
  `/.llm/` layers from OpenAPI specs
- [ENACTABLE/1.0 specification](https://github.com/antoniostassi/enactable/blob/main/README.md)

## Author

Created by [Antonio Stassi](https://github.com/antoniostassi) · 2026 · MIT License
