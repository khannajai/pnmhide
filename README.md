# pnmhide
Steganograhy in C: hide text in an image file

## Build and run
```
$ mkdir build && cd build
$ cmake ..
$ make
```

Hide the text "hello world" in the stegotext image stego.pnm
```
$ pnmhide -e "hello world" cover.pnm > stego.pnm
```

Retrieve the hidden text from the stegotext image stego.pnm
```
$ pnmhide -d stego.pnm
```

Detect if there is no hidden text in an image (do not produce garbage)
```
pnmhide -d cover.pnm
```