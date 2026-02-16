# AeonSage Documentation

This directory contains the official AeonSage documentation content, designed to be integrated into the existing website at `apps/website/`.

---

## About AeonSage

AeonSage is a self-hosted AI orchestration platform that connects language models, messaging channels, and real-world tools. Run entirely on your infrastructure with complete control over your data.

### Editions

| Edition | License | Best For |
|---------|---------|----------|
| **OSS** | MIT | Individuals, developers, self-hosters |
| **Pro** | Commercial | Teams, organizations, power users |

### OSS Repository

The open-source repository is available at: [github.com/velonone/Aeonsage](https://github.com/velonone/Aeonsage)

| Feature | OSS | Pro |
|---------|-----|-----|
| Local AI (Ollama) | Full | Full |
| Cloud AI (BYOK) | Full | Full |
| All Channels (27+) | Full | Full |
| Skills System (100+) | Full | Full |
| Desktop App | Full | Full |
| CLI Tools | Full | Full |
| Cloud Relay | No | Yes |
| Multi-device Sync | No | Yes |
| VDID Identity | No | Yes |
| Team Management | No | Yes |
| Priority Support | No | Yes |

[Compare Plans](https://aeonsage.org/pricing)

---

## Documentation Integration

This documentation is **integrated into the existing website**:

- **Website**: `apps/website/` (React 19 + Three.js)
- **Deploy URL**: https://aeonsage.org/docs
- **No separate deployment needed**

### Integration Files

| File | Purpose |
|------|---------|
| `apps/website/src/pages/Docs.tsx` | Docs page component |
| `apps/website/src/lib/i18n.ts` | Docs categories and articles |

---

## Documentation Structure

```
docs-v2-new/
├── introduction.mdx       # Homepage
├── quickstart.mdx         # Quick start guide
├── installation.mdx       # Installation guide
├── changelog.mdx          # Version history
│
├── concepts/              # Core concepts
│   ├── architecture.mdx
│   ├── gateway.mdx
│   ├── channels.mdx
│   ├── ai-providers.mdx
│   ├── skills.mdx
│   ├── workflows.mdx
│   └── ecosystem.mdx
│
├── desktop/               # Desktop app docs
│   ├── installation.mdx
│   ├── interface.mdx
│   ├── features.mdx
│   └── local-ai.mdx
│
├── configuration/         # Configuration docs
│   ├── overview.mdx
│   ├── environment.mdx
│   └── security.mdx
│
├── channels/              # Channel integration docs
│   ├── overview.mdx
│   ├── telegram.mdx
│   ├── discord.mdx
│   ├── whatsapp.mdx
│   ├── slack.mdx
│   ├── imessage.mdx
│   ├── signal.mdx
│   └── all.mdx
│
├── providers/             # AI provider docs
│   ├── overview.mdx
│   ├── ollama.mdx
│   ├── openai.mdx
│   ├── anthropic.mdx
│   ├── openrouter.mdx
│   └── models.mdx
│
├── api-reference/         # API documentation
│   ├── introduction.mdx
│   ├── authentication.mdx
│   ├── http.mdx
│   ├── websocket.mdx
│   └── errors.mdx
│
├── self-hosting/          # Self-hosting docs
│   ├── overview.mdx
│   ├── docker.mdx
│   ├── kubernetes.mdx
│   ├── monitoring.mdx
│   └── upgrading.mdx
│
├── security/              # Security docs
│   ├── overview.mdx
│   ├── authentication.mdx
│   ├── encryption.mdx
│   └── audit.mdx
│
└── resources/             # Resources
    ├── faq.mdx
    ├── troubleshooting.mdx
    └── glossary.mdx
```

---

## Development

### Local Development

Start the website development server:

```bash
cd apps/website
pnpm dev
```

Open http://localhost:3000/docs

### Adding Documentation

1. Create new `.mdx` file in appropriate directory
2. Update `apps/website/src/lib/i18n.ts` to add navigation entry
3. Update `apps/website/src/pages/Docs.tsx` if needed

---

## Writing Guidelines

### Style Guide

- Use clear, concise language
- Write in second person ("you", "your")
- Use sentence case for headings
- Include code examples for technical concepts
- No emojis — professional enterprise style

### Component Reference

```mdx
<!-- Note/Warning/Tip -->
<Note type="info" title="Title">
  Content here
</Note>

<!-- Cards -->
<CardGroup cols={3}>
  <Card title="Title" icon="icon" href="/path">
    Description
  </Card>
</CardGroup>

<!-- Tabs -->
<Tabs>
  <Tab title="Option A">Content A</Tab>
  <Tab title="Option B">Content B</Tab>
</Tabs>

<!-- Code blocks with filename -->
```javascript:filename.js
// code here
```
```

### File Naming

- Use lowercase with hyphens: `my-page.mdx`
- Match the URL path: `/my-page`
- Group related files in directories

---

## Resources

| Resource | Link |
|----------|------|
| GitHub (OSS) | [github.com/velonone/Aeonsage](https://github.com/velonone/Aeonsage) |
| Website | [aeonsage.org](https://aeonsage.org) |
| Pricing | [aeonsage.org/pricing](https://aeonsage.org/pricing) |
| Discord | [discord.gg/aeonsage](https://discord.gg/aeonsage) |

---

## License

Documentation is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).

**Copyright 2026 VelonLabs & The AeonSage Contributors**