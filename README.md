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

Only one LDD source version is kept such that it can be managed by github.

- [src](src)

## Versions

A Local Data Dictionary (LDD) is built for selected versions of the [PDS4 Information Model](https://pds.nasa.gov/pds4/doc/im/).
The build process insures compatiblity of the LDD with the core information model.

## Builds


This LDD has been released for the following versions of the PDS4 information model:

- [development](build/development/)
- [releases](build/release/)


## Notes

Each build is generated using the [lddtool](https://pds.nasa.gov/tools/about/ldd/) specific to a version of the [PDS4 Information Model](https://pds.nasa.gov/datastandards/documents/im/). The build command used is:

```
lddtool -lpsnJ PDS4_IMG_IngestLDD.xml PDS4_MSSS_CAM_MH_IngestLDD.xml
```

# Contribute

Have a bug or feature request? Create one in the [PDS4 Issue Repo](https://github.com/pds-data-dictionaries/PDS4-LDD-Issue-Repo/issues/new/choose).


# Support

See the [PDS Data Dictionaries Support page](https://pds-data-dictionaries.github.io/support/) for more Support information.

