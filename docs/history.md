# history

## Naming

Previously, this project was called Kaxon, then Knowledge Supercluster, then Kosmic

## Note Structure

1. Flat Representation

The root "knowledge directory" contains directories that contain the notes themselves. Only one layer of directories was supported and only markdown files were supported for simplicity. Things were split into "single" and "coupled" documents, which was dumb.

2. Hierarchial Representation

The root "knowledge directory" contains directories in the following hierarchy: `root dir -> areas -> topics`. Each topic directory then contains the markdown files. This is a makeshift representation, existing so that I can actually use this project to store my notes and work on other parts of the project.

3. Flexible Hierarchy

Later, investigate making the representation completely flat, using UUIDs. `12/3e4567-e89b-12d3-a456-426614174000/note.md`. Investigate using symlinks (leak abstractions) or FUSE (slow) to better connect topics for browsing. Think about how different file types should be separated and treated (markdown, code files, PNGs, other assets, etc.)
