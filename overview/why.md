# Why

There's an abundance of platforms for writing, organizing, and searching knowledge in existence. However, these platforms are often composed of disparate components or are implemented behind an opaque curtin. Others are well-thought-out, but aren't useful to the way I think, learn, and retrieve.

So I decide to make one myself, Quasipanacea. It's my personal panacea for personal knowledge management, purportedly.

It's wishlist of features includes:

- An interface system:
  - Simple
  - Intuitive
- A storage system:
  - Backed by the file system (but not coupled to its hierarchy!)
  - Flat hierarchy
- A plugin system:
  - Low friction
  - Dynamically loadable
  - Fully type-safe
  - Arbitrarily extensible
- A collaboration system:
  - I'm not sure; definitely something [CRDT](https://en.wikipedia.org/wiki/Conflict-free_replicated_data_type)-related
- Novel systems
  - Reproducible References (like [Reproducible Builds](https://reproducible-builds.org))
  - Proper handling of data source types (bronze, silver, gold)
  - A global schema and constraint system

What I'm not trying to do:

- Scale
  - Each user must spin up their own instance

I'll detail the parts later.
