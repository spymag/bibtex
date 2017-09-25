# bibtex
A trial bibtex php browser

1.Install

Add the files in the same folder. Make sure php can write in this folder. (it writes cache so performancewise is much quicker)

2. How to call the library:

Create a bib file with the publication records (e.g. biblio.bib) and upload it to your server.
* Use the link bibtexbrowser.local.php?bib=biblio.bib (frameset based view)
* Use the link bibtexbrowser.local.php?bib=biblio.bib&all (pub list sorted by year)
* Use the link bibtexbrowser.local.php?bib=biblio.bib&all&academic (pub list sorted by publication type, then by year, see "Sectioning in academic mode" below)

Warning: bibtexbrowser maintains a cached version of the parsed bibtex, for high performance, check that PHP can write in the working directory of PHP.

Handling mutliple bibtex files: If you want to include several bibtex files, just give bibtexbrowser the files separated by semi-columns e.g:
bibtexbrowser.local.php?bib=strings.bib;biblio.bib
