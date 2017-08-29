# chromosome-browser
A chromosome browser that displays csv data (gedmatch, ftdna) in a SVG

Features
* Import CSV data
* Filter by centimorgan (cM)
* Include or exclude kits (persons)
* Different views (compact, by kit, ordered by segment)

### CSV data

Formats supported are
```
"chr","start","end","cm","kit","name"
1,72017,3230059,8.1,"ABC123","John Doe"
1,92017,13771690,9.9,"DEF456","Alice Bob"
```

familytreedna.com export format
```
NAME,MATCHNAME,CHROMOSOME,START LOCATION,END LOCATION,CENTIMORGANS,MATCHING SNPS
```
