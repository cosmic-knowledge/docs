# Terminology

## Concepts

A _concept_ in quazipanacea matches its colloquial definition. Each concept has different _kinds_, and plugins can be made to create a new concept.

### pod

A _pod_ is the smallest unit that holds data. This can be mentally represented as a file (on the file system) with extra functionality or parts abstracted away.

For example, a `pdf` pod contains the abstractions to work with PDF files: reading, writing, opening in an editor, and so on.

Pods aren't limited to wrapping a single file. For example, a `latex` pod, can include its associated `.tex`, `.pdf`, `.sty` files and other assets.

### overview

The _overview_ exists to create a view around _pods_ and _collections_. You're likely most used to hierarchal overviews, such as the file explorer within VSCode.

This concept exists as a first-class citizen so other representations such as "graph", "timeline", etc. have some level of interoperability, so the user can switch seamlessly between them.

### collection

_Collections_ are simply of pods that are grouped together. Usually, they share _rules_.

Tags are generally preferred to draw connections among pods, but discrete categories still need to be represented in some fashion.

### rule

_Rules_ are constraints or code that enforces behavior. For example, one rule may enforce that pod names match a particular regular expression within a collection.

## Plugins

Plugins are a core part of quazipanacea:

### Plugin Pack

These are collections of plugins. Currently, plugin packs correspond to an individual. There is also a `Core/` plugin pack for all.

### Plugins

Plugins change functionality for a specific interface. Often, plugins for different interfaces of quazipanacea need to be written to fully implement the desired behavior.
