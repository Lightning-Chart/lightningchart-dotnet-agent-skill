# LightningChart .NET Agent Skill

An Agent Skill for building with LightningChart .NET accurately in AI coding
agents.

The skill teaches agents to start every LightningChart .NET task from the
official LLM-friendly documentation indexes, then follow the exact
task-specific documentation and API URLs found there. This helps prevent
hallucinated method names, stale package names, wrong option shapes, and API
patterns copied from unrelated charting libraries.

**For latest user guides on LightningChart .NET and AI, please refer to the [Developer Documentation](https://lightningchart.com/net-charts/docs/lightningChart-and-ai/)**

## Installation

Copy the `lightningchart-dotnet` folder into a skills directory supported by your
agent.

Project-local Agent Skills location:

```text
.agents/skills/lightningchart-dotnet/
```

OpenAI Codex local skills location:

```text
~/.codex/skills/lightningchart-dotnet/
```

Windows PowerShell example for Codex:

```powershell
Copy-Item -Recurse .\lightningchart-dotnet $env:USERPROFILE\.codex\skills\
```

VS Code and other Agent Skills compatible tools can also use this skill from a
project-local `.agents/skills/lightningchart-dotnet/` directory.

## Example Prompts

```text
Use $lightningchart-dotnet to add a XY-chart to this component.
```

```text
Use $lightningchart-dotnet to review this chart implementation for outdated or hallucinated LightingChart .NET APIs.
```

```text
Use $lightningchart-dotnet to migrate this existing chart to LightningChart .NET and verify the API usage with local type checks if possible.
```

That said, it seems that many agents are capable of automatically picking up locally installed skills even if your prompt doesn't explicitly mention them.

## License

This Agent Skill is licensed under the MIT License.

LightningChart .NET is separate proprietary software with its own licensing terms:
https://lightningchart.com/net-charts/
