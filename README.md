### some configs and scripts I use on my MacBookPro12,1 (early 2015 Retina MBP 13")


to apply dwm and st patches I use the following approach
* copy patches needed to /etc/portage/patches/x11-wm/dwm-6.1/*
* assign numbers to patch files so they can apply in correct order

```bash
USE=-savedconfig emerge x11-wm/dwm
```

* modify /etc/portage/savedconfig/x11-wm/dwm-6.1 (hint: you can symling dwm-6.1 to dwm-6.1.h to get syntax highlighting in vim)
* enable savedconfig USEflag for dwm 

```bash
flaggie dwm +savedconfigi
```

* emerge dwm
* repeat for x11-terms/st
