# Claude Code Integration

This folder contains configuration for [Claude Code](https://claude.ai/code) integration with the Conversion Blueprints knowledge base.

## Quick Start

When you open this repository in Claude Code, the custom commands become available automatically.

## Available Commands

| Command | Purpose | Example |
|---------|---------|---------|
| `/audit-page` | Audit a page against best practices | `/audit-page landing-page https://example.com` |
| `/benchmark` | Get conversion benchmarks | `/benchmark saas` |
| `/checklist` | Generate a build/review checklist | `/checklist homepage ecommerce` |
| `/pattern` | Find a specific pattern | `/pattern hero` |

## How It Works

1. **Commands** (`commands/*.md`) define slash commands that Claude Code recognizes
2. **Settings** (`settings.json`) configure permissions and behavior
3. **CLAUDE.md** (root) provides overall context about the repository

## Usage Examples

### Auditing a Landing Page
```
/audit-page landing-page "B2B SaaS signup page with hero, features, and pricing"
```

### Getting Benchmarks
```
/benchmark trial-to-paid
```

### Building a New Page
```
/checklist pricing saas
```

### Understanding a Pattern
```
/pattern social-proof
```

## Extending

To add new commands:
1. Create a new `.md` file in `commands/`
2. Follow the format of existing commands
3. Document usage and examples

## Requirements

- Claude Code CLI or IDE extension
- This repository cloned or opened as context

## More Info

- [Claude Code Documentation](https://docs.anthropic.com/claude-code)
- [Conversion Blueprints README](../README.md)
- [CLAUDE.md](../CLAUDE.md) - AI context reference
