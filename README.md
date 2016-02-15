# Bossy

Bossy is an easy-to-use and awesome developer- and player-friendly Bukkit Boss Bar API (wow that's a mouthful).

**Dependencies:**
* [ProtocolLib](https://www.spigotmc.org/resources/protocollib.1997/)
* Any derivative of Bukkit 1.8 ([PaperSpigot!](https://tcpr.ca/downloads/paperspigot))


**Demonstration:**

![http://imgur.com/bY9dESb.gif](http://imgur.com/bY9dESb.gif)

**Usage:** It's as easy as this!

```
Sidebar sidebar = new Sidebar();
sidebar.set(0, "Message at line #0");
sidebar.set(0, "Another message at line #0");
sidebar.set(1, ""); // empty blank line
sidebar.set(2, "A message at line #3");
sidebar.replace(0, "Replaces line #0 with this!");
sidebar.reset();
sidebar.remove("A message at line #3"); // removes that
sidebar.remove(0); // removes any at line #0
sidebar.removeAll(); // removes everything!
```
