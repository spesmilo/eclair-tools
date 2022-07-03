Eclair management tools

The following environment variables need to be defined:

 MAINNET_ECLAIR
 MAINNET_BITCOINCLI


Examples:

 $ ./listchannels --public --sortby nodeId  | ./format
 $ ./listchannels --private --sortby toLocal | ./format
 $ ./listchannels | ./sum_balances
 $ eclair peers | ./connected | jq -s 'length'


Some commands require init_db:

 $ ./init_db
 $ ./last_active 718327x534x2
 $ ./relayed_by_channel 718327x534x2

