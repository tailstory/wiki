# wiki

Notes on the tools we use at Tailstory, published at [wiki.tailstory.dev](https://wiki.tailstory.dev). A [Nimbus](https://nimbus-docs.com) site served as static assets from a Cloudflare Worker.

Pages are `src/content/docs/<vendor>/<product>/*.mdx`. Writing rules are in [AGENTS.md](AGENTS.md).

```sh
npm ci
npm run dev        # local preview
npm run typecheck
npm run build
npm run lint:docs
```

Needs the Node version in `.nvmrc`. Merges to `main` deploy.

## License

Copyright 2026 Tailstory.

- Tailstory's own prose (`src/content/`) is [CC0 1.0](LICENSE-CC0-1.0).
- Everything else, and code samples inside the prose, is [Apache 2.0](LICENSE).

CC0 covers only what Tailstory wrote. Product names, screenshots and quoted text belong to their vendors and are not ours to license. Each page links its vendor. To have something removed, open an [issue](https://github.com/tailstory/wiki/issues).

The site scaffolding comes from [Nimbus](https://github.com/cloudflare/nimbus) (MIT, copyright Cloudflare, Inc.). The fonts in `src/pages/og/_fonts/` are Inter (SIL Open Font License 1.1).
