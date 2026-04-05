# Rangoon Hub

Public registry for [Rangoon](https://github.com/jeremytoce/rangoon-cli) skills, MCP servers, agent templates, and powerpacks.

## Structure

```
catalog.json          # Registry index (fetched by the Hub)
skills/               # Skill markdown files
  {skill-id}.md       # Individual skill content
```

## Usage

Add this registry to your `rangoon.json`:

```json
{
  "registries": [
    {
      "url": "https://raw.githubusercontent.com/jeremytoce/rangoon-hub/main",
      "name": "rangoon"
    }
  ]
}
```

Then open the Hub in your Rangoon dashboard to browse and install skills.

## Contributing

Submit a PR with your skill file in `skills/` and an entry in `catalog.json`.
