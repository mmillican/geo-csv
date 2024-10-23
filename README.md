# GEO Data

This is a utility repository for me to easily copy data for populating dev data sources.

It is **not** meant to be an exhaustive list for all countries, but if you would like to contribute, please feel free to submit a PR.

## Formats

The primary format is CSV, but I plan to add more later as needed.

## CSV Spec

The CSV directory has a `countries.csv` file with the following structure

### Countries

This data is in the `csv/countries.csv` file.

| id | name | code | state_province_file_name |
| -- | ---- | ---- | ------------------------ |
| _arbitrary "pk" for reference_ | _name of the country_ | _3-letter code_ | _file name of state/provinces, if it exists_ |

### State / Provinces

| country_id | name | code |
| -- | ---- | ---- |
| _"fk" to the country id (above)_ | _name of the state/province_ | _abbrevation_ |
