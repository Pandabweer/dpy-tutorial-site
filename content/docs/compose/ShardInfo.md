+++
title="ShardInfo"
weight=16
+++

<hr>

*class* discord.**ShardInfo**(**options) *<sup>[Source](https://discordpy.readthedocs.io/en/master/api.html?highlight=discord#shardinfo)</sup>*

{{< block "grid-2" >}}

{{< column >}}

**<h3>Attributes</h3>**
{{< tip >}}
id<br>
latency<br>
shard_count
{{< /tip >}}

{{< /column >}}
{{< column >}}

**<h3>Methods</h3>**
{{< tip >}}
`async` connect<br>
`async` disconnect<br>
`def` is_closed<br>
`def` is_ws_ratelimited<br>
`async` reconnect

{{< /tip >}}

{{< /column >}}

{{< /block >}}

A class that gives information and control over a specific shard.

You can retrieve this object via AutoShardedClient.get_shard() or AutoShardedClient.shards.
