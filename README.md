## Overview
These are optional patches provided by the community that can be applied to the RattlesnakeOS build process. Both patches and shell scripts are supported. Credit for patch 5-7 to martepato and his fork located here: https://github.com/martepato/mtpo_community_patches

## How do I add these patches to my builds?
Add the following to end of your `rattlesnakeos-stack` config file.
```
[[custom-patches]]
repo = "https://github.com/Hammergrat7/community_patches"
patches = [
        "00001-global-internet-permission-toggle.patch",
        "00002-global-sensors-permission-toggle.patch",
        "00003-disable-menu-entries-in-recovery.patch",
        "00004-increase-default-maximum-password-length.patch",
        "00005-enable-powersaving-features.patch",
        "00006-use-cloudflare-dns.patch",
        "00007-disable-agps.patch"
]
```
## Submitting Community Patches
Rules for submitting a patch:
* Patches should have a number and name describing patch (e.g. 00002-description-of-patch.patch)
* Patches should be fully tested with a build using latest version of rattlesnakeos-stack
* Patches need to assume it is going to be applied from the <b>root of the AOSP build directory</b>. You can look at existing patches to get an idea of how that looks.

## Contributors
* martepato - https://github.com/martepato
