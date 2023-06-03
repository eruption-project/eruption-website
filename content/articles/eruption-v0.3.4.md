+++
title = "Released Eruption v0.3.4"
slug = "eruption-v0.3.4"
paginate_by = 5
weight = 20
author = "X3n0m0rph59"
date = 2023-05-28
+++

### Released Eruption v0.3.4

[Eruption v0.3.4 on GitHub](https://github.com/X3n0m0rph59/eruption/releases/tag/v0.3.4)

- This release should fix at least one scenario where Eruption failed to fully initialize a device when that device was not yet ready during bootup of the system
- Improve the stability of the `eruption-fx-proxy` session daemon
- Update all dependencies to their latest releases

## Please Note:

If you are using the [Eruption Profile Switcher GNOME 4x Shell Extension](https://extensions.gnome.org/extension/2621/eruption-profile-switcher/) you may receive the spurious message 'Ambient effect disabled'. In this case you can disable the `eruption-fx-proxy` session-daemon using the following command:

```sh
  systemctl --user disable --now eruption-fx-proxy.service
```
> Please note that you do not need to put `sudo` in front of the aforementioned command, since it should act on the current user's session and not on the system wide configuration
