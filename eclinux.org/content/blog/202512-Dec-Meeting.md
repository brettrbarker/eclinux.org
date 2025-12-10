+++
title = "Meeting Notes - December 2025"
date = "2025-12-08T16:00:00-05:00"
tags = ["meeting-notes"]
categories = ["Meeting Notes"]
banner = "img/banners/note-icon.jpg"
authors = ["EC Linux"]
summary = "This is our monthly meeting notes post. You will find the topics discussed along with links to relevant topics brought up in our discussions. Hopefully, this will help those who were not able to attend or refresh the memory of those that did. We hope you will join us in person for our next meeting. If you find an error or need to add anything to these notes, please let us know, or open an issue or pull request on our [Github page](https://github.com/brettrbarker/eclinux.org)."
+++
## Business Items

**Next Meeting:** January 12, 2026 @6PM

**Location:** Beachside Church

* * *

Items discussed:

Tonight we discussed my AI vibe coded NixOS machine that runs
a kiosk for my church production room. It will show
Planning Center Live and Ableset in two different kiosk windows.
The trouble I was having was how to make it switch the focus
between the two windows via ssh command. It did not want to do
this due to Wayland and setting the active display.

To work around this, we created a local user service that can then
be run via ssh with a command such as 

```bash
ssh production@kiosk-pclive systemctl --user start focus-pcolive
```

This Worked!

Aaron also showed his recent Nix config changes including things like:

```conf
nix.settings.auto-optimise-store = true;
nix.optimise.automatic = true;
```