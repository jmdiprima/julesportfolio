<div align="center">

# Jules DiPrima

**GRC Specialist / RMF Subject Matter Expert** - Project manager driving continuous authorization, cybersecurity, and audit readiness through smart automation.

</div>

## About this site

Personal portfolio site for Jules DiPrima, built for a lunch-and-learn presentation. It covers:

- **About** - background as a Civic Tech industry expert and Project Manager
- **Work Experience** - Aquia Inc., Mindex Technologies, ScaleSec
- **Education** - Southern New Hampshire University, Mount Wachusett Community College
- **Skills** - FedRAMP, SOC 2, PCI DSS, NIST SP 800-53 Rev. 5, NIST CSF, GRC, RMF, cATO, and more
- **Projects** - the USPTO cATO initiative, Aquia's cATO offering, and Nava PBC's Unemployment Insurance modernization work
- **Contact** - LinkedIn and email

All content lives in `src/data/resume.tsx`, a single typed data file - the components read from it and don't need to be touched to update copy, links, or images.

## Stack

- [Astro v6](https://astro.build) - static site generator
- [React](https://react.dev) - interactive islands
- [Tailwind CSS v4](https://tailwindcss.com) - styling
- [shadcn/ui](https://ui.shadcn.com) - UI components
- [Cloudflare Pages](https://pages.cloudflare.com) - deployment adapter
- [pnpm](https://pnpm.io) - package manager

## Local development

**Prerequisites:** Node.js >= 22.12.0, pnpm

```bash
pnpm install
pnpm dev
```

Open <http://localhost:4321>.

## Commands

| Command | Action |
| --- | --- |
| `pnpm install` | Install dependencies |
| `pnpm dev` | Start dev server at `localhost:4321` |
| `pnpm build` | Build for production |
| `pnpm preview` | Preview production build locally |

## Project structure

```
src/
├── content/blog/     # MDX blog posts
├── data/
│   ├── resume.tsx    # Jules's personal data - name, bio, work, education, skills, projects, contact
│   └── config.ts     # Site settings & theme
├── components/       # UI components (no need to edit)
├── layouts/
│   └── Layout.astro  # HTML shell, reads from config.ts
├── pages/
│   ├── index.astro
│   └── blog/
└── styles/
    └── global.css    # Font imports & Tailwind base
public/               # Static assets (images, favicon, logos)
```

## Deployment

Pre-configured for **Cloudflare Workers or Pages** via `@astrojs/cloudflare`. Run `pnpm build` and deploy the `dist/` folder.

## Credits

Built on [Starfolio](https://github.com/webrating/starfolio), an Astro portfolio template, itself inspired by [dillionverma/portfolio](https://github.com/dillionverma/portfolio).

## License

[MIT](LICENSE)
