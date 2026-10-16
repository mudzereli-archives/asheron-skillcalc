# Asheron's Call Character Planner

A browser-based character planner for Asheron's Call. The app's editable source
is in `src/`. Try the [live planner](https://mudzereli-archives.github.io/asheron-skillcalc/).

## Run locally

Requirements: Node.js and npm.

```sh
npm install
npm start
```

Open <http://localhost:8080>. The app loads several legacy libraries from CDNs,
so an internet connection is required.

There is no compilation or separate build step: the deploy command publishes
the files under `src/` as-is.

## Publish to GitHub Pages

The deploy command publishes `src/` to the `gh-pages` branch on `origin`:

```sh
npm run deploy
```

You need push access to the repository, and GitHub Pages must be configured to
serve the `gh-pages` branch from its root. The script uses the `gh-pages` npm
package; it does not use Grunt.

**Review before deploying:** publishing replaces the contents of `gh-pages`
with the files in `src/` and changes the live site. This command does not build
or merge with the existing published site.
