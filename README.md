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

Prose is [CC0](LICENSE).
