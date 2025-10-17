# Syntropy Provider Documentation

This repository contains curated documentation summaries for software vendors/providers that the Syntropy broker can help users with.

## Structure

- `providers/` - Individual provider documentation files
- `scripts/` - Instructions and tools for generating new provider docs

## Adding New Providers

See `scripts/generate-provider-doc.md` for instructions on generating new provider documentation.

## Usage

These docs are fetched by the Syntropy broker system via raw GitHub URLs:
```
https://raw.githubusercontent.com/YOUR_USERNAME/syntropy-provider-docs/main/providers/{provider-id}.md
```
