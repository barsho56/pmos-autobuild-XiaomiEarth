# Autobuild PostmarketOS
Real autobuild pmos for mido (msm8953) with plasma-mobile, extra packages and without systemd every wednesday.

## Why?
Because I can, xd.  
- You may fork this repo, edit configs with **own** settings and don't waste the resources of your PC's (waste the resources of companies😈).  
- You don't need Linux, just download the archive, unzip the files and  
```
fastboot flash boot lk2nd.img && fastboot flash userdata qcom-msm8953.img && fastboot reboot
```
-----
Inspired by [Telegram AutoLSPatch](https://github.com/dsys1100/tg-autolspatch)