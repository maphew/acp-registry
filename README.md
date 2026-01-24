# ACP Registry

> ⚠️ **Work in Progress**: This registry is under active development. Format and contents may change.

A registry of agents and extensions implementing the [Agent Client Protocol, ACP](https://github.com/agentclientprotocol/agent-client-protocol).

> **Note**: This registry only includes agents that support [authentication](AUTHENTICATION.md). Agents must implement auth flows to be listed here. See also the [ACP auth methods proposal](https://github.com/agentclientprotocol/agent-client-protocol/blob/main/docs/rfds/auth-methods.mdx).

## Included Agents

| Agent                                                                       | Description                                                                       |
|-----------------------------------------------------------------------------|-----------------------------------------------------------------------------------|
| [Auggie CLI](https://github.com/augmentcode/auggie-zed-extension)           | Augment Code's powerful software agent, backed by industry-leading context engine |
| [Codex CLI](https://github.com/zed-industries/codex-acp)                    | ACP adapter for OpenAI's coding assistant                                         |
| Factory Droid                                                               | Factory Droid - AI coding agent powered by Factory AI                             |
| [Gemini CLI](https://github.com/google-gemini/gemini-cli)                   | Google's official CLI for Gemini                                                  |
| [GitHub Copilot](https://github.com/github/copilot-language-server-release) | GitHub's AI pair programmer                                                       |
| [Mistral Vibe](https://github.com/mistralai/mistral-vibe)                   | Mistral's open-source coding assistant                                            |
| [OpenCode](https://github.com/sst/opencode)                                 | The open source coding agent                                                      |
| [Qwen Code](https://github.com/QwenLM/qwen-code)                            | Alibaba's Qwen coding assistant                                                   |

## Usage

Fetch the registry index:

```
https://github.com/agentclientprotocol/registry/releases/latest/download/registry.json
```

## Documentation Site

Generate the agents list and run the local docs server:

```bash
uv run .github/workflows/generate_mintlify_agents.py
cd docs && npx mintlify dev --port 3000
```

## Registry Format

See [FORMAT.md](FORMAT.md) for the registry schema, distribution types, and platform targets.

## Adding an Agent or Extension

See [CONTRIBUTING.md](CONTRIBUTING.md) for instructions.

## License

This registry is licensed under the [Apache License 2.0](LICENSE). Individual agents are subject to their own licenses.
