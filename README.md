# bm_fivenum_weight
weighted fivenum statistics (min,mean,max,std,var)
## Objective
Descriptive statistics.
## Screenshot
![screenshot1](./assets/screenshot1.png?raw=true)
## Usage
* input: a database in a known file format:
   - csv (headered ascii)
   - xlsx (headered excel table)
   - bmf (vulcan block model)
   - isis (vulcan table)
   - dm (datamine table)
 * condition: optional expression to filter. syntax is vulcan (bmf) or python (csv,isis)
 * lito: one or more classification variables that will break data into multiple tables (optional)
 * weight: variable that will be used as the weight on averages and sums (optional)
 * variables: a list of grade variables to analise
 * output: (optional) file to write the result: csv or xlsx
 * keep_null: dont exclude -99 values from calculations
## Sample Data
topo|lito|length|gradeA|gradeB|gradeC
---|---|---|---|---|---
1|low|9|10|69|0.677381478
1|medium|14|20|27|0.863516924
1|high|7|30|1|0.516238426
0|low|7|40|20|0.196520844
0|medium|12|50|58|0.566308143
0|high|7|60|83|0.313694847
## Example1
![screenshot2](./assets/screenshot2.png?raw=true)  
  
null|variable|count|mean|min|q1|q2|q3|max|var|std
---|---|---|---|---|---|---|---|---|---|---
0|gradeA|6|35|10|22.5|35|47.5|60|350|18.70828693
0|gradeB|6|45|6|6.5|40|81|94|1812.4|42.57229146
0|gradeC|6|0.363161953|0.149790216|0.189887634|0.287176466|0.481167815|0.75153895|0.055583222|0.235760943
  
## Example2
![screenshot3](./assets/screenshot3.png?raw=true)  
  
lito|variable|count|mean|min|q1|q2|q3|max|var|std
---|---|---|---|---|---|---|---|---|---|---
high|gradeA|2|45|30|37.5|45|52.5|60|450|21.21320344
low|gradeA|2|25|10|17.5|25|32.5|40|450|21.21320344
medium|gradeA|2|35|20|27.5|35|42.5|50|450|21.21320344
high|gradeB|2|50|6|28|50|72|94|3872|62.22539674
low|gradeB|2|46|8|27|46|65|84|2888|53.74011537
medium|gradeB|2|39|6|22.5|39|55.5|72|2178|46.66904756
high|gradeC|2|0.450664583|0.149790216|0.300227399|0.450664583|0.601101766|0.75153895|0.181050769|0.42550061
low|gradeC|2|0.287176466|0.199960489|0.243568478|0.287176466|0.330784455|0.374392444|0.015213254|0.123342019
medium|gradeC|2|0.35164481|0.186530016|0.269087413|0.35164481|0.434202208|0.516759605|0.054525791|0.233507582
  
## Example3
![screenshot4](./assets/screenshot4.png?raw=true)  
  
lito|variable|length|count|mean|min|q1|q2|q3|max|var|std
---|---|---|---|---|---|---|---|---|---|---|---
high|gradeA|30|2|41|30|30|30|60|60|450|21.21320344
low|gradeA|12|2|22.5|10|10|10|40|40|450|21.21320344
medium|gradeA|25|2|29.6|20|20|20|50|50|450|21.21320344
high|gradeB|30|2|38.26666667|6|6|6|94|94|3872|62.22539674
low|gradeB|12|2|52.33333333|8|8|84|84|84|2888|53.74011537
medium|gradeB|25|2|50.88|6|6|72|72|72|2178|46.66904756
high|gradeC|30|2|0.370431418|0.149790216|0.149790216|0.149790216|0.75153895|0.75153895|0.181050769|0.42550061
low|gradeC|12|2|0.27264047|0.199960489|0.199960489|0.199960489|0.374392444|0.374392444|0.015213254|0.123342019
medium|gradeC|25|2|0.411086137|0.186530016|0.186530016|0.516759605|0.516759605|0.516759605|0.054525791|0.233507582
  
## Repository
https://github.com/pemn/bm_fivenum_weight

