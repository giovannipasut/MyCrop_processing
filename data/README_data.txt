DATA FOLDER ORGANIZATION
========================

Store the original survey data using the following folder structure:

data/
├── 2025_flights/
│   └── flight_YYYY_MM_DD/
│       ├── YYYY_MM_DD_data/
│       ├── YYYY_MM_DD_multispectral/
│       ├── YYYY_MM_DD_thermal/
│       ├── YYYY_MM_DD_multispectral.p4d
│       └── YYYY_MM_DD_thermal.p4d
└── 2026_flights/
    └── flight_YYYY_MM_DD/
        ├── YYYY_MM_DD_data/
        ├── YYYY_MM_DD_multispectral/
        ├── YYYY_MM_DD_thermal/
        ├── YYYY_MM_DD_multispectral.p4d
        └── YYYY_MM_DD_thermal.p4d

Naming rules
------------
1. YEAR
   Create one folder for each survey year, e.g. 2025_flights or 2026_flights.

2. SURVEY DATE
   Inside the year folder, create one folder per survey using:
   flight_YYYY_MM_DD
   Example: flight_2026_05_22

3. SURVEY-SPECIFIC FILES
   Inside each survey folder, store the files and folders associated with that
   survey. Use the survey date as the filename/folder prefix:
   - YYYY_MM_DD_data
   - YYYY_MM_DD_multispectral
   - YYYY_MM_DD_thermal
   - YYYY_MM_DD_multispectral.p4d
   - YYYY_MM_DD_thermal.p4d

Replace YYYY_MM_DD with the actual survey date. Keep the naming consistent
across all surveys.

Note
----
This file documents the expected organization. Large raw imagery, Pix4D
projects, and other data should only be committed to GitHub if appropriate
and permitted. Consider keeping these datasets locally and documenting how
to obtain them instead.
