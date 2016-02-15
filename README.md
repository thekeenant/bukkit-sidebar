# Sidebar

Sidebar is a simple abstraction of the Bukkit scoreboard API for sidebars, developer- and player- friendly!

**Dependencies:**
* Any derivative of Bukkit 1.8 ([PaperSpigot!](https://tcpr.ca/downloads/paperspigot))


**Demonstration:**

![http://imgur.com/bY9dESb.gif](http://imgur.com/bY9dESb.gif)

**Usage:** It's as easy as this!

```
Sidebar sidebar = new Sidebar("Original title!");
player.setScoreboard(sidebar.getScoreboard());

sidebar.setTitle("Change the title!"); // max 32 chars

sidebar.set(0, "Message at line #0"); // max 48 chars (incl. colors)
sidebar.set(0, "Another message at line #0");
sidebar.set(1, ""); // empty blank line
sidebar.set(2, "A message at line #3");

sidebar.replace(0, "Replaces line #0 with this!");

sidebar.remove("A message at line #3"); // removes that
sidebar.remove(0); // removes any at line #0
sidebar.removeAll(); // removes everything!
```

**All constructors:**
```
// These create a new scoreboard
new Sidebar();
new Sidebar("Custom title!");

// These let you use your own scoreboard
new Sidebar(existingScoreboard);
new Sidebar(existingScoreboard, "Custom title!");
```
