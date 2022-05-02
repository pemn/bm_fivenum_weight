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
## Saample Data
topo|lito|length|gradeA|gradeB|gradeC
---|---|---|---|---|---
1|low|9|10|69|0.677381478
1|medium|14|20|27|0.863516924
1|high|7|30|1|0.516238426
0|low|7|40|20|0.196520844
0|medium|12|50|58|0.566308143
0|high|7 60|83|0.313694847
## Example1
[screenshot2](./assets/screenshot2.png?raw=true)
## Example2
[screenshot3](./assets/screenshot3.png?raw=true)
