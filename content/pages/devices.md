+++
title = "Device Compatibility"
path = "devices"
slug = "devices"
paginate_by = 5
weight = 5
author = "X3n0m0rph59"
date = 2022-05-11
+++

### Keyboards

| Vendor  | Product                | Status                     | Macro Keys | Easy Shift Key | Switch Profiles via F1-F4 Keys | Special functions via F5-F8 Keys    | Media keys F9-F12 |
| ------- |------------------------| -------------------------- | ---------- | -------------- | ------------------------------ | ----------------------------------- | ----------------- |
| ROCCAT  | Vulcan 100/12x         | 100%                       | Yes        | Yes            | Yes                            | Yes                                 | Yes               |
| ROCCAT  | Vulcan Pro TKL         | 98%                        | No         | Yes            | Yes (*inofficial)              | No, but may be forced (*inofficial) | Yes               |
| ROCCAT  | Vulcan TKL             | work-in-progress, untested | No         | Yes            | Yes (*inofficial)              | No, but may be forced (*inofficial) | Yes               |
| ROCCAT  | Vulcan Pro             | work-in-progress, untested | Yes        | Yes            | Yes                            | Yes                                 | Yes               |
| ROCCAT  | Magma                  | work-in-progress, untested | Yes        | Yes            | Yes (*inofficial)              | Yes                                 | Yes               |
| Corsair | Strafe Gaming Keyboard | 35%, work-in-progress      | No         | No             | No                             | No                                  | No                |

<p class="annotation">* This feature is not supported/endorsed by the OEM and may be subject to change.</p>

<div class="spacer-xs"></div>

### Mice

| Vendor | Product              | Status | Profiles | DPI  | Poll Rate | Debounce | Angle snapping | DCU | Macro Keys | Easy Shift Key |
| ------ |----------------------| ------ | -------- | ---- | --------- | -------- | -------------- | --- | ---------- | -------------- |
| ROCCAT | Kone Pure Ultra      | 100%   | Yes      | Yes  | TODO      | Yes      | Yes            | No  | N.a.       | N.a.           |
| ROCCAT | Burst Pro            | 100%   | Yes      | Yes¹ | No        | No       | No             | No  | N.a.       | N.a.           |
| ROCCAT | Kain 100 AIMO        | 80%    | No       | No   | No        | No       | No             | No  | N.a.       | N.a.           |
| ROCCAT | Kain 2xx AIMO        | 80%    | No       | No   | No        | No       | No             | No  | N.a.       | N.a.           |
| ROCCAT | Kone XP              | ??%    | Yes      | No   | No        | No       | No             | No  | N.a.       | N.a.           |
| ROCCAT | Kone Pro             | ??%    | Yes      | No   | No        | No       | No             | No  | N.a.       | N.a.           |
| ROCCAT | Kone Pro Air         | ??%    | No       | No   | No        | No       | No             | No  | N.a.       | N.a.           |
| ROCCAT | Kone Aimo            | 80%    | No       | No   | No        | No       | No             | No  | N.a.       | N.a.           |
| ROCCAT | Kone Aimo Remastered | 80%    | No       | No   | No        | No       | No             | No  | N.a.       | N.a.           |
| ROCCAT | Kova AIMO            | 80%    | No       | No   | No        | No       | No             | No  | N.a.       | N.a.           |
| ROCCAT | Kova 2016            | ??%    | No       | No   | No        | No       | No             | No  | N.a.       | N.a.           |
| ROCCAT | Kone XTD             | N.a    | No       | No   | No        | No       | No             | No  | N.a.       | N.a.           |

<p class="annotation">
* This feature is not supported/endorsed by the OEM and may be subject to change.
</p>

<p class="annotation">
¹ Only supported via the profile switching mechanism
</p>

<p class="annotation">
Profiles: Switch between hardware profiles, DPI: Pointer resolution, Debounce: Debouncing of button switches,
Angle snapping: stabilize pointer movement, DCU: Distance Control Unit settings
</p>

<div class="spacer-xs"></div>

### Miscellaneous Devices

| Vendor                | Product            | Status | Device Type                 |
| --------------------- | ------------------ | ------ | --------------------------- |
| ROCCAT / Turtle Beach | Elo 7.1 Air        | 50%    | Headset (Wireless)          |
| ROCCAT                | Sense AIMO XXL (Aimo Pad Wide) | 95%    | Misc device (Mousepad)      |
| Adalight / Custom     | Custom serial LEDs | 95%    | LED Strip (variable length) |

<p class="annotation">* This feature is not supported/endorsed by the OEM and may be subject to change.</p>

<div class="spacer-xs"></div>

### Enabling Experimental Drivers

**Experimental** drivers are **disabled** in the default configuration. To enable support for experimental drivers, please edit the configuration file
`/etc/eruption/eruption.conf` and set the following value:

```toml

[global]
driver_maturity_level = "experimental"
```

<div class="spacer-xs"></div>
