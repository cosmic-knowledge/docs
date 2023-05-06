# Storage

Quasipanacea stores everything directly on the file system.

Currently, there are two location Quasipanacea reads and writes from:

## config

Configuration at `"${XDG_CONFIG_HOME:-$HOME/.config}/quasipanacea/server.json"`

```json
{
  "documentsDir": "~/Documents/Quasipanacea"
}
```

## data

The directory contains the files:

```txt
views.json
views
  b8/
    e1a398-6c62-4159-a8c3-2fa1038f8dce/
    ...
  d1
    c14642-7bad-4bb9-bef0-64cf4a32a982/
    def81a-3cd0-420b-9eac-dff07aa37d7c/
    ...
  ...
pods.json
pods/
  ...
```

Each of those subdirectory contain a pod's data.
