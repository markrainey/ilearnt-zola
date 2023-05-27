+++
title="Show seconds in the Windows 11 taskbar"
date=2023-05-29
authors = ["Mark Rainey"]
[taxonomies]
categories=["technology","howto"]
tags=[]
+++

I noticed the other day that my wife's laptop was showing seconds in the time in the taskbar but my laptop was not; a very handy feature to have.

<!-- more -->

I checked I had the latest update (22621.1702). I then searched online and most places said there should be an option under the taskbar behaviours section of settings to enable it. I went there and it wasn't present. Back to googling.

It seems like [others](https://geekermag.com/how-to-show-seconds-in-windows-11-taskbar-clock/) have encountered this and there is a registry fix for this. It involves running regedit and then navigating to the section:

> HKEY_CURRENT_USER\\Software\\Microsoft\\Windows\\CurrentVersion\\Explorer\\Advanced

Once there, if there is no entry called "ShowSecondsInSystemClock" then add a new DWORD. Set this to 1. Some guides say a reboot is needed but my change showed up immediately.

__Links__

[How to Show Seconds in Windows 11 Taskbar Clock](https://geekermag.com/how-to-show-seconds-in-windows-11-taskbar-clock)/
