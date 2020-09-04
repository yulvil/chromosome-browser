# chromosome-browser

**Goals**:
* A chromosome browser to easily find overlapping DNA segments between your matches
* Visualize segment data from multiple sources at the same time: gedmatch, familytreedna, myheritage, 23andme or your handcrafted csv file.

**Try it**: https://yulvil.github.io/chromosome-browser.html

Features
* Copy/paste your CSV data (gedmatch, familytreedna, myheritage, 23andme)
* Drag and drop CSV files from your desktop
* No limits on the number of segments
* All the rendering is done on the client side. No data sent to servers.
* No tracking. No Google Analytics.
* Filter by centimorgan (cM)
* Include or exclude kits (persons)
* Different views (compact, by kit, ordered by segment)
* You can save the webpage to your desktop and use the Chromosome Browser without Internet connection.

### CSV data formats

Formats supported are

familytreedna.com segments file format
```
NAME,MATCHNAME,CHROMOSOME,START LOCATION,END LOCATION,CENTIMORGANS,MATCHING SNPS
or
Name,Match Name,Chromosome,Start Location,End Location,Centimorgans,Matching SNPs
```

myheritage.com segments file format
```
Name,"Match name",Chromosome,"Start Location","End Location","Start RSID","End RSID",Centimorgans,SNPs
```

gedmatch.com segments file format
```
"kit1","name1","email1","kit2","name2","email2","chr","start","end","cm"
```

23andme segments file format
```
"Display Name","Surname","Chromosome Number","Chromosome Start Point","Chromosome End Point","Genetic Distance","# SNPs","Full IBD","Link to Compare View","Sex","Birth Year","Set Relationship","Predicted Relationship","Relative Range","Percent DNA Shared","# Segments Shared","Maternal Side","Paternal Side","Maternal Haplogroup","Paternal Haplogroup","Birthplace","Residence","Family Surnames","Family Locations","Maternal Grandmother Birth Country","Maternal Grandfather Birth Country","Paternal Grandmother Birth Country","Paternal Grandfather Birth Country","Self Reported Ashkenazi Jewish Descent","Notes","Sharing Status"
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

To export your segment data (23andme)
* Sign in to 23andme.com
* Click on `DNA relatives`
* Click on `Download aggregate data`

## TODO
* Sort by cM
* Make it pretty
* Fix performance problem with Compact view and cM<5
* Improve screen resize
* Improve mobile usability

## Screenshot

![Chromosome 1 Compact View](screenshot.png?raw=true "Chromosome 1 Compact View")
