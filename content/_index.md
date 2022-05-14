+++
title = "Realtime RGB LED Driver for Linux"
slug = "landing"
paginate_by = 5
weight = 0
author = "X3n0m0rph59"
date = 2022-05-11
+++

**What is Eruption?**

Eruption consists of a core daemon providing an integrated Lua interpreter and additional plugin components. Its primary usage is to execute Lua scripts that may react to certain **events** on the system like e.g. `Timer tick`, `Key press` or `Mouse move` and subsequently control the connected **devices** and transform the user input via the integrated **programmable macro** feature.

#### Features in a Nutshell

* **Various LED effects** available, including a **Spectrum Analyzer** and a **VU-Meter**
* **Ambient effect** via **Network FX** client (**X11 screen's** **contents** displayed on the keyboard)
* Effects are implemented as **Lua scripts** running inside of **Lua VMs**
* **Lua support library** written in **Rust** (Math, color handling, noise functions, etc...)
* Multiple effects and macro **Lua scripts** are combined to a single **profile**
* **Profiles** may change configuration parameters of **Lua scripts** (e.g.: Colors, timing parameters)
* A **profile** can be assigned to one of **four slots**
* **Macro keys** are supported and **freely programmable** via Lua functions
* Up to **6** freely configurable and switchable **macro layers**
* Packages available for: **Arch Linux**, **Ubuntu**, **Fedora**
* License: **GPL3+**

<div class="spacer-button"></div>

<div class="d-flex justify-content-center">
    <a class="viewMoreButton animate__animated animate__fadeInDown animate__delay-4s" onclick="document.getElementById('player').scrollIntoView(false);">View Demo Video</a>
</div>

<div class="spacer-padding"></div>

<div class="scroll-reveal">
    <iframe id="ytplayer" type="text/html" width="100%" height="720px"
    src="https://www.youtube.com/embed/ig_71zg14nQ?autoplay=1&origin=https://eruption-project.org/"
    frameborder="0"></iframe>
</div>

<div id="player" class="spacer-special"></div>

<div class="spacer-padding"></div>

#### System requirements

What does Eruption require to run?

Some of the **profiles** require a CPU built **later than 2015** with support for **SIMD/AVX2**

<div class="spacer-xs"></div>

# Installation

<br/>

##### Arch Linux and derivatives like ArcoLinux or Manjaro

```sh

paru -Syu aur/eruption

systemctl --user enable --now eruption-audio-proxy.service
systemctl --user enable --now eruption-process-monitor.service

sudo systemctl enable --now eruption.service
```

<div class="spacer-section"></div>

##### Fedora based

```sh

sudo dnf copr enable x3n0m0rph59/eruption
sudo dnf install eruption

systemctl --user enable --now eruption-audio-proxy.service
systemctl --user enable --now eruption-process-monitor.service

sudo systemctl enable --now eruption.service
```

<div class="spacer-section"></div>

##### Ubuntu or Pop!_OS

```sh

sudo add-apt-repository ppa:x3n0m0rph59/eruption
sudo apt update
sudo apt install eruption

systemctl --user enable --now eruption-audio-proxy.service
systemctl --user enable --now eruption-process-monitor.service

sudo systemctl enable --now eruption.service
```

<div class="spacer-section"></div>

##### Build from Source

```sh

git clone https://github.com/X3n0m0rph59/eruption.git
cd eruption
make
sudo make install
make start
```

To remove Eruption from your system run:

```sh

make stop
sudo make uninstall
```

Please refer to [INSTALL.md](https://github.com/X3n0m0rph59/eruption/blob/master/docs/INSTALL.md) for further information, e.g. the dependencies you need to install to be
able to successfully build Eruption from source.

<div class="spacer-section"></div>

#### After the Setup

You may want to try the [Eruption Profile Switcher](https://extensions.gnome.org/extension/2621/eruption-profile-switcher/)
GNOME Shell extension that enables easy switching of profiles on the fly!
