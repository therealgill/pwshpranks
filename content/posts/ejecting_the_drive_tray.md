---
date: 2025-02-07T06:28:34-06:00
description: Eject the physical drive tray of a system
lastmod: 2025-02-07
showTableOfContents: false
tags:
  - Drive
  - Tray
  - CD
  - DVD
  - Physical
  - Hardware
title: Ejecting the Drive Tray
type: post
---
<base target="_blank">
# Description

This will eject the physical drive tray of all available "CD Drive" devices.

``` powershell
$sh = New-Object -ComObject "Shell.Application"
$sh.Namespace(17).Items() |  Where-Object { $_.Type -eq "CD Drive" } | foreach { $_.InvokeVerb("Eject") }
```

### Source
[Reddit](https://www.reddit.com/r/PowerShell/comments/5z55g4/need_a_fun_prank_script/)