# MyOps TextLocal Module

This module provides support for sending text messages using [TextLocal](http://textlocal.co.uk)
in [MyOps](https://myops.io). To use this in your MyOps installation just follow the instructions below.

## Installation

Add `myops-textlocal` plus required configuration to your MyOps configuration file at `/opt/myops/config/myops.yml`.

```yaml
modules:
  -
    name: myops-textlocal
    config:
      username: your-tl-username
      auth_hash: your-tl-api-hash
      sender: SenderName
```

Once, you've done this you can reinitize the application and restart it.

```
$ myops update-modules
$ myops restart
```
