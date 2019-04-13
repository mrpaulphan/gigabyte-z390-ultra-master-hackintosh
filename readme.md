# Hackintosh 2019 Build

## Parts
https://pcpartpicker.com/user/Mrpaulphan/saved/Wc6kdC


## Overview
I followed this [article](https://hackintosher.com/builds/gigabyte-z390-aorus-ultra-i7-9700k-vega-64-hackintosh-build-guide/).


## Post Install Mojave
Remove EmuVariableUefi-64.efi from /Volumes/EFI/EFI/CLOVER/drivers64UEFI after logging in App Store, iTunes, iMessage, FaceTime, … as its only needed for activation of these apps and can actually interfere with performance.


## Personal Issues
- [Resolved] When I was doing a fresh install, I kept getting a kernal panic issue when booting from my SSD. I found out that the [Samsung 970 Evo Plus 500 GB M.2-2280 Solid State Drive was not compatiable when building a hackintosh](https://www.reddit.com/r/hackintosh/comments/aprsbp/970_evo_plus_hackintosh/). I returned my Plus and got the regular one and I was able to boot. 

- [Resolved] I've been running into a minor issue which is the hackintosh FREEZES after boot few seconds later on login screen WHEN LEFT IDLE (but doesn't usually freeze after logging in). Both keyboard and mouse become unresponsive and there's no KP logs shown on screen, I can only force restart the whole machine and login quickly once it's done booting, but it's annoying. The system would still occasionally and randomly freeze after logging in but mostly when performing tasks that takes up high resources such as video editing in Final Cut Pro X, but it freezes ALL THE TIME on the login screen after boot without logging in/left idle after seconds. I decided to keep the 970 Evo Plus as my Windows SSD. After finding a thread [this](86.com/threads/mojave-10-14-4-random-freezes-mostly-after-boot-without-logging-in-left-idle-on-login-screen.275012/#post-1940530) thread, I concluded that my mac was freaking out when trying to mount my 970 Evo Plus. Removing this SSD from my motherboard solved this issue

