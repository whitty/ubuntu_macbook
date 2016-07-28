# Ubuntu on macbook

Hardware:

 * NVidia `MacBookPro11,3`

Software:

 * Ubuntu 14.04.4 - with `-wily` X and kernel packages.

# Ubuntu packages

Start by installing these packages:


`macfanctld` - without this you may not get any fans running


# PC Niceties

To help you turn your machine into a normal PC:

## Fixing the keyboard

Fix the layout to match a normal 104 PC keyboard.  Install `hid_apple.conf` into `/etc/modprobe.d`

Enable F1-F12 function keys by default

```
options hid_apple fnmode=2
```

Put alt back next to the space-bar - option/alt becomes "windows" key.

```
options hid_apple swap_opt_cmd=1
```

For more info try `modinfo hid_apple`
