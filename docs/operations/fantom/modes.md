---
meta:
  - name: description
    content: Learn the difference between a Fantom full node and an archive node. Run sample commands to see the difference.
  - name: keywords
    content: fantom geth opera ftm node full archive difference
---

# Modes

Chainstack supports deploying a Fantom node on the mainnet in the following modes:

* Full node — a node that stores full blockchain data.
* Archive node — a node that stores full blockchain data and an archive of historical states.

To be a part of the Fantom mainnet, you can deploy either a full node or an archive node.

With a full node, you can query the historical state of the Fantom mainnet at only the latest 128 blocks.

To be able to query the historical state of the Fantom mainnet at any block, you need an archive node.

See [Geth JSON-RPC methods](https://eth.wiki/json-rpc/API#the-default-block-parameter) that support querying at a block number.

Query example to get the balance of an address at different block numbers through an archive node:

``` js
> ftm.getBalance("0x663f6ab861014056274128C69ff80caDCf048603","latest")
114374136421608538487
> ftm.getBalance("0x663f6ab861014056274128C69ff80caDCf048603","18372820")
0
```

::: tip See also

* [Networks](/operations/fantom/networks)
* [Tools](/operations/fantom/tools)
* [Tutorials](/tutorials/fantom/)

:::
