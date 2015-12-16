Wikidata List Generator
=======================
Creates a list of Page titles and their corresponding Wikidata items.
## Data download
Download the json dump [Wikidata database downloads](https://www.wikidata.org/wiki/Wikidata:Database_download) and 
extract it somewhere on your file system and extract it.
The download is approx 4G (Dez 2015) compressed json data which extracts to approx 60G.
## Run
```
mvn clean install -DskipTests
mvn test
mvn exec:java -Dexec.args="--help"
```
help displays the available options to pass instead of "--help":
```
  Options:
    -a, --aliases

       Default: false
    --help

       Default: false
    -i, --input
       path to the file with the wikidata json dump
    -l, --language
       language to extract
       Default: en
    -o, --output
       path to output file
```

## See also
[Wikibase data model](https://www.mediawiki.org/wiki/Wikibase/DataModel/JSON)

[![Build Status](https://travis-ci.org/physikerwelt/WikidataListGenerator.svg?branch=travis)](https://travis-ci.org/physikerwelt/WikidataListGenerator)
[![MavenCentral](https://maven-badges.herokuapp.com/maven-central/com.formulasearchengine/wikidatalistgenerator/badge.svg)](maven-badges.herokuapp.com/maven-central/com.formulasearchengine/wikidatalistgenerator/)
[![Coverage Status](https://coveralls.io/repos/physikerwelt/WikidataListGenerator/badge.svg)](https://coveralls.io/r/physikerwelt/WikidataListGenerator)
