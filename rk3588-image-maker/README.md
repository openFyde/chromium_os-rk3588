### Step-by-Step transfer ChromiumOS image to RK3588 update image

1. Compile ChromiumOS Image. You can find the image at `~/trunk/src/build/images/inaugural/latest` 
 <br>
 Sample: Test image as `chromiumos_test_image.bin`

2. Map the image partitions to Image.

```
  .map_chromiumos_image.sh <path to chromiumos_test_image.bin>
```

3. Create update image

```
  .rk3588-mkupdate.sh
```

4. Get you update.img at this directory. (not Image/update.img)
