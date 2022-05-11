+++
title = "Realtime RGB LED Software for Linux"
slug = "landing"
paginate_by = 5
weight = 0
author = "X3n0m0rph59"
date = 2022-05-11
+++

Eruption is a Linux daemon written in the Rust programming language.

Eruption consists of a core daemon with an integrated Lua interpreter, and additional plugin components. Its intended usage is to execute Lua scripts that may react to certain events on the system like e.g. Timer tick, Key pressed or Mouse moved and subsequently control the connected LED devices and/or transform the user input via the integrated programmable macro feature.

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


<div class="spacer-xxs"></div>

<div class="d-flex justify-content-center">
    <a class="viewMoreButton animate__animated animate__fadeInDown animate__delay-4s" onclick="document.getElementById('player').scrollIntoView(false);">View Demo Video</a>
</div>


<div class="spacer-xs"></div>

<div>
    <iframe id="ytplayer" type="text/html" width="100%" height="720px"
    src="https://www.youtube.com/embed/ig_71zg14nQ?autoplay=1&origin=https://eruption-website.vercel.app/"
    frameborder="0"></iframe>
</div>

<div id="player"  class="spacer-special"></div>


<div class="spacer-xs"></div>

#### System requirements

* What does Eruption need to run?


  Some of the profiles require a CPU built later than 2015 with support for SIMD/AVX2

<div class="spacer-xs"></div>

#### Installation

<div class="spacer-section"></div>

##### Arch Linux and derivatives like ArcoLinux or Manjaro

```shell

paru -Syu aur/eruption

systemctl --user enable --now eruption-audio-proxy.service
systemctl --user enable --now eruption-process-monitor.service

sudo systemctl enable --now eruption.service
```

<div class="spacer-section"></div>

##### Fedora based

```shell

sudo dnf copr enable x3n0m0rph59/eruption
sudo dnf install eruption

systemctl --user enable --now eruption-audio-proxy.service
systemctl --user enable --now eruption-process-monitor.service

sudo systemctl enable --now eruption.service
```

<div class="spacer-section"></div>

##### Ubuntu or Pop!_OS

```shell

sudo add-apt-repository ppa:x3n0m0rph59/eruption
sudo apt update
sudo apt install eruption

systemctl --user enable --now eruption-audio-proxy.service
systemctl --user enable --now eruption-process-monitor.service

sudo systemctl enable --now eruption.service
```

<div class="spacer-section"></div>

##### From Source

```shell

git clone https://github.com/X3n0m0rph59/eruption.git
cd eruption
make
sudo make install
make start
```

To remove Eruption from your system run:

```shell

make stop
sudo make uninstall
```

Please refer to [INSTALL.md](https://github.com/X3n0m0rph59/eruption/blob/master/docs/INSTALL.md) for further information, e.g. the dependencies you need to install to be
able to successfully build Eruption from source.

---

<div class="spacer-section"></div>

#### After Setup

You may want to try the [Eruption Profile Switcher](https://extensions.gnome.org/extension/2621/eruption-profile-switcher/)
GNOME Shell extension that enables easy switching of profiles on the fly
