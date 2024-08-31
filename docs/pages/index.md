---
layout: page
title: Home
permalink: /
description: "Godot State Charts is a plugin for Godot Engine that allows you to use state charts in your game."
---

# {{ site.title }}

<style type="text/css">
img {
    align: center;
    display: block;
    margin-left: auto;
    margin-right: auto;
}
</style>

**If you prefer to learn in video form, there is also a [video tutorial available on YouTube](https://www.youtube.com/watch?v=E9h9VnbPGuw) to get you started.**

{{ page.description }}
Now what is a state chart? [Statecharts.dev](https://statecharts.dev/) explains it like this:

> Put simply, a state chart is a beefed up state machine.  The beefing up solves a lot of the problems that state machines have, especially state explosion that happens as state machines grow.

Godot State Charts allows you to build state charts in the Godot editor.  The library is built in an idiomatic way, so you can use nodes to define states and transitions and use Godot signals to connect your code to the state machine. As states and transitions are nodes you can also easily modularize your state charts by using scenes for re-using states and transitions.

There is only a single class with two methods for your code to interface with the state chart. This makes it easy to integrate state charts into your game, as you don't need to extend from a base class or implement an interface for your states.

## Index

{%- for section in site.data.toc %}
- [{{ section.title }}]({{ section.url }})
{%- if section.links %}
    {%- for link in section.links %}
    - [{{ link.title }}]({{ link.url }})
    {%- endfor %}
{%- endif %}
{%- endfor %}