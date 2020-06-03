This repository contains annotations for our mixed typeface/mixed context (body text and table text) OCR training corpus
built by randomly sampling over 1000 pages from the <a href="http://zefys.staatsbibliothek-berlin.de/list/title/zdb/2436020X/">Berliner Börsen-Zeitung</a>. An effort was made to balance the amount of pages containing Fraktur or Antiqua respectively as well as the amount of lines drawn from each year.

To view/edit annotations you need the following artefacts:

1. images of full pages
2. line segmentation for each page
3. annotations for selected lines (`annotations.db`)

2. was generated with the origami OCR toolset. To obtain 1. and 2., use one of these two:

A. <a href="https://www.dropbox.com/sh/vqb0ky4gtdjuuws/AADnKPzQwvsklfNn38HDWZ93a?dl=0">Mini Version (1 GB).</a> Intended for viewing text annotations and for trying things out.
B. <a href="https://www.dropbox.com/sh/mgsopnami242i8u/AAByAKVmdMACiQK72jhLLQ2Ka?dl=0">Full Version (6,8 GB).</a>. Intended for editing annotations and exporting training data.

Now unzip `annotate.db.zip` from this repository, put `annotate.db` inside the A./B. folder, then run:

```
python -m origami.tool.annotate /path/to/images
```
