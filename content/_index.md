+++
title = "Eruption"
slug = "landing"
paginate_by = 5
weight = 0
author = "X3n0m0rph59"
date = 2022-05-09
+++

## Linux user-mode input and LED driver

Eruption is a Linux daemon written in the Rust programming language.

Eruption consists of a core daemon with an integrated Lua interpreter, and additional plugin components. Its intended usage is to execute Lua scripts that may react to certain events on the system like e.g. Timer tick, Key pressed or Mouse moved and subsequently control the connected LED devices and/or transform the user input via the integrated programmable macro feature. Eruption plugins may export additional functionality to the Lua scripting engine. Multiple Lua scripts may be run in parallel, each one in its own VM thread. A Lua script shall compute some kind of effect resulting in a 'color map'. Each Lua scripts 'submitted color map' will be combined with all other scripts 'submitted color maps' using a compositor that performs an alpha blending step on each 'color map' before it finally gets sent to the connected LED devices.

[![Eruption Video](https://img.youtube.com/vi/ig_71zg14nQ/0.jpg)](https://www.youtube.com/watch?v=ig_71zg14nQ)
