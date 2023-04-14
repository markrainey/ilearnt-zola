+++
title="Fix default Android emulator not showing in Visual Studio 2022"
date=2022-12-15
authors = ["Mark Rainey"]
[taxonomies]
categories=["howto","coding"]
tags=[]

+++

I am working on a Maui application in my spare time and Visual Studio has this annoying habit of not showing the default Android emulator when I load the project. I could go through the hassle of creating a new emulator each time but that is painful and slow.

<!-- more -->

I scanned for solutions and looked at things like the Android subsystem for Windows and while doing so I accidentally stumbled on a simple solution.

In Visual Studio, select *Tools/Android/Android adb command prompt*. For some reason this causes Visual Studio to recognise the previously created emulator. You can then close the command prompt.