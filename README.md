# scantools

A series of tools to improve film scanning.

includes the following:

- stripscan
- framescan
- profilescan
- invertscan
- takepicture
- scantool

stripscan

    turns the multiple strips of film on a flat bed into single strips

    e.g. usage:

    stripscan -s 2 -r 90 somefile.tif

    "bin" half the pixels, rotate 90

    currently gives acceptable speed at 2400dpi, but is designed to process the scan at the hightest resolution. 

framescan:

    framescan  somefile_strip.tif

profilescan:

    creates profile information for later use

invertscan:

    inverts a scan using a variety of different approaches, which is controlled by flags

    invertscan -c3 someneg.tif

takepicture:

    creates a "digital negative" purely for trying ideas out.

    takepicture some.jpg

scantool:

    does it all in one go:

    for foo in n10_757_a_full4800_exp1_*.tif;do scantool $foo;done
