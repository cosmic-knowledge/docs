# Roadmap

1. Dogfood and iterate on abstractions

Currently, _pods_ and _models_ are core abstractions that hide details of managing files and satisfying schemas (of mind maps), respectively.

Other abstractions include:

- [ ] Common settings functionality
- [ ] Enable nesting _models_
- [ ] Modern layout manager (GoldenLayout is mediocre)
- [ ] Make it easier for plugins to export their functionality (forking to make quick fixes it not preferred)
- [ ] SSR and stuff (vite-plugin-ssr?)

Also improve package boundaries. Instead of a catch-all `@quasipanacea/util` package, things should be better separated as to not mix server/client or plugin/core concerns.

1. Improve DX experience

Fix types and add utility functions for authoring plugins for the client and server.

Make plugins dynamically loadable. Bundle plugins for use. Far in the future, experiment with module federation for easier experimentation of plugins?

When Deno improves `npm`-compatibility, remove the `dependencies -> node_modules/` symlink and dependencies in `deno.jsonc` hack.

1. Overhaul then-current plugins

Polish the then-current plugins (likely LaTeX, Excalidraw, MindElixir, Cytoscape.js). Make sure they don't have hacks.

1. Improve release process

Make tagged commits for releases and upload artifacts to GitHub.
