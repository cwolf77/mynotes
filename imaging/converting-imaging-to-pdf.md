# Image convertion

## Convert to pdf

`#!/bin/bash`

``convert `ls -v *.jpg` tmp_outfile.pdf``

`convert-density 200x200 -quality 30 -compress jpeg tmp_outfile.pdf $1`

## Convert to a lower quality image

`convert img.jpg -quality 50 img-lower-quality.jpg`

