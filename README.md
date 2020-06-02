This repository contains annotations for our mixed typeface OCR training corpus
built by randomly sampling over 1000 pages from the Berliner Börsen-Zeitung. An effort
was made to balance the amount of pages containing Fraktur or Antiqua respectively.

To view/edit annotations you need the following artefacts:

1. images of full pages
2. segmentation analysis for each page
3. contour analysis for each page
4. line segmentation for each page
5. annotations for selected lines (`annotations.db`)

2., 3. and 4. were generated with the origami OCR toolset. For 1. to 4. we provide
two separate versions:

* mini (1 GB): intended for viewing text annotations and for trying things out
* full (6,8 GB): intended for editing annotations and exporting training data

In order to view or edit annotations, download one of the above, put `annotate.db`
inside the downloaded images folder, then run:

```
python -m origami.tool.annotate /path/to/this/repo
```
