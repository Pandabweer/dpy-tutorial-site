+++
title = "Discord.py tutorial"
[data]
baseChartOn = 3
colors = ["#627c62", "#11819b", "#ef7f1a", "#4e1154"]
columnTitles = ["Section", "Status", "Author"]
fileLink = "content/projects.csv"
title = "Projects"

+++
{{< block "grid-2" >}}
{{< column >}}

# A Discord.py tutorial & documentation

Clean and easy on the eyes, inspired by [tutorial.vcokltfre](https://tutorial.vcokltfre.dev).

{{< tip "warning" >}}
This is an open sourced project,
Feel free to open a [PR](https://github.com/Pandabweer/dpy-tutorial-site/pulls "Open GitHub pull request"),
raise an [issue](https://github.com/Pandabweer/dpy-tutorial-site/issues/new/choose "Open a Github Issue")(s).
{{< /tip >}}

{{< tip "warning" >}}
The discord.py library is an advanced Python library. As such a certain amount of intermediate Python knowledge is assumed in this tutorial,
and basic Python functionality will be not covered or explained.

If you're willing to learn and search for things you don't understand as you follow along,
there's no reason you shouldn't be able to participate.
{{< /tip >}}

{{< tip "warning" >}}
The premise of this tutorial is that you write code yourself, and understand what you are writing.
I aim to explain what I'm doing, and clarify the decisions I make,
but this tutorial will not help you if you choose to copy and paste its content rather than try to understand and work it out for yourself.

I highly recommend you play around with the code you write and make it different from what you see here.
This is to help you learn how to use discord.py, you can also ask for help in the [Python Discord server](https://discord.gg/Python).
{{< /tip >}}

{{< tip >}}
For this tutorial you will need:

 - Python 3.8 or later installed
 - discord.py 2.0.0 or later installed
 - Intermediate Python experience or a strong will to learn

{{< /tip >}}

{{< button "tutorials/" "Tutorial" >}}
{{< button "docs/compose/" "Read the Docs" >}}
{{< /column >}}

{{< column >}}

## Updates & info
{{< tip "warning" >}}
#### Privileged Intent & bot verification
Discord is making message content a privileged intent for verified bots. This will
go in on **August 31, 2022**.

**This change affects only verified bots**, bots that are in 75 or more servers. Unverified bots in fewer than 75 servers are not affected at all.

This means that **verified** bots will need to [request](https://support.discord.com/hc/en-us/requests/new)
this intent to Discord.

[Read more](https://support-dev.discord.com/hc/en-us/articles/4404772028055-Message-Content-Privileged-Intent-for-Verified-Bots)
{{< /tip >}}
{{< tip >}}
#### Updates from [Discord.py](https://github.com/Rapptz/discord.py "GitHub")
Thanks to the 19 authors who had 23 merged pull requests this week!

**Breaking Changes**

- The arguments for item, interaction inside View callbacks have been swapped to interaction, item for consistency with the rest of the library.
    - So, if you had (self, button, interaction) as a callback in a View it should change to (self, interaction, button).
- StoreChannel has been removed.
- ChannelType.store has been removed.
- StoreChannelConverter has been removed.
- A lot of method parameters were changed to be positional only.
    - Chances are very high this does not affect you.

**New Features**

- Allow Transformer.transform to be a sync method as well as a coroutine.
- Add cover_image to AuditLogDiff.
- Add app_commands.rename decorator to give a parameter a different name than the one in the function.
- Add some built-in checks in the new app_commands.checks package:
    - app_commands.checks.has_permissions
    - app_commands.checks.bot_has_permissions
    - app_commands.checks.has_role
    - app_commands.checks.has_any_role
    - app_commands.checks.cooldown
    - app_commands.checks.dynamic_cooldown
    - These work similar to the ext.command counterpart.
    - All of these are checks done locally in the program. Discord is not aware of it.
- Add CommandTree.interaction_check callback to implement global checks.
    - Using this requires subclassing the CommandTree.
- [commands] Add tree_cls keyword argument to pass a custom CommandTree subclass type for the bot provided tree.

**Bug Fixes**

- Fix audit logs for INVITE_CREATE returning a None target.
- Fix context menu names not allowing characters like ? and !.
- Errors that happen during a Transformer invocation will be wrapped in a TransformerError if they don't inherit from AppCommandError.
- Fix errors raised when receiving a message from a voice channel.
- Fix multiple 3.10 union annotation parameters causing an error due to mishandling of annotation resolver cache.
- [commands] Fix help command errors and invoke hooks not running.
{{< /tip >}}

{{< /column >}}
{{< /block >}}
