# www.giscience.net

## Welcome!

Here you will find data about conferences and journals in the field of geographical information science (GIScience).  The data are used to generate [www.giscience.net](http://www.giscience.net).

Please feel welcome to contribute to the website by adding more conferences and journals.  For doing so, you create a merge request, and the data will appear soon on the website.

The data are licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License](https://github.com/giscience/geogrid/blob/master/LICENSE).  Please feel free to reuse them.  The contributors would be happy if you would not forget to give the appropriate credit.

## How to contribute?

The files are formatted in YAML, a language that is designed to be human readable and easy to understand.  In the following, you will find some information about the internal format of these files.  If you have any questions, please do not hesitate to contact [Franz-Benjamin Mocnik](http://www.mocnik-science.net).

### Conferences

A typical conference looks like follows:

```YAML
COSIT 2017:
  count: 13th
  start: 2015-09-04
  end: 2015-09-08
  place: L'Aquila, Italy
  url: http://www.cosit2017.org
  proceedings: http://drops.dagstuhl.de/opus/volltexte/lipics-complete/lipics-vol86-cosit2017-complete.pdf
  proceedings2: http://doi.org/10.1007/978-3-319-63946-8
```

If you do not know the exact `start` and `end` date, please only note the year in the corresponding fields.

The field `proceedings` refers to the main proceedings of the conference (e.g., long papers), while `proceedings2` refers to additional proceedings (e.g., short papers and posters).  If a doi is available, please use `http://doi.org/...` as a url.

Please add only conferences series that comply to the following rules:

* Only conference series, no single or one-time conferences.
* The conference is strongly related to and broadly accepted in the field of GIScience.
* The conference has an international character.  This excludes conferences that are of purely local character.
* Workshops are not counted as a conferences.

### Journals

A typical journal looks like follows:

```YAML
GSIS:
  name: Geo-spatial Information Science
  abbreviation: GSIS
  url: http://www.tandfonline.com/toc/tgsi20/current
  publisher: Taylor & Francis
  open access: false
```

The first line is only an internal abbreviation.  If an official/widely-used abbreviation exists, it is used in the first line, and the first characters of the journal name otherwise (including capitals and lower case letters).

Please **order** the journals by the internal abbreviation (first line)!

The `abbreviation` shall only be provided if an official or a widely-used abbreviation exists.  The `url` of the journal is essential.  For Taylor & Francis journals, please provide a link of the form `http://www.tandfonline.com/toc/***/current`.  The `publisher` needs to be provided in short form.

If a journal does not provide open access by default, it shall be marked as `open access: false`.  Only purely open access journals shall be marked as `open access: true`.

Please add only journals that comply to the following rules:

* The journal is strongly related to and broadly accepted in the field of GIScience.  This is the case for all journals that have GIS or GIScience in their name or in their description.
* The journal has an international character.  This excludes journals that are of purely local character.

## License

The data are licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License](https://github.com/giscience/geogrid/blob/master/LICENSE).  Please feel free to reuse them.  The contributors would be happy if you would not forget to give the appropriate credit.
