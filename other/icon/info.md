# Icons

From the MS guidelines:

"Apps should have, at the bare minimum: 16x16, 24x24, 32x32, 48x48, and 256x256. This covers the most common icon sizes, and by providing a 256px icon, ensures Windows should only ever scale your icon down, never up."

Source: https://learn.microsoft.com/en-us/windows/apps/design/style/iconography/app-icon-construction#icon-scaling

Create windows `ico` file with `ImageMagick`:

```
magick <input-file.png> -background transparent -define icon:auto-resize="16,24,32,48,64,256" ./output.ico
```
