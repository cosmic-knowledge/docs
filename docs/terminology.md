# Terminology

For each of the following, there are different types. To see all implemented types,

## Resources

We have the following resource _kinds_:

### pod

A _pod_ is the smallest unit that holds some_data. There are many types of pods. For example, a `pdf` pod contains the abstractions to work with PDF files (reading, writing, opening in editor, printing, etc.). They aren't limited to wrapping a particular file; a "LaTeX" pod, for example can have multiple files ".tex", ".pdf", ".sty", including any associated images or media files.

### overview

The _overview_ exists to create a view around _pods_ and _collections_. These exist so different representations of pods may exist as a first-class citizen. People are most used to hierarchal views, which exist in VSCode, Evernote, and plenty of other places, but other ones include "graph", "timeline", "pie", and so on.

At a minimum, an overview must have the following functionality:

- show some pods
- create a pod at any particular place
- open any particular pod

### collection

_Collections_ are simply of pods that are grouped together. Typically, but not necessarily, it is associated with a set of rules. Usually, the type of a collection is matched with its overview type.

### rule

A _rule_ is, well, a rule for a pod or a collection of pods. Rules can include pod constraints, schema constraints, tagging strategy, and more.

## Relationships

### handler

Each resource has a handler. That handler corresponds to the type of that resource.

## Reusability

### Plugins

Plugins are a core part of Quazipanacea. They extend functionality for each resource.

A plugin might have code for multiple components

### Component

Code for a particular piece of Quazipanacea.

### Packs

A collection of plugins
