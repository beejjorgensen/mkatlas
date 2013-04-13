mkatlas
=======
Build poor-man's spritesheets using bash, Image Magick, and pngcrush.

Usage
-----
I use this with my `goatee` tool when building web pages. It's a little
too specialized for general consumption.

    usage: mkatlas -o outfile [options] image [image2 ...] > metadata.src.css
    
       -n val       set the namespace (prefix) for all variables
       -r val       set the relative path to the image in the CSS
       -f #rrggbb   flatten the output with the specified background

Image names can be `BR` which means to move down to the next "row"
(clearing all previously added images):

    mkatlas -o atlas.png img1.png img2.png BR img3.png img4.png

Dependencies
------------
Bash, Image Magick, and pngcrush.

