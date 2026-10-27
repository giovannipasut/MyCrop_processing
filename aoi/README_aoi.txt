AOI BOUNDARIES — FIELD VS. CROP
=================================

This folder contains the two boundary files used to define the spatial extent
of the MyCrop analyses.

1. field_boundary.gpkg
----------------------
Represents the boundary of the entire agricultural field. Use this boundary
when an operation needs to consider the full field extent, including areas
outside the cultivated crop area.

2. crop_boundary.gpkg
---------------------
Represents only the area occupied by the specific cultivated crop. Use this
boundary when an analysis should be limited to the cultivated area and exclude
uncultivated parts of the field.

Key distinction
---------------
field_boundary = the whole field.
crop_boundary  = only the cultivated area within the field.

Keep both files in this aoi/ folder at the root of the MyCrop-Processing
project, alongside the data/ and notebooks/ folders. Preserve the exact
filenames because processing scripts may refer to them.

Example project layout
----------------------

MyCrop-Processing/
├── aoi/
│   ├── README_aoi.txt
│   ├── field_boundary.gpkg
│   └── crop_boundary.gpkg
├── data/
├── notebooks/
└── requirements.txt

Note: Publish these boundary files to GitHub only if you have permission to
share them. Otherwise, keep them locally and document how to obtain them.
