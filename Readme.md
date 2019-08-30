# Summer student report template

Jakob Beyer, 2019

## Installation

Simply clone this repository (clone button in top right corner in GitHub) or fork it to your own GitHub account and then clone it.

## Structure

- `LateX` contains the actual latex code
- `Plots` is where you put all the plots you want to use
- `Logos` is where logos of DESY/universities sit

## Running

Here is how you compile your `Report.tex` file in the `LateX` directory.

1. Create a common library file from the individual bibtex (.bib) files in the `ManuelBibEntries`:
  ```shell
  ./combine_bib_entries.sh
  ```
2. Compile the report using `lualatex` (needed for Feynman diagrams) and `biber`:
  ```shell
  lualatex Report.tex
  biber Report
  lualatex Report.tex
  ```
  
## Adding references

1. Create a new `.bib` file in the `LateX/ManuelBibEntries` directory.
2. Find the `bibtex` reference for the paper/book/etc. These can often be found on the website of the article (e.g. <http://bib-pubdb1.desy.de/record/166034> at bottom of page under the `BibTeX (UTF-8)` button).
3. Copy the bibtex code into the `.bib` file and save.
4. Compile as written above.
  
## Remarks

- This template isn't strict, you may modify it as you wish.
- The line numbers are thought to be temporary to ease the job of correctors. They can be disabled at the top of the `Report.tex` document.
- If you have any questions, comments or suggestions please contact me to update this template!