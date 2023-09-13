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
