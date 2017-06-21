# Image convertion

\#!/bin/bash

convert \`ls -v \*.jpg\` tmp\_outfile.pdf

convert-density 200x200 -quality 30 -compress jpeg tmp\_outfile.pdf $1

