+++
title = "Meeting Notes - July 2025"
date = "2025-07-14T16:00:00-05:00"
tags = ["meeting-notes"]
categories = ["Meeting Notes"]
banner = "img/banners/note-icon.jpg"
authors = ["EC Linux"]
summary = "This is our monthly meeting notes post. You will find the topics discussed along with links to relevant topics brought up in our discussions. Hopefully, this will help those who were not able to attend or refresh the memory of those that did. We hope you will join us in person for our next meeting. If you find an error or need to add anything to these notes, please let us know, or open an issue or pull request on our [Github page](https://github.com/brettrbarker/eclinux.org)."
+++
## Business Items

**Next Meeting:** August 12, 2025 @6PM

**Location:** Beachside Community Church

* * *

Items discussed:

Kevin showed off his local LLM installed on Ubuntu.

[Ollama](https://ollama.com/)

Aaron also provided easy NixOS config to get it up and running on NixOS.

```Nix
    services.ollama = {
      enable = true;
      #package = pkgs.unstable.ollama;
      package = pkgs.ollama;
    };
```
