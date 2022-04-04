+++
title="Discord Models"
weight=16
+++

Models are classes that are received from Discord and are not meant to be created by the user of the library.

{{< tip "warning" >}}
The classes listed below are **not intended to be created by users** and are also **read-only**.

For example, this means that you should not make your own `User` instances nor should you modify the `User` instance yourself.

If you want to get one of these model classes instances they’d have to be through the cache,
and a common way of doing so is through the `utils.find()` function or attributes of model classes that you receive from the events specified in `Event Reference`.
{{< /tip >}}

{{< tip >}}
Nearly all classes here have \__slots__ defined which means that it is impossible to have dynamic attributes to the data classes.
{{< /tip >}}

### ClientUser
<hr>
