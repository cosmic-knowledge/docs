# Terminology

## pod

A _pod_ is data. Conceptually, this is the same as a "Word Document", "Notion Page", or "Blender File".

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

The third dimension of a pod's type:

- node
- edge
- structural (todo)
- virtual (the name and its connections inferred, but pod does not exist)

## group

_Groups_ are simply of pods that are grouped together. Usually, they share _rules_.

While it's usually better to form relationships through tags and connections for a larger graph, discrete categories are required to implement some features.

This will be removed in favor of a more "virtual pod"-like approach. To group together, say, 10 pods, use a virtual pod map to each pod. These connections could be a "virtual connection", or a "structural connection" (separate from "conceptual" connections).

## document

A _document_ is ...

## link

A _link_ is ...

## overview

An _overview_ creates a view around data. Usually, each node of an overview is a _pod_ or _collection_, and it shows the _collections_ between them. You're likely most used to hierarchal overviews, such as the file explorer within VSCode.

This concept exists as a first-class citizen so other representations such as "graph", "timeline", etc. have some level of interoperability, so the user can switch seamlessly between them.

## cover

A _cover_ is a group of pods, usually constrained against a schema. For example, an "Algebra Cover" may represent the topic of algebra. It may include links to algebra homework problems, algebra lecture notes, algebra lecture videos, and algebra cheat sheets, and other algebra-related "note groups". These different categories each have a set of associated pods.

Covers _complement_ collections. A collection may have multiple colors, that show the data in a different way. Conceptually similar are those productivity apps that allow seamless switching between Kanban Board, Calendar, and Todo List views.

In a way, _covers_ are like _overviews_, but more structured and local. This distinction helps keep covers simple, since they only cover pods, often in a single group (not multiple groups or covers themselves).

## rule

_Rules_ are constraints or code that enforces behavior. For example, one rule may enforce that pod names match a particular regular expression within a collection.

They are a core primitive that other pods and covers may use.

## plugin

Quazipanacea has a plugin-based infrastructure.

Currently, there exists _Plugin Packs_ at the highest level, which itself contains _plugins_ for each part of the app, separated by pods, overviews, collections, and the like.
