# File System

Kaxon stores everything directly on the file system.

Currently, there are two location Kaxon reads and writes from:

## config

Configuration at `"${XDG_CONFIG_HOME:-$HOME/.config}/kaxon/server.json"

```json
{
  "port": 3000,
  "documentsDir": "~/Documents/Kaxon"
}
```

## documents

Documents located at `config.documentsDir`. It has the following subdirectories:


```txt
- `single`
- `coupled`
```
