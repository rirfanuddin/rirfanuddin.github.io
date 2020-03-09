# laravel


### checking value
|           |'' or ""   |NULL       |[]         |0 OR "0"   |FALSE      |Object     |
|:---       |:---:      |:---:      |:---:      |:---:      |:---:      |:---:      |
|if()       |false      |false      |false      |false      |false      |true       |
|isset()    |true       |false      |true       |true       |true       |true       |
|is_null()  |false      |true       |false      |false      |false      |false      |
|empty()    |true       |true       |true       |true       |true       |false      |