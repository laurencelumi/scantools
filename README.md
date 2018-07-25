# scantools

A series of tools to improve film scanning.

includes the following:

- scantool
- vtrimscan
- invertscan

- profilescan
- takepicture

scantool:

    takes a single scan of multiple films strips removes the holder and seperats each frame and inverts it

    scantool both fullscan.tif
    scantool both -p profile dmax 1.8 fullscan.tif prefix_used_output_files

    or

    scantool frames fullscan.tif

vtrimscan

    removes the film holder and seperates film from a scan containing multiple images

    e.g. usage:

     vtrimscan holder fullpage.tif

     trims the film vertically in to strips removing the holder frame holder between film strims

     vtrimscan holder -r 90 fullpage-strip-1.tif

     rotates the a film strip 90 degrees then removes the film holder from ends

     vtrimscan gap strip-1.tif

     seperates each frame and trims the film

invertscan:

    inverts a scan using a variety of different approaches, which is controlled by flags

    invertscan -c3 someneg.tif

profilescan:

    creates profile information for later use

takepicture:

    creates a "digital negative" purely for trying ideas out.

    takepicture some.jpg

