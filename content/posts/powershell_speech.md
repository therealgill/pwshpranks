---
date: 2025-02-07T06:28:34-06:00
description: Make a remote system 'speak'
lastmod: 2025-02-07
showTableOfContents: false
tags:
  - Speech
  - Audio
title: Make a System 'Speak'
type: post
---
<base target="_blank">
# Description

This will cause a system to 'say' a phrase.

``` powershell
Add-Type -AssemblyName System.speech
$speak = New-Object System.Speech.Synthesis.SpeechSynthesizer
$speak.Speak("INSERT SPEECH TEXT HERE") 
```

### Source
[Reddit](https://www.reddit.com/r/PowerShell/comments/5z55g4/need_a_fun_prank_script/)