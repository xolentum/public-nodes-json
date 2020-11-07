# Xolentum Public Nodes JSON

## About

JSON list of public nodes for [Xolentum](https://www.xolentum.org).

This list can be consumed in your application so you'll always have an up-to-date list of public nodes. To consume the list, use the following URL: https://raw.githubusercontent.com/xolentum/public-nodes-json/main/xolentum-public-nodes.json

## Adding your node

If you operate a public node for Xolentum, and would like to add it to this list, fork this repository, edit the file `xolentum-public-nodes.json` in the following format and create a pull request.

```json
{
    "name": "Node Operator Name",
    "url": "node.url",
    "port": 13580,
    "ssl": false
}
```

`name` can be any name you would like. `url` should *NOT* include `http`, `https` or *any slashes*. You only need to change the `port` if you have explicitly set a separate port for the daemon RPC server, else leave it unchanged. `ssl` should only be set to `true` if you have configured *daemon SSL*, else leave it unchanged. 

To avoid node priority conflicts, please insert your node at the requisite place in *alphabetical order* of `name`.

*NOTE: Any pull requests not adhering to the above guidelines will be rejected.*

## LICENSE

[BSD 3-Clause License](LICENSE)

Copyright © 2020 The Xolentum Project
