# Learnings

I have tried to write things, but have failed. I learned some things.

## Orbs and Links

I implemented the concept of 'orbs' and 'links' in `routes.ts` with corresponding files to match.

I thought it would make sense to have the concept of "nodes" and "edges" abstracted as a core concept, rather than be an implementation of a particular _overview_.

I also thought it would be a good way to have "virtual pods" (ones created on demand).

I'm removing them because "overviews" are not mature enough to warrant this abstraction.

## Plugin Families

Plugin families were supposed to distinguish the behavior of plugins. Between "themes", "packs", "pods", and "overviews". But, as I decoupled the view and logic layer of these plugins, families began to also include "modelview", and "podview". Things became less clear, as these families don't have corresponding `.json` files.

I don't think distinguishing these behaviors/responsibilities is needed. Plugins could just export different function names, or have an object for each behavior/responsibility.

Removing "plugin families" would also simplify the TypeScript types representing a plugin.

Executing plugin logic would be easier. Instead of checking that both "plugin family" and a function exists (to call), only the latter check is needed.

This would also simplify existing plugins since "models" can come bundled with an existing "modelview" (instead of having it separated in an extra plugin).

## Deno

Not useful.

## Approach 2

I don't think the previous approach works well:

1. Poor integration with external tools / Data ownership

When integrating with other technologies (data formats, diagram types, etc.), it was somewhat difficult when it was its own application. For example, in the case of a flashcard app, it would be easier to create some Anki plugin to integrate with Quasipanacea, compared to creating a separate app.

The way that Quasipanacea works, it made that difficult because data was owned by the "quasipanacea main app", and applications/plugins queried that information. As a side affect, any documents or data not in Quasipanacea were harder to integrate with.

Therefore, it is important to:

- Reuse existing applications when possible
- Centrally storing objects and files in a uuid/ file system hierarchy is not good
  - This was originally done because In The Future, the file system can be "recreated" elsewhere for arbitrary hierarchy
    - This can still be done without uuid/ stuff
- If applications "own the data", then integrating it with other Quasipanacea things will be more difficult

This would best be solved in a compaible way. You will want to use your notes in Obsidian vault for starters (so nothing needs to be copied over).

Add "obsidian-like" vault directories. These contain Markdown notes with links, etc. Expose that information to be used in some way by models.

You had thoughts about some sort of "data broker" but that seems unecessary.

2. Bad central interface

The idea of a graph view sounded good. For example, Obsidian uses this. But using this was too hard to use. Automated layouts did not work properly. And manually moving nodes on a graph does did not feel right.

Nodes would later become problematic when showing, say, pictures or pixibufs. These things should be represented as a set of 4 points, rather than a single point like a node.

Solve this by creating a new, default interface. Similar to Obsidian Canvas.

Keep it simple, more complex things can always be done in tldr, excalidraw, etc.

A simple infinite canvas.

3. Testing changes

Previously, opening app in background and running server + client was requied for testing. Testing changes, and using the app (more than just the HEAD version) needs to be easier.
