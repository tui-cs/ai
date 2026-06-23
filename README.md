# ai

A [Terminal.Gui](https://github.com/tui-cs/Terminal.Gui) inline-mode CLI powered by the [GitHub Copilot SDK](https://www.nuget.org/packages/GitHub.Copilot.SDK).

## Features

- **Interactive chat mode** — multi-turn conversation with streaming markdown rendering
- **Single-turn mode** — pipe a prompt and get a streamed answer inline
- **Slash commands** — `/help`, `/clear`, `/model <name>`, `/compact`, `/quit`
- **Autocomplete** — tab-completion for slash commands
- **Model switching** — change models mid-conversation with `/model`

## Prerequisites

- [.NET 10 SDK](https://dotnet.microsoft.com/download/dotnet/10.0)
- [GitHub Copilot CLI](https://docs.github.com/en/copilot) installed and authenticated

## Install

```bash
dotnet tool install -g Terminal.Gui.ai
```

## Usage

```bash
# Interactive chat mode
ai

# Single-turn mode
ai "Explain async/await in C#"

# Specify a model
ai -m gpt-4o "What is Terminal.Gui?"
```

## Slash Commands

| Command | Description |
|---|---|
| `/help` | Show available commands |
| `/clear` | Clear conversation history |
| `/model <name>` | Switch to a different model |
| `/compact` | Summarize conversation |
| `/quit` | Exit chat |

## License

[MIT](LICENSE)
