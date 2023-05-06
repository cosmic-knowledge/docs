# Terminology

```mermaid
flowchart TD
  subgraph "Overview (graph perspective)"
    direction BT
    overview1[Overviews]

    orb1[Orbs] --> overview1
    link1[Links] --> overview1
    orb1 <-.-> link1
  end

  subgraph "Overview (knowledge perspective)"
    direction BT
    overview2[Overviews]

    anchor2[Anchors] --> overview2
    cover2[Covers] --> anchor2
    orb2[Orbs] --> anchor2
    link2[Links] --> anchor2
    pod2[Pods] --> anchor2
    rule2a[Rules] --> cover2
    rule2b[Rules] --> orb2
    rule2c[Rules] --> link2
    rule2d[Rules] --> pod2
  end
```

## Definitions

### overview

An _overview_ renders a knowledge repository. Most of the graph and relationship construction is delegated to _anchors_.

This concept exists as a first-class citizen so users can experiment with how _they_ display their knowledge.

### orb

Is a node on the knowledge graph.

- May have an associated pod (TODO)

### link

Is an edge on the knowledge graph.

- May have an associated pod

### pod

Responsible for managing data. Like a "Word Document", "Notion Page", or "Blender File".

A _pod_ is to documents as a class is to bytes.

There are _file_ pods and _directory_ pods.

For example, a `pdf` _file pod_ contains a `.pdf` file, and has functionality for reading, writing, and opening the pdf file.

For example, a `latex` _directory pod_, has not only a `.tex` file, but also its associated `.pdf`, `.sty`, `.png`, and other files.

### anchor

Is a node on the knowledge graph.

Anchors play a vital part in organizing data and their relationships. They:

- are a schema for knowledge to be constrained against
- have rules as additional constraints for orbs, pods, and the like
- have covers for a set of faithful semantic representations of the schema
- store metadata of properties like: tags, authorship, last modified dates, etc.

### cover

Responsible for representing knowledge of an anchor.

For example, an "Algebra Cover" may represent the topic of algebra. It may include links to algebra homework problems, algebra lecture notes, algebra lecture videos, and algebra cheat sheets, and other algebra-related "note groups". These different categories each have a set of associated pods.

Another example relates to productivity apps that have a kanban, calendar, and todo view. Each view would correspond to a cover, and the data within those views are _conceptually_ stored in each anchor.

### rule

_Rules_ are constraints that enforce behavior. For example, one rule may enforce that pod names match a particular regular expression.

They are a core primitive that other pods, covers, and anchors may use.

### plugin

Quasipanacea is highly extensible.

There are many different types of plugins:

- anchor
- cover
- overview
- pack
- pod
- theme

## Definitions 2

- Analogue
