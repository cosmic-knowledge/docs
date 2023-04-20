# Terminology

## Definitions

### orb

Nodes of a knowledge graph.

### link

Edges of a knowledge graph.

### anchor

A special orb. It includes:

- a schema for knowledge to be constrained against
- rules as additional constraints for orbs, pods, and the like
- covers for a set of faithful semantic representations of the schema
- metadata to store properties, tags, authorship, last modified dates, and the like

### cover

It is responsible for representing knowledge, given a particular schema.

A _cover_ is to an _anchor_ as an _overview_ is to a knowledge graph.

For example, an "Algebra Cover" may represent the topic of algebra. It may include links to algebra homework problems, algebra lecture notes, algebra lecture videos, and algebra cheat sheets, and other algebra-related "note groups". These different categories each have a set of associated pods.

Another example includes productivity apps that have a kanban, calendar, and todo view.

### pod

Responsible for managing data. Like a "Word Document", "Notion Page", or "Blender File".

A _pod_ is to documents as a class is to bytes.

The first dimension of a pod's type:

- file
- directory

For example, a `pdf` _file pod_ contains a `.pdf` file, and has functionality for reading, writing, and opening the pdf file.

Another example, a `latex` _directory pod_, has not only a `.tex` file, but also its associated `.pdf`, `.sty`, `.png`, and other files.

The second dimension of a pod's type:

- void (no file)
- plaintext
- markdown
- chemical

So far, all of these are first-party plugins.

### overview

An _overview_ creates a view around data. Usually, each node of an overview is a _pod_ or _anchor, and it shows the_collections_ between them. You're likely most used to hierarchal overviews, such as the file explorer within VSCode.

This concept exists as a first-class citizen so other representations such as "graph", "timeline", etc. have some level of interoperability, so the user can switch seamlessly between them.

### rule

_Rules_ are constraints or code that enforces behavior. For example, one rule may enforce that pod names match a particular regular expression within a collection.

They are a core primitive that other pods and covers may use.

### plugin

Quasipanacea is highly extensible with plugins.

There are different types of plugins:

- anchor
- cover
- overview
- pack
- pod
- theme

## Definitions 2

- Analogue
