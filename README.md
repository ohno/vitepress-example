# vitepress-example

1. Add [Node.gitignore](https://github.com/github/gitignore/blob/main/Node.gitignore).
2. Select [VitePress theme](https://www.builtatlightspeed.com/category/vitepress).
3. Install [VitePress](https://vitepress.dev/guide/getting-started):
    1. `npm add -D vitepress`,
    2. `npx vitepress init`,
    3. Insert Informations.
4. Start [a local dev server](https://vitepress.dev/guide/getting-started#up-and-running) `npm run docs:dev`.
5. Visit ［`https://github.com/user/repo-name/settings/pages`](https://github.com/ohno/vitepress-example/settings/pages) and set "Source" to "GitHub Actions".
6. Add `base: '/repo-name/', ` to `.vitepress/config.mts`.<br>https://github.com/ohno/vitepress-example/blob/0f13cb41743316ff88816c4e68f67a3d9788a43e/.vitepress/config.mts#L5
7. Add [deploy.yml](https://vitepress.dev/guide/deploy#github-pages) and change `path: docs/.vitepress/dist` to `path: .vitepress/dist` for GitHub Pages. https://github.com/ohno/vitepress-example/blob/0f13cb41743316ff88816c4e68f67a3d9788a43e/.github/workflows/deploy.yml#L53
