+++
title="clients"
weight=16
+++
### Client

<hr>

*class* discord.**Client**(**options) *<sup>[Source](https://discordpy.readthedocs.io/en/master/api.html?highlight=discord#clients)</sup>*

{{< block "grid-2" >}}

{{< column >}}

**<h3>Attributes</h3>**
{{< tip >}}
activity<br>
allowed_mentions<br>
application_flags<br>
application_id<br>
cached_messages<br>
emojis<br>
guilds<br>
intents<br>
latency<br>
persistent_views<br>
private_channels<br>
status<br>
stickers<br>
user<br>
users<br>
voice_clients<br>
ws
{{< /tip >}}

{{< /column >}}
{{< column >}}

**<h3>Methods</h3>**
{{< tip >}}
`def` add_view<br>
`async` application_info<br>
`async` before_identify_hook<br>
`async` change_presence<br>
`def` clear<br>
`async` close<br>
`async` connect<br>
`async` create_dm<br>
`async` create_guild<br>
`async` delete_invite<br>
`@` event<br>
`async` fetch_channel<br>
`async` fetch_guild<br>
`async for` fetch_guilds<br>
`async` fetch_invite<br>
`async` fetch_premium_sticker_packs<br>
`async` fetch_stage_instance<br>
`async` fetch_sticker<br>
`async` fetch_template<br>
`async` fetch_user<br>
`async` fetch_webhook<br>
`async` fetch_widget<br>
`def` get_all_channels<br>
`def` get_all_members<br>
`def` get_channel<br>
`def` get_emoji<br>
`def` get_guild<br>
`def` get_partial_messageable<br>
`def` get_stage_instance<br>
`def` get_sticker<br>
`def` get_user<br>
`def` is_closed<br>
`def` is_ready<br>
`def` is_ws_ratelimited<br>
`async` login<br>
`async` on_error<br>
`def` run<br>
`async` setup_hook<br>
`async` start<br>
`async` wait_for<br>
`async` wait_until_ready
{{< /tip >}}

{{< /column >}}

{{< /block >}}

Represents a client connection that connects to Discord. This class is used to interact with the Discord WebSocket and API.

A number of options can be passed to the [Client](http://localhost:1313/docs/compose/client/)

**Parameters:**
- **max_messages** (Optional[[int](https://docs.python.org/3/library/functions.html#int)])
<br>The maximum number of messages to store in the internal message cache. This defaults to `1000`. Passing in `None` disables the message cache.
- **proxy** (Optional[[str](https://docs.python.org/3/library/stdtypes.html#str)]) – Proxy URL.
- **proxy_auth** (Optional[[aiohttp.BasicAuth](https://docs.aiohttp.org/en/stable/client_reference.html#aiohttp.BasicAuth)]) – An object that represents proxy HTTP Basic Authorization.
- **shard_id** (Optional[[int](https://docs.python.org/3/library/functions.html#int)]) – Integer starting at `0` and less than shard_count.
