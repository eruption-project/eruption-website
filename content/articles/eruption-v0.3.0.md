+++
title = "Released Eruption v0.3.0"
slug = "eruption-v0.3.0"
paginate_by = 5
weight = 20
author = "X3n0m0rph59"
date = 2022-12-02
+++

### Released Eruption v0.3.0

[Eruption v0.3.0 on GitHub](https://github.com/X3n0m0rph59/eruption/releases/tag/v0.3.0)

- Fix a locking issue that lead to excessive jitter and noticeable input lag
- Add a new user-session daemon: eruption-fx-proxy that supersedes some features of eruption-netfx
- Replace the Ambient Fx effect based on eruption-netfx and netfx.profile with the newer and more efficient Ambient Effect provided by eruption-fx-proxy
- Improve compatibility with USB HUBs and KVM switches
- Improve compatibility with laptop docks
- Add support for most Wayland compositors to the eruption-process-monitor session daemon. (To enable support for automatic profile switching)
- Improve stability of some drivers, most notably: ROCCAT Kone Pro Air, ROCCAT/Turtle Beach Elo 7.1 Air
- Further reduce CPU load of the eruption daemon by only trying to invoke Lua event handler functions that actually exist. Thanks to Phen-Ro for implementing this!
- Add a table view to eruptionctl used for showing script and profile parameters. Thanks to Phen-Ro for implementing this!
- Improve parameter handling in eruptionctl. Thanks to Phen-Ro for implementing this!
- Switch the hidapi backend from libusb to the linux-specific hidapi-hidraw
- Add a new companion utility eruption-macro that allows to record macros, which then can be assigned using the eruption-keymap utility
- Ship an initial technology preview version of the new Pyroclasm UI
- Allow to configure the fade duration or to completely disable fading when switching profiles. Thanks to Phen-Ro for implementing this!
- Eruption SDK: Add APIs for switching profiles and for modifying configuration parameters. Thanks to Phen-Ro for implementing this!
- Eruption SDK: Improve the Python 3 SDK and publish it on <https://pypi.org/project/eruption-sdk/>
- Eruption SDK: Rename Rust package to eruption-sdk and publish on <https://crates.io/crates/eruption-sdk>
- Improve the way we handle parameters of *.profile files. Thanks to Phen-Ro for implementing this!
- New Lua scripts: stock-gradient.lua linearly interpolates colors from a pre-defined color scheme or from a stock gradient
- New profile: rainbow-vertical.profile that makes use of the newly introduced Lua script that renders stock gradients and custom color schemes
- Update all dependencies to their latest releases
- New theme for the eruption CLI tools (--help) output, provided by Clap v4
- Bump MSRV to latest stable Rust 1.64
