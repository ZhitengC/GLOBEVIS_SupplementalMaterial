# Chart Source Folder

## Organization
<br/>

- `source/` - 34 locale CSV files organized by region-language pairs
  - File naming (example: `UnitedStates-English.csv`, `Germany-German.csv`, `Bangladesh-Bengali.csv`)
  - Standard columns:
    - `Image` - image filename
    - `URL` - source page URL

## Naming Convention

- CSV filenames use full region-language format (consistent with `annotations/Annotations_Full` and locale directories under `images/ChartImages_Full_LowRes`).


## Cross-Folder Linkage

- `annotations/Annotations_Full/*.json` uses image filenames that map to this folder.
- `images/ChartImages_Full_LowRes/` stores the corresponding image files.
