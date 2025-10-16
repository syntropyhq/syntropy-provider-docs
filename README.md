# Syntropy Provider Documentation

This repository contains curated documentation summaries for software vendors/providers that the Syntropy broker can help users with.

## Structure

- `providers/` - Individual provider documentation files
- `scripts/` - Instructions and tools for generating new provider docs

## Provider Documentation Format

Each provider doc should be a markdown file containing:

1. **Overview** - What the provider does, core value proposition
2. **Key Features** - Main capabilities and offerings
3. **Use Cases** - Common scenarios and applications
4. **Pricing** - Pricing model overview (tiers, free tier, enterprise)
5. **Integration** - How developers typically integrate (APIs, SDKs, platforms)
6. **Comparison Points** - Key differentiators vs alternatives
7. **Support & Resources** - Documentation, community, support channels

## Adding New Providers

See `scripts/generate-provider-doc.md` for instructions on generating new provider documentation.

## Usage

These docs are fetched by the Syntropy broker system via raw GitHub URLs:
```
https://raw.githubusercontent.com/YOUR_USERNAME/syntropy-provider-docs/main/providers/{provider-id}.md
```
