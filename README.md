# css-reloader-ce

**Archived.** This repository is kept read-only for reference.

A 2022 scaffold for a Chrome extension that was meant to reload a page's stylesheets without a full refresh. It never got past the starting point: the code is the React 17 + Webpack 5 Manifest V3 boilerplate ([lxieyang/chrome-extension-boilerplate-react](https://github.com/lxieyang/chrome-extension-boilerplate-react)) with the default popup, new-tab, options, devtools panel and content script, and no CSS-reloading logic. There are no releases and it was never published to the Chrome Web Store.

## What is here

- `src/manifest.json`: Manifest V3, content script on all URLs, background service worker, popup, options and devtools pages (all boilerplate).
- `src/pages/*`: the template's React pages, untouched.
- `utils/build.js`, `utils/webserver.js`, `webpack.config.js`: the template's build and dev-server scripts.

`npm install && npm run build` should produce an unpacked extension in `build/`, but the dependency list still includes `node-sass`, which fails to install on current Node versions; dropping it (see closed PR #2) is the known fix.

## Why it is archived

Any dev server with live reload or hot module replacement covers the use case, so there was no reason to finish it. Archived in November 2026 rather than deleted so the history stays visible.

## License

MIT. See [LICENSE](LICENSE).
