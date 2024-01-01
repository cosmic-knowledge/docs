# Tools <!-- omit in toc -->

- [Introduction](#introduction)
- [Static Formats](#static-formats)
  - [Diagrams](#diagrams)
  - [Typesetting Languages](#typesetting-languages)
  - [Markup Languages](#markup-languages)
  - [Drawing](#drawing)
  - [generator](#generator)
- [Dynamic Formats](#dynamic-formats)
  - [Diagrams / Charts](#diagrams--charts)
  - [Infinite Canvas](#infinite-canvas)
  - [Infinite Whiteboard](#infinite-whiteboard)
  - [Documents](#documents)
  - [Flow-Based Programming](#flow-based-programming)
  - [Slides](#slides)
  - [Blocks](#blocks)
  - [Text Editors](#text-editors)
  - [Block-Based Standards](#block-based-standards)
- [Sidecar Formats](#sidecar-formats)
  - [category](#category)
- [Querying formats](#querying-formats)
  - [Table](#table)
  - [Graph](#graph)
  - [Structured](#structured)
- [Other](#other)
  - [Computation](#computation)
  - [Storage and Synchronization](#storage-and-synchronization)
- [Applications](#applications)
  - [Code IDEs](#code-ides)
  - [Design Prototyping](#design-prototyping)
  - [Thinking Tools](#thinking-tools)
  - [Notebooks](#notebooks)
- [Knowledge Infrastructure](#knowledge-infrastructure)
- [Miscellaneous](#miscellaneous)
  - [Domain-Specific](#domain-specific)
  - [Similar Tool Aggregations](#similar-tool-aggregations)
  - [Obsolete Solutions](#obsolete-solutions)

## Introduction

There are a lot of useful tools. Naturally, separate tools have limited interoperability. This document lists some tools, some of which are prime candidates for experimenting with that.

TODO: sort by implementation, grammars, standards, etc.

## Static Formats

Standalone format with limited to no interaction points.

### Diagrams

Hierarchy:

- Graphics / Diagrams
  - [penrose](https://penrose.cs.cmu.edu/)
  - [bpmm-io](https://bpmn.io) (bpmm-js, cmmn-js, dmm-js, form-js)
  - [Kroki](https://kroki.io)
  - [VegaLite](https://vega.github.io/vega-lite)
  - [railroad-diagrams](https://github.com/tabatkins/railroad-diagrams)
- Architecture
  - [C4](https://c4model.com)
- Novel representations
  - [kodemo](https://kodemo.com)
- Gantt Chart
  - [Markwhen](https://markwhen.com)
- ?
  - [Metadesk](https://dion.systems/metadesk)
  - [Scribble](https://docs.racket-lang.org/scribble)
  - [Org Mode](https://orgmode.org)
  - [Mathlingua](https://mathlingua.org)
  - [Argdown](https://argdown.org)
  - [notecalc3](https://github.com/bbodi/notecalc3)
- Kind of XML
  - [DITA](https://www.oxygenxml.com/dita/1.3/specs)
  - [HTML](https://html.spec.whatwg.org/multipage)
  - [DocBook](https://docbook.org)
- [From Pandoc](https://pandoc.org)
- Publishing systems
  - [pollen](https://docs.racket-lang.org/pollen)
  - [speedata](https://github.com/speedata/publisher)
  - [TUSTEP](https://www.tustep.uni-tuebingen.de/tustep_eng.html)
- UML
  - [PlantUML](https://plantuml.com)
  - [nomnoml](https://nomnoml.com)
  - YUML

### Typesetting Languages

- text to document
- markup languages
- typesetting languages

- Typesetting
  - [LaTeX](https://www.latex-project.org)
  - [typst](https://typst.app)
  - [sile](https://github.com/sile-typesetter/sile)
  - [troff](https://troff.org)
  - [Heirloom](https://heirloom.sourceforge.net/doctools.html)
  - [lout](https://savannah.nongnu.org/projects/lout)
  - [Patoline](https://github.com/patoline/patoline)

### Markup Languages

- Markup: Markdown
  - [Markdoc](https://markdoc.dev)
  - [Markdown GitHub Flavoured](https://github.github.com/gfm)
  - [Markdown MyST](https://jupyterbook.org/en/stable/content/myst.html)
  - [MDX](https://mdxjs.com)
  - [Markdown RMarkdown](https://rmarkdown.rstudio.com)
  - [AsciiDoc](https://asciidoc.org)
  - [Asciidoctor](https://asciidoctor.org)
- Markup: Other
  - [NestedText](https://nestedtext.org/en/stable)
  - [reStructuredText](https://docutils.sourceforge.io/rst.html)
  - [Smartdown](https://smartdown.io)
  - [BBCode](https://en.wikipedia.org/wiki/BBCode)
  - [PENDOWN](https://github.com/senselogic/PENDOWN)
  - [Scroll](https://scroll.pub)
  - [Textile](https://en.wikipedia.org/wiki/Textile_(markup_language))
  - [WikiText/WikiCode](https://en.wikipedia.org/wiki/Help:Wikitext)
  - [Creole](https://en.wikipedia.org/wiki/Creole_(markup))

### Drawing

- [milton](https://github.com/serge-rgb/milton)
- [excalidraw](https://excalidraw.com)
- [tldraw](https://www.tldraw.com)
- [jspaint](https://github.com/1j01/jspaint)

### generator

- [tbls](https://github.com/k1LoW/tbls)

## Dynamic Formats

Standalone format fundamentally based on interaction points.

### Diagrams / Charts

- [D3](https://d3js.org)
- [JSXGraph](https://jsxgraph.uni-bayreuth.de/wp)
- [function-plot](https://mauriciopoppe.github.io/function-plot)
- [Observable Plot](https://observablehq.com/plot)
- [sprotty](https://github.com/eclipse-sprotty/sprotty)
- [miro](https://miro.com)
- [state-designer](https://github.com/steveruizok/state-designer)
- [xstate](https://github.com/statelyai/xstate)

### Infinite Canvas

- [jade](https://github.com/dragonman225/jade)
- [fastboard](https://github.com/netless-io/fastboard)

### Infinite Whiteboard

- [fastboard](https://github.com/netless-io/fastboard)
- [lovasoa/whitebophir](https://github.com/lovasoa/whitebophir)
- [cracker0dks/whiteboard](https://github.com/cracker0dks/whiteboard)
- [box-line-text](https://github.com/jncraton/box-line-text)
- [Whitebird](https://github.com/BuchholzTim/Whitebird)

### Documents

- WYSIWYG Editors

### Flow-Based Programming

- Category: 1
  - [reaflow](https://github.com/reaviz/reaflow)
  - [flume](https://flume.dev)
  - [rete](https://github.com/retejs/rete)
  - [noflo](https://github.com/noflo/noflo)
- Category: 2
  - [Node-RED](https://nodered.org)
- Category: other
  - [Drawflow](https://github.com/jerosoler/Drawflow)
  - [NodeBox](https://www.nodebox.net)
  - [baklavajs](https://github.com/newcat/baklavajs)
  - [litegraph.js](https://github.com/jagenjo/litegraph.js)
  - [nodify](https://github.com/miroiu/nodify)
  - [nodes.io](https://nodes.io)
  - [Seneral](https://github.com/Seneral/Node_Editor_Framework)
  - [ThreeNodes.js](https://github.com/idflood/ThreeNodes.js)
  - [GSN Composer](https://www.gsn-lib.org/docs/getstarted.php)
  - [enso](https://github.com/enso-org/enso)
  - [butterfly](https://github.com/alibaba/butterfly)
  - [samuelmtimbo/unit](https://github.com/samuelmtimbo/unit)
  - [diagram-maker](https://github.com/awslabs/diagram-maker)

### Slides

- [sli.dev](https://github.com/slidevjs/slidev)
- [marp](https://github.com/marp-team/marp)
- [slides](https://github.com/maaslalani/slides)
- [code-surfer](https://github.com/pomber/code-surfer)
- [gitpitch](https://github.com/gitpitch/gitpitch)
- [fusuma](https://github.com/hiroppy/fusuma)
- [mdp](https://github.com/visit1985/mdp)
- [big](https://github.com/tmcw/big)
- [reveal.js](https://github.com/hakimel/reveal.js)

### Blocks

- [editor.js](https://editorjs.io)
- [BlockSuite](https://github.com/toeverything/blocksuite)
- [BlockNote](https://www.blocknotejs.org)
- [Plate](https://plate.udecode.io)
- [slate](https://github.com/ianstormtaylor/slate)
- [bangle.dev](https://github.com/bangle-io/bangle.dev)
- Markdown-based
  - [Milkdown](https://milkdown.dev)
  - [tui.editor](https://ui.toast.com/tui-editor)

### Text Editors

- [Lexical](https://github.com/facebook/lexical)
- [Tiptap](https://tiptap.dev)
- [ProseMirror](https://prosemirror.net)
- [Quill](https://github.com/quilljs/quill)
- [Trix](https://trix-editor.org)

### Block-Based Standards

- [GitHub Blocks](https://blocks.githubnext.com)
- [Mobiledoc](https://github.com/bustle/mobiledoc-kit)
- [Block Protocol](https://blockprotocol.org)
- [hash.ai](https://hash.ai)
- [Solid](https://solidproject.org)
- [Adaptive Cards](https://adaptivecards.io)

## Sidecar Formats

Annotate or extends existing format.

### category

- [Annotator](https://github.com/openannotation/annotator)
- [h](https://github.com/hypothesis/h)
- [OpenPecha](https://github.com/OpenPecha)
- [audino](https://github.com/midas-research/audino)
- [Universal Data Tool](https://udt.dev)
- [doccano](https://github.com/doccano/doccano)
- [brat](https://github.com/nlplab/brat)
- [INCEpTION](https://github.com/inception-project/inception)

## Querying formats

### Table

### Graph

- [GraphQL](https://graphql.org)

### Structured

- XQuery
- [GROQ](https://github.com/sanity-io/GROQ)

## Other

### Computation

- [numbat](https://github.com/sharkdp/numbat)

### Storage and Synchronization

- [IPFS](https://github.com/ipfs/ipfs)
- [IPLD](https://github.com/ipld)
- [Earthstar](https://earthstar-project.org)
- [perkeep](https://github.com/perkeep/perkeep)
- [PDS Interop](https://github.com/pdsinterop)

## Applications

### Code IDEs

- [codesandbox](https://codesandbox.io)
- [sandpack](https://github.com/codesandbox/sandpack)
- [theia](https://theia-ide.org)
- [VSCode](https://code.visualstudio.com/docs/editor/vscode-web)
- [devcontainers](https://github.com/devcontainers)
- [awesome-online-ide](https://github.com/styfle/awesome-online-ide)
- [devpod.sh](https://devpod.sh)

### Design Prototyping

- [Penpot](https://github.com/penpot/penpot)
- [Wireflow](https://wireflow.co)
- [Plasmic](https://www.plasmic.app)
- [Akira](https://github.com/akiraux/Akira)
- [QuantUX](https://quant-ux.com)
- Other
  - [JSON Crack](https://github.com/AykutSarac/jsoncrack.com)
  - [drawio](https://github.com/jgraph/drawio)
  - [motion-canvas](https://github.com/motion-canvas/motion-canvas)

### Thinking Tools

- Toolbox / Creative Coding Libraries / Frameworks
- Visual Thinking Tool / Thinking Canvas / Mind Mapping / FreeForm Thinking

- [Kinopio](https://kinopio.club)
- [orange3](https://github.com/biolab/orange3)
- [gtoolkit](https://github.com/feenkcom/gtoolkit)
- [raylib](https://github.com/raysan5/raylib)
- [nannou](https://github.com/nannou-org/nannou)
- [datarabbit](https://www.datarabbit.com)

### Notebooks

- [Jupyter](https://jupyter.org)
- [Pluto.jl](https://github.com/fonsp/Pluto.jl)
- [polynote](https://github.com/polynote/polynote)
- [clerk](https://github.com/nextjournal/clerk)
- [starboard-notebook](https://github.com/gzuidhof/starboard-notebook)
- [percival](https://github.com/ekzhang/percival)
- [nbdev](https://nbdev.fast.ai)
- [nteract](https://nteract.io) stack
- [quarto](https://quarto.org)

## Knowledge Infrastructure

Tools to search, explore, publish, and use data or knowledge.

- [datahub](https://github.com/datahub-project/datahub)
- [ckan](https://github.com/ckan/ckan)
- [Datasette](https://datasette.io)
- [PubPub](https://www.pubpub.org)
- [KnowledgeFutures](https://www.knowledgefutures.org)
- [Open Knowledge Foundation](https://okfn.org)
- [TopicQuests](https://topicquests.org)
- [Underlay](https://www.underlay.org)
- [LearnAwesome](https://learnawesome.org)
- Research?
  - [OER Commons](https://oercommons.org)
  - [Dryad](https://datadryad.org/stash)
  - [Microsoft Dataverse](https://powerplatform.microsoft.com/en-us/dataverse)
  - [OSF](https://osf.io)
  - [figshare](https://figshare.com)

## Miscellaneous

### Domain-Specific

- GNOME
- [Workbench](https://github.com/workbenchdev/Workbench)
- Language Parsing
  - [ASTExplorer](https://astexplorer.net)
- Biology
  - [WikiPathways](https://www.wikipathways.org)
- Geology
  - [TopoJSON](https://github.com/topojson)
  - [GeoJson](https://geojson.org)
- C++
  - [Compiler Explorer](https://compiler-explorer.com)
  - [BuildBench](https://build-bench.com)
  - [QuickBench](https://quick-bench.com)
  - [CppInsights.io](https://cppinsights.io)
- Event Processing
  - [memphis](httpsh://github.com/memphisdev/memphis)

### Similar Tool Aggregations

- [infinitecanvas.tools](https://infinitecanvas.tools/gallery)
- [swyxio/spark-joy](https://github.com/swyxio/spark-joy/blob/master/README.md#diagramming)
- [Knowledge-Graph-Tutorials-And-Papers](https://github.com/heathersherry/Knowledge-Graph-Tutorials-and-Papers)
- [awesome-nod-ebased-uis](https://github.com/wbkd/awesome-node-based-uis)
- [awesome-diagramming](https://github.com/shubhamgrg04/awesome-diagramming)
- [Awesome-Design-Tools](https://github.com/goabstract/Awesome-Design-Tools)
- [tools-list](https://github.com/everestpipkin/tools-list)
- [xosh.org/text-to-diagram](https://xosh.org/text-to-diagram)

### Obsolete Solutions

These were popular in the past, but have been superceded by more modern tools.

- [js-sequence-diagrams](https://bramp.github.io/js-sequence-diagrams): use Mermaid
- [flowchart.js](https://flowchart.js.org): use Mermaid
- [mxGraph](https://jgraph.github.io/mxgraph): use Cytoscape.js
- [Umple](https://cruise.umple.org/umple): use PlantUML
- [Treant.Js](https://github.com/fperucic/treant-js): use D3.js/vis.js/Cytoscape.js
- [mapjs](https://www.mindmup.com): use markmap
- [jsmind](https://jsmind.online): use markmap
- [VivaGraph](https://github.com/anvaka/VivaGraphJS): use vis.js/Cytoscape.js
- [jsconsole](https://github.com/remy/jsconsole)
- [mdx-deck](https://github.com/jxnblk/mdx-deck)
- [nodeppt](https://github.com/ksky521/nodeppt)
