# Why

There's an abundance of platforms for writing, organizing, and searching knowledge. However, these platforms are often composed of disparate components or are implemented behind an opaque curtin. Others are well-thought-out, but aren't useful to the way I think, learn, and retrieve.

So I decide to make one myself, Quasipanacea. It's my personal panacea for personal knowledge management, purportedly.

It's wishlist of features includes:

- An interface that's:
  - Simple
  - Intuitive

- Data that's:
  - Backed by the file system

- A plugin system that's:
  - Arbitrarily extensible
  - Dynamically loadable
  - Fully type-safe
  - Interoperable (plugins can easily be individually replaced)

- Collaboration that's:
  - Something CRDT or OT-based

- Novel systems
  - Proper handling of data source types (bronze, silver, gold)
  - Localized schema and constraint system

I'm trying to avoid:

- Scale (each user has their own instance)
