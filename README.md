# Autobuild PostmarketOS
Real autobuild pmOS for YOUR device with YOUR settings without installing anything to you PC!

## How is it better than the official builds?
You choose **YOUR OWN** settings and build when you want.

## How to use
1. Fork this repo  
2. Go to Actions, Select Build and set up configs  
3. Run workflow!  
4. After building compressed files will be in Releases with information about your settings  
5. Just unpack zip and  
```
fastboot flash boot lk2nd.img && fastboot flash userdata rootfs.img && fastboot reboot
```

## Why?
Because I can, xd  
And just for fun.

## Little help
Device is spelled “xiaomi-mido” or nowadays “qcom-msm8953” (see actual codename in [pmOS Wiki](https://wiki.postmarketos.org/wiki/Devices))  
Extra packages are listed comma-separated without spaces with the correct Alpine Packagename  
Hostname is also without spaces, it's easier to leave it as is  
Systemd - oooh, this is a hot topic for discussion, but for now I would VERY advise leaving off “never” as it doesn't work correctly on all devices. You could try turning on “always”.  
DE - everything is clear here, I like KDE Mobile, but you can install Phosh or any other, also check out the [pmOS Wiki](https://wiki.postmarketos.org/wiki/Category:Interface).  
User password is entered for pmOS user, do not enter GitHub password here. I put very simple, but you can make it more complicated, also without spaces. It's possible to change it via “passwd”  
Username is your username in pmOS, without spaces.  
Locale - system language. The interface should be in English only, so don't change it. It is possible to put for example “ru_RU”.

-----
Inspired by [Telegram AutoLSPatch](https://github.com/dsys1100/tg-autolspatch)
