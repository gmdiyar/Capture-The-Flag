# Dresden puzzle full solution

Start file: `dresden.jpg` 

## Layer 1

Caesar Cipher

`KNNJ CDDODQ SGZM SGD OGNSN`
"The wheel has turned 3301 times." key = 3301
**LOOK DEEPER THAN THE PHOTO**

## Layer 2

the file is also a valid ZIP.

- Rename `dresden.jpg` to `dresden.zip` and open it.
- Or upload it to aperisolve.com, whose binwalk/foremost output shows the embedded ZIP and PNG.

Inside the ZIP: `the_weeders.png`

## Layer 3

The lowest bit of the red channel holds a QR code in the middle of the image.

- Upload `the_weeders.png` to aperisolve.com or StegOnline (georgeom.net/StegOnline) and look at the **Red bit plane 0**.
- Scan the QR code with your phone camera. It says **today**.

The PNG's metadata comment (shown by exiftool or Aperi'Solve) says *"The moon is still keeping a secret."* That points back to the moonlit Dresden image.

## Layer 4

Upload `dresden.jpg` to boxentriq.com/steganography/outguess-extractor with the passphrase **today** (lowercase).

Output:

> You came back to the moon. Well done.
> The flag is: SEVENTEEN YEARS UNDERGROUND
