# scantools

A series of tools to improve film scanning.

includes the following:

- vtrimscan
- profilescan
- invertscan
- takepicture
- scantool

vtrimscan

    removes the film holder and seperates film from a scan containing multiple images

    e.g. usage:

     vtrimscan holder fullpage.tif

     trims the film vertically in to strips removing the holder frame holder between film strims

     vtrimscan holder -r 90 fullpage-strip-1.tif

     rotates the a film strip 90 degrees then removes the film holder from ends

     vtrimscan gap strip-1.tif

     seperates each frame and trims the film

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

    or

    for foo in n10_757_a_full4800_exp1_*.tif;do scantool -m2 $foo;done
