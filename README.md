# scantools

A series of tools to improve film scanning.

includes the following:

- scantool
- invertscan

- vtrimscan
- profilescan

- takepicture

##scantool

    takes a single scan of multiple films strips removes the holder and seperates each frame and inverts it

    scantool both fullscan.tif
    scantool both -p profile dmax 1.8 fullscan.tif prefix_used_output_files

```scantool both -fb 0.85001 -dmax auto  BW_gain1_85_033.tif BW_gain1_85_034.tif n10-816```

    or

    scantool frames fullscan.tif

##invertscan

    inverts a scan using a variety of different approaches, which is controlled by flags

    invertscan -c3 someneg.tif

##vtrimscan

    removes the film holder and seperates film from a scan containing multiple images

    e.g. usage:

     vtrimscan holder fullpage.tif

     trims the film vertically in to strips removing the holder frame holder between film strims

     vtrimscan holder -r 90 fullpage-strip-1.tif

     rotates the a film strip 90 degrees then removes the film holder from ends

     vtrimscan gap strip-1.tif

     seperates each frame and trims the film

##profilescan

Creates profile information for later use

e.g. usage:

```profilescan -fb -p profile_name example_crop.tif```

creates a profile called profile_name using example_crop.tif as the input

```profilescan -fb -crop -crop 135x169+870+18213 -p profile_name example_crop.tif```
creates a profile called profile_name using cropped area from example_crop.tif as the input

```profilescan -l```

lists all existing profiles
        

##takepicture

    creates a "digital negative" purely for trying ideas out.

    takepicture some.jpg

