# AutoKey3D

## Description

AutoKey3D (formerly known as PhotoBump) is a software to create 3D models for
key blanks, bumpkeys and regular keys.

This Fork will use for the AKAB (All Keys are beautiful) project to milling key profiles.

### About

Written by Christian Holler (:decoder). For questions, send an email to:

`decoder -at- own-hero -dot- net`

The software was first presented and demonstrated at LockCon 2014, Sneek, NL.

The recorded talk is available here: https://www.youtube.com/watch?v=3pSa0pslxpU

## Requirements

* OpenSCAD (a version > 2014.03 taken from GIT or daily snapshots is recommended)
* pstoedit
* Inkscape
* Python >= 2.7

## Example

In order to create the 3D model for the bump key that was used in my video,
you can run the following command:

`python AutoKey.py --bumpkey --profile profiles/ABUS-AB95.svg --definition definitions/ABUS-E20.scad`

Once OpenSCAD has started, you can Preview/Render/Export the STL as desired.

Instead of using the `--bumpkey` parameter, you can also specify `--blank` for
creating a blank instead, or use `--key 1,2,3,4,5,6` to create a key with
the specified combination.

## Profiles

In the profiles/ subdirectory, you can find SVG traces created from photos for
certain locks. You can add your own SVG data there if you wish to create a
model for a profile not supported yet by the software. In addition to the SVG,
there is always a profile definition file (.def) that contains dimensional
information about the profile (see profiles/README for more information).

## System Definitions

The definitions/ subdirectory contains system definitions for certain locks.
Such a definition typically contains information such as the key length, the
pin/shoulder distances, key cut heights and angles. For bump keys, it is
possible to deviate from the regular system definitions for better results.

Also see definitions/README for a more detailed documentation.
