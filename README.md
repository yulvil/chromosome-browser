# chromosome-browser
A chromosome browser that displays csv data (gedmatch, ftdna, myheritage) in a SVG

**Try it**: https://yulvil.github.io/chromosome-browser.html

Features
* Copy/paste your CSV data (gedmatch, familytreedna, myheritage)
* Drag and drop CSV files from your desktop
* All the rendering is done on the client side. No data sent to servers.
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

familytreedna.com segments file format
```
NAME,MATCHNAME,CHROMOSOME,START LOCATION,END LOCATION,CENTIMORGANS,MATCHING SNPS
```

myheritage.com segments file format
```
Name,"Match name",Chromosome,"Start Location","End Location","Start RSID","End RSID",Centimorgans,SNPs
```

To export your segment data (familytreedna.com)
* Sign in to familytreedna.com
* Open the Family Finder - Chromosome Browser
* Click on `Download All Matches to Excel (CSV Format)`

To export your segment data (myheritage.com)
* Sign in to myheritage.com
* Open the DNA - DNA matches
* Click on `Export shared DNA segment info for all DNA matches`

## TODO
* Sort by cM
* Make it pretty
* Fix performance problem with Compact view and cM<5
* Improve screen resize
* Improve mobile usability

## Screenshot

![Chromosome 1 Compact View](screenshot.png?raw=true "Chromosome 1 Compact View")
