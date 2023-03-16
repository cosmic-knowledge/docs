# File System

Quazipanacea stores everything directly on the file system.

Currently, there are two location Quazipanacea reads and writes from:

## config

Configuration at `"${XDG_CONFIG_HOME:-$HOME/.config}/quazipanacea/server.json"`

```json
{
  "documentsDir": "~/Documents/Quazipanacea"
}
```

## data

The directory contains the files:

```txt
covers.json
covers
  b8/
    e1a398-6c62-4159-a8c3-2fa1038f8dce/
    ...
  d1
    c14642-7bad-4bb9-bef0-64cf4a32a982/
    def81a-3cd0-420b-9eac-dff07aa37d7c/
    ...
  ...
groups.json
groups/
  ...
pods.json
pods/
  ...
```

Each of those subdirectory contain a pod's data.
