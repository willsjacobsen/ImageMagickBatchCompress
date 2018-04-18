# ImageMagickBatchCompress
Script to Batch Compress Images


Install Image Magick on your machine - https://www.imagemagick.org/script/download.php

In the command line, navigate to the directory holding your images.

Run the following code in the command line:

magick mogrify -filter Triangle -define filter:support=2 -unsharp 0.25x0.25+8+0.065 -dither None -posterize 136 -quality 50 -define jpeg:fancy-upsampling=off -define png:compression-filter=5 -define png:compression-level=9 -define png:compression-strategy=1 -define png:exclude-chunk=all -interlace none -colorspace sRGB -strip *.jpg *.jpeg



The '-quality 50' value you can be changed. For example, change it to '-quality -75' if you only want to compress by 75%. 




