# Overview

This repository contains a script that visually formats simple tables in Asciidoc files into a more readable format.

The script allows you to render tables of the following type:

```adoc
|===
|Header 1        |Header 2        |Header 3

|Column 1, row 1                                                |Column 2, row 1 |Column 3, row 1

|Column 1, row 2|Column 2, row 2 |Column 3, row 2

|Column 1, row 3  |Column 2, row 3 |Column 3, row 3
|===
```

Into a more visualized view:

```adoc
|===
| Header 1        | Header 2        | Header 3       
| Column 1, row 1 | Column 2, row 1 | Column 3, row 1
| Column 1, row 2 | Column 2, row 2 | Column 3, row 2
| Column 1, row 3 | Column 2, row 3 | Column 3, row 3
|===
```

As a result, the script will create a file **output.adoc**, which will be a copy of the selected file, but with formatted tables.

> **Note**
> The contents in the **output.adoc** file are always overwritten after the script is run!

## Dependency|Requirement

* python 3.x

## Installation

```
sudo make install
```

After that, the tool will be available in console with command `asciidoc-table-beautifier`.


## How to use

Just run the script with the following command:

`python script.py`

At that, the console will display help. Or you can specify as an argument the file in which you want to format the tables:

`python script.py input.adoc`

## What's new

* [feature--1.0.a](https://github.com/Andronovss/asciidocTablePrettify/tree/feature--1.0.a) -- Added a check for the number of "|" symbols.
If the number is not true, then -- false.


## ToDo


- [x] Make `./script.py` standalone run
- [ ] Adding support of argparse
- [ ] Adding support of advanced table formatting 1/4: supports custom options in table meta-info like: `[cols="4s,30", frame=none, prettify=no]` (ability to skip certain tables with prettify/donttouch attribute)
- [ ] Adding support of advanced table formatting 2/4: supports tables with merging rows and/or columns
- [ ] Adding support of advanced table formatting 3/4: supports tables in manner "single cell per string"
- [ ] Adding support of advanced table formatting 4/4: ???





