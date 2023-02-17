# Quirks

There are a few quirks. Currently, for things to work, there must be a symlink to `node_modules/` in `init/` and a symlink to `server-deno/` in `client-web/`. Not to mention the symlinking of `common/` in nearly all repositories.

- Stray `tsconfig.json` files
- Edit main `tsconifg.json` to not include `server-deno/` subdirectory (and edit eslint config and prettier config to match)
- Fix types (`globals.t.ds`)

In the future, these should be cleaned up.
