+++
title = "Eruption"
slug = "landing"
paginate_by = 5
weight = 0
author = "X3n0m0rph59"
date = 2022-05-09
+++


### Linux user-mode input and LED driver

Eruption is a Linux daemon written in the Rust programming language.

Eruption consists of a core daemon with an integrated Lua interpreter, and additional plugin components. Its intended usage is to execute Lua scripts that may react to certain events on the system like e.g. Timer tick, Key pressed or Mouse moved and subsequently control the connected LED devices and/or transform the user input via the integrated programmable macro feature. Eruption plugins may export additional functionality to the Lua scripting engine. Multiple Lua scripts may be run in parallel, each one in its own VM thread. A Lua script shall compute some kind of effect resulting in a 'color map'. Each Lua scripts 'submitted color map' will be combined with all other scripts 'submitted color maps' using a compositor that performs an alpha blending step on each 'color map' before it finally gets sent to the connected LED devices.

<div class="spacer-xxs"></div>

<div class="d-flex justify-content-center">
    <a class="viewMoreButton animate__animated animate__fadeInDown animate__delay-4s" onclick="document.getElementById('player').scrollIntoView(false);">See a Demo Video</a>
</div>


<div class="spacer-xs"></div>

<div>
    <iframe id="ytplayer" type="text/html" width="100%" height="720px"
    src="https://www.youtube.com/embed/ig_71zg14nQ?autoplay=1&origin=https://eruption-website.vercel.app/"
    frameborder="0"></iframe>
</div>

<div id="player"  class="spacer-xs"></div>

#### Features Overview

* Integrated Lua interpreter
* LED Control via Lua scripts
* Macros via Lua scripts
* Multiple Lua scripts may be executed in parallel, with their outputs and effects combined
* Allows for construction of complex "effect pipelines"
* Event-based architecture
* Daemon plugins may export functions to Lua
* Profiles may be switched at runtime via a D-Bus method
* A GNOME based profile switcher extension is available

<div id="player"  class="spacer-xs"></div>

#### System requirements

* What does Eruption need to run?


  Some of the profiles require a CPU built later than 2015 with support for SIMD/AVX2