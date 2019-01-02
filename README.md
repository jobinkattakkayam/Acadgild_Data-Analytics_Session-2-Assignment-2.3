# Acadgild_Data-Analytics_Session-2-Assignment-2.3
SESSION 2 - INTRODUCTION TO R - Assignments 2.3

	Problem Statement
  
1.	How to Import SAS XPORT Files into R With The foreign package

2.	How To Import SAS Files into R With The haven Package?

3.	How to read Weka Attribute-Relation File Format (ARFF) files in R?

4.	How to read a heavy csv/tsv file using readr package?
 
 ANSWERS : 
 
# Acadgild-Dataanalytics-session3-Assignment1
DATA ANALYTICS WITH R, EXCEL AND TABLEAU SESSION 2 ASSIGNMENT 2.3      

1. 

library(foreign)

read.xport (foreign)

read.xport(file) 


2. 

install.packages("haven")

library(haven)

dat= read_sas("path to file", "path to formats catalog")

Eg: path <- system.file("examples", "iris.sas7bdat", package = "haven")

read_sas(path)

 
3.

Library(foreign)

read.arff(file)

Eg: read.arff(system.file("arff", "contact-lenses.arff",
 package = "RWeka"))
 
 
 
4.
# Read a txt file, named "mtcars.txt"

my_data <- read_tsv("mtcars.txt")

# Read a csv file, named "mtcars.csv"

 my_data <- read_csv("mtcars.csv")
