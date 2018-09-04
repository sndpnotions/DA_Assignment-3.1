# DA_Assignment-3.1
Q1: How to Import SAS XPORT files into R with the foreign package?
The foreign package with the read.xport() function also allows you to get your SAS XPORT files into R:
  >library(foreign)
  >data<- read.xport(“Path to your SAS File”)

Q2: How to Import SAS Files into R with the Haven package?

Just like foreign package the haven package also allows you to export b7dat files into R using read_sas() function.
>library(haven)
>read_sas(“Path to your File”)

Q3: How to read Weka Attribute-Relation File Format (ARFF) files in R?
Data from Weka Attribute-Relation File Format (ARFF) can be read in with the read.arff() function.
>library(foreign)
data<- read.arff(“Path to your File”)

Q4: How to read a heavy csv/tsv file using readr package?

One of the faster packages that you may use to import your big data set into R could be the readr package, which allows you to read tabular text data, just like read.table. Nevertheless, the readr package offers “a number of replacement functions that provide additional functionality and are much faster”
>df<- read_table(“path to your file”,col_names=TRUE)
the readr package also offers the functions read_csv(), read_csv2(), read_delim(), read_fwf(), read_tsv() and many other functions that go faster than their original ones.
