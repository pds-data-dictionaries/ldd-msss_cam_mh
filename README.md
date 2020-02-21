# MSSS Camera Mini-header Local Data Dictionary (LDD)

This dictionary is used for a class of cameras developed by Malin Space
Science Systems (MSSS) that all share a common architecture (primarily
the Digital Electronics Assembly, or DEA).  These cameras include but
are not limited to Mastcam, MAHLI, and MARDI on MSL, and Mastcam-Z,
SHERLOC-Watson, and SHERLOC-ACI on Mars 2020.  In each, a 64-byte header
is created by the camera itself and returned along with the image data.
This "mini-header" is distinct from normal data product headers in that
it is created by the camera, rather than by the spacecraft.  In some
cases (so-called "recovered products"), this mini-header is all the
metadata that is available.  Much of the information in here is repeated
elsewhere in the label, but due to the unique nature of the mini-header
it is useful to group all items occurring in it in this dictionary.  In
general, the equivalent items elsewhere in the label should be used to
determine the state of the image (for example, compression status or
filter number) because they apply to any mission or instrument, whereas
this dictionary is specific to this particular class of cameras.

Steward: [IMG Node](https://pds-imaging.jpl.nasa.gov/)

## Released Versions

A Local Data Dictionary (LDD) is built for each version of the [PDS4 Information Model](https://pds.nasa.gov/datastandards/documents/im/).
The build process ensures compatibility of the LDD with the core information model.

This LDD has been released for the following versions of the PDS4 information model:

```
not yet released
```

## Notes

Each build is generated using the [lddtool](https://pds.nasa.gov/tools/about/ldd/) specific to a version of the [PDS4 Information Model](https://pds.nasa.gov/datastandards/documents/im/). The build command used is:

```
lddtool -lpsnJ ldd-file.xml
```
