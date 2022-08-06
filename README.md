# Eclair management tools


## Getting started

The following environment variables need to be defined:

```
 MAINNET_ECLAIR
 MAINNET_BITCOINCLI
```

Note that amount are in mBTC.


## Examples:

```
 $ ./listchannels --public --sortby nodeId  | ./format
 $ ./listchannels --private --sortby toLocal | ./format
 $ ./listchannels | ./sum_balances
 $ eclair peers | ./connected | jq -s 'length'
```

Some commands require a database initialization:

```
 $ ./init_db
 $ ./last_active 718327x534x2
 $ ./relayed_by_channel 718327x534x2
```
