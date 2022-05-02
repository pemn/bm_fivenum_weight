# bm_fivenum_weight
weighted fivenum statistics (min,mean,max,std,var)
## Objective
Descriptive statistics.
## Screenshot
[screenshot1](./assets/screenshot1.png?raw=true)
## Usage
* input: a database in a known format (csv, xls, bmf, 00t, 00g, isis, msh, dm)
 * condition: optional expression to filter. syntax is vulcan (bmf) or python (csv,isis)
 * lito: one or more classification variables that will break data into multiple tables (optional)
 * weight: variable that will be used as the weight on averages and sums (optional)
 * variables: a list of grade variables to analise
 * output: (optional) file to write the result: csv or xlsx
 * keep_null: dont exclude -99 values from calculations
## Example1
[screenshot2](./assets/screenshot2.png?raw=true)
## Example2
[screenshot3](./assets/screenshot3.png?raw=true)
