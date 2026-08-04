# Skills for oleander

Forkable skills repository for teams using [oleander.dev](https://oleander.dev/).

Use this repo to store reusable skills, connect to the MCP, and install the oleander CLI to get the most capabile local experience for oleander.

## Quick start

```bash
git clone https://github.com/oleanderHQ/skills.git
cd oleander-spark
```

## Install via skills

You can install skills from the published repository on [skills.sh](https://skills.sh/) using:

```bash
npx skills add oleanderHQ/skills
```

## Install the oleander CLI

Install with Homebrew:

```bash
brew tap OleanderHQ/tap
brew install oleander-cli
```

Configure with your API key:

```bash
oleander configure --api-key <YOUR_API_KEY>
```

You can find your API key in [oleander settings](https://oleander.dev/app/settings/api-key).

## MCP

### Cursor

```bash
agent mcp add oleander -- npx -y mcp-remote https://oleander.dev/api/mcp
```

Verify:

```bash
agent mcp list
```

Alternative config in `.cursor/mcp.json`:

```json
{
  "mcpServers": {
    "oleander": {
      "command": "npx",
      "args": [
        "-y",
        "mcp-remote",
        "https://oleander.dev/api/mcp"
      ]
    }
  }
}
```

### Claude Code

```bash
claude mcp add oleander -- npx -y mcp-remote https://oleander.dev/api/mcp
```

Verify:

```bash
claude mcp list
```

## Included Skills

- `skills/spark-best-practices`
- `skills/oleander-spark-lineage`
- `skills/oleander-iceberg-catalog`
- `skills/oleander-spark-submit`
- `skills/oleander-mcp-queries`

## Contributing

External contributors are welcome.

- Open a PR with clear context
- A contribution is considered approved and official only after review, approval, and merge by an oleander employee.

See `CONTRIBUTING.md` for details.

## License

MIT. See `LICENSE`.
