# AIBolt Labs

The public website for [AIBolt Labs](https://aiboltlabs.com): an independent open-source software lab publishing projects, experiments, field notes, documentation, and working demonstrations.

## Featured project

The site includes a dedicated DYNT experience powered by the public `@dynt/formation` and `@dynt/kinetic` npm packages. It provides independent and combined engine modes, reversible Formation profiles, separate Tilt and Wave studios, fine-density cell geometry, dynamic element discovery, and framework-neutral integration.

The global site uses a calm, light-only editorial system. Expressive runtime effects remain inside the dedicated DYNT laboratories.

## Development

```bash
npm install
npm run dev
```

Before publishing:

```bash
npm run check
npm run build
npm audit --audit-level=high
```

## Content

Blog posts are Markdown files in `src/content/blog`. Pages and demonstrations live in `src/pages` and `src/components`.

## Deployment

Production deploys through Vercel from the repository default branch. The canonical domain is `aiboltlabs.com`.

## License

MIT. Brand artwork remains © AIBolt Labs.
