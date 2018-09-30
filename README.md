# Assignment-3.1
assignments for Acadgild Data Science with R course

1. How to Import SAS XPORT files into R with the foreign package?
answer:
          read.xport(*filename*)
          example:
            read.xport("example.xpt")
            #end
2. How to Import SAS Files into R with the Haven package? 
answer:
        read_sas(data_file, catalog_file = NULL, encoding = NULL,
         catalog_encoding = encoding, cols_only = NULL)
  example:
        path <- system.file("examples", "iris.sas7bdat", package = "haven")
        read_sas(path)
3. How to read Weka Attribute-Relation File Format (ARFF) files in R?
answer: 
      readARFF(path, data.reader = "readr", tmp.file = tempfile(),
      convert.to.logicals = TRUE, show.info = TRUE, ...)
  example:
      path = tempfile()
      d = readARFF(path)
     
4.How to read a heavy csv/tsv file using readr package?
answer:
   install and load the package "tidyverse" or only "readr"
    read_csv() : is used for comma seperated files
        read_csv(file, col_names = TRUE, col_types = NULL,
        locale = default_locale(), na = c("", "NA"), quoted_na = TRUE,
        quote = "\"", comment = "", trim_ws = TRUE, skip = 0, n_max = Inf,
        guess_max = min(1000, n_max), progress = show_progress())
          
   read_csv2(file, col_names = TRUE, col_types = NULL,
        locale = default_locale(), na = c("", "NA"), quoted_na = TRUE,
        quote = "\"", comment = "", trim_ws = TRUE, skip = 0, n_max = Inf,
        guess_max = min(1000, n_max), progress = show_progress())   
        
   read_tsv() : is used for tab seperated files
       read_tsv(file, col_names = TRUE, col_types = NULL,
       locale = default_locale(), na = c("", "NA"), quoted_na = TRUE,
       quote = "\"", comment = "", trim_ws = TRUE, skip = 0, n_max = Inf,
       guess_max = min(1000, n_max), progress = show_progress())

      
      
