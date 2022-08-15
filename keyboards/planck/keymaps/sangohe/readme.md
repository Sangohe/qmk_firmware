# Sangohe Planck Layout

## Linux

First compile the layout into a binary file
```
qmk compile -kb planck/rev6_drop -km sangohe
```

Then put your keyboard into boot mode and execute the following command to flash it:

```
sudo dfu-util -a 0 -d 03A8:A4F9:0006 -s 0x8000000:leave -D /home/sangohe/Documents/Projects/qmk_firmware/.build/planck_rev6_drop_sangohe.bin
```
