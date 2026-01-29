---
name: rest-to-graphql
description: Convert REST API routes to GraphQL schema. Use when migrating APIs.
---

# REST to GraphQL Converter

Migrating REST to GraphQL means mapping endpoints to queries and mutations. This tool reads your REST routes and generates a GraphQL schema.

**One command. Zero config. Just works.**

## Quick Start

```bash
npx ai-rest-to-graphql ./src/routes/
```

## What It Does

- Reads REST route definitions
- Maps to GraphQL types and resolvers
- Handles relationships and nesting
- Generates complete schema

## Usage Examples

```bash
# Convert routes
npx ai-rest-to-graphql ./src/routes/

# Single file
npx ai-rest-to-graphql ./routes/users.ts -o schema.graphql
```

## Best Practices

- **Think in graphs** - relationships, not endpoints
- **Batch similar endpoints** - users and user/:id become one query
- **Use proper types** - not everything is a String
- **Add descriptions** - GraphQL schemas are self-documenting

## When to Use This

- Migrating REST API to GraphQL
- Creating GraphQL layer over REST
- Learning GraphQL schema design
- Quick prototyping

## Part of the LXGIC Dev Toolkit

This is one of 110+ free developer tools built by LXGIC Studios. No paywalls, no sign-ups, no API keys on free tiers. Just tools that work.

**Find more:**
- GitHub: https://github.com/LXGIC-Studios
- Twitter: https://x.com/lxgicstudios
- Substack: https://lxgicstudios.substack.com
- Website: https://lxgicstudios.com

## Requirements

No install needed. Just run with npx. Node.js 18+ recommended. Needs OPENAI_API_KEY environment variable.

```bash
npx ai-rest-to-graphql --help
```

## How It Works

Parses your REST route files to understand endpoints and response shapes. Then maps them to GraphQL types, queries, and mutations following best practices.

## License

MIT. Free forever. Use it however you want.
