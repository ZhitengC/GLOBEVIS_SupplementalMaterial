# Annotation Schema

This document defines the operational schema used in `annotations/Annotations_Full/*.json`.

## Organization
<br/>

- Record format (top-level fields)
- `meta` section inventory
- Core subsection fields
- Missingness conventions
- Consistency requirements

## Record Format

Each locale file is a JSON array of annotation records. Each record contains:

- `image` (string) - image filename in `images/ChartImages_Full_LowRes/`
- `source` (string) - source URL
- `meta` (object) - structured annotation metadata

## `meta` Sections

- `title`
- `chart_type`
- `writing_and_reading_direction`
- `number`
- `number_complexity`
- `datetime`
- `units`
- `color_semantics`
- `axis_semantics`
- `layout_semantics`
- `visual_styling`
- `notes`
- `extracted_text`

## Core Subsection Fields

### `writing_and_reading_direction`

- `chart_text_writing_direction`
- `chart_reading_direction`
- `language_mix`
  - `mixed` (boolean)
  - `primary_language`
  - `primary_script`
  - `secondary_languages` (array)
  - `secondary_scripts` (array)

### `number`

- `related` (boolean)
- `numeral_system`
- `digit_grouping`
- `decimal_separator`
- `numeric_abbreviation` (array)
- `currency_format_related` (boolean)

### `datetime`

- `date_related` (boolean)
- `date_structure`
- `separator`
- `time_related` (boolean)
- `time_format`

### `units`

- `related` (boolean)
- `unit_combinations` (array)

### `color_semantics`

- `related` (boolean)
- `meaning_mappings` (array of objects with `color_hex` and `meaning`)


