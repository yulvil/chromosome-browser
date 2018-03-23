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

### CSV data formats

Formats supported are

familytreedna.com segments file format
```
NAME,MATCHNAME,CHROMOSOME,START LOCATION,END LOCATION,CENTIMORGANS,MATCHING SNPS
```

myheritage.com segments file format
```
Name,"Match name",Chromosome,"Start Location","End Location","Start RSID","End RSID",Centimorgans,SNPs
```

gedmatch.com segments file format
```
"kit1","name1","email1","kit2","name2","email2","chr","start","end","cm"
```

### Export segments file

To export your segment data (familytreedna.com)
* Sign in to familytreedna.com
* Open the Family Finder - Chromosome Browser
* Click on `Download All Matches to Excel (CSV Format)`

To export your segment data (myheritage.com)
* Sign in to myheritage.com
* Open the DNA - DNA matches
* Click on `Export shared DNA segment info for all DNA matches`

To export your segment data (gedmatch.com)
* Sign in to gedmatch.com
* Select `Analyse your data` and `'One-to-many' matches`
* Choose a kit and click on `Display Results`
* Select some kits by clicking the checkbox in the `Select` column
* Click the `Submit` button
* Click the `List/CSV` tab
* Click the `Segment CSV file` button

## TODO
* Sort by cM
* Make it pretty
* Fix performance problem with Compact view and cM<5
* Improve screen resize
* Improve mobile usability

## Screenshot

![Chromosome 1 Compact View](screenshot.png?raw=true "Chromosome 1 Compact View")
