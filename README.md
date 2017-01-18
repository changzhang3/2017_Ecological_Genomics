
## Welcome to the 2017 Ecological Genomics course! 


<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.  

### Things you'll need to download:
1. [R](https://www.r-project.org/) and [Rstudio](https://www.rstudio.com/) (be sure to install and load the "knitr"" package)
2. Create a [github](https://github.com/) account and download github [desktop](https://desktop.github.com/)

Access to my whole project can be found on my [github](https://github.com/adnguyen/2017_Ecological_Genomics).

It includes this readme file, which I turned into a website you see here, but it also logs research activities on [my online notebook](https://github.com/adnguyen/2017_Ecological_Genomics/blob/master/Online_notebook.md).

### Common code you'll need to word process in (R)markdown  

1. To embed a link, all you need is the URL, implemented in the following way:   
```
[hyperlinked words](URL)
```

2. To embed an image, you'll need a URL of the image, implemented similarly as above:
```
![](URL)
```
To get a URL in (R)markdown:
    * go to your github repository and click **"Issues"**    
    * Click **"New"**    
    * Include a title (Pictures); click and drag any image you'd like into the comment section
    * Click **"Submit New Issue"** 
    * You will see the image, right click it and copy the URL.     

3. To include a table, it is best if you format it first as a csv(comma separated values). (Note, if on a mac, make sure the file type is unicode and unix). With the knitr package, you can generate tables easily from the csv. Here is an example: 

Grab a dataset real fast
```{r}
#packages for reading in data
library(data.table)

#grab dataset online
dat<-fread("https://raw.githubusercontent.com/adnguyen/HelmsCahan_CBP-partA_2016/master/Script_Analyses/Sampling_sites_table.csv")

#making a table
knitr::kable(dat)
```
|  n|Locale                    |State |Site ID | Longitude| Latitude| Tmax|
|--:|:-------------------------|:-----|:-------|---------:|--------:|----:|
|  1|Notchview                 |MA    |NO      | -73.01277| 42.49833| 24.8|
|  2|Smokey Mountains          |TN    |GP      | -83.49340| 35.63650| 25.0|
|  3|Molly Bog                 |VT    |MB      | -72.64000| 44.50000| 25.3|
|  4|Kennebec Highlands        |ME    |KH      | -69.92110| 44.56755| 25.9|
|  5|Blue Ridge Parkway        |NC    |BP      | -81.95380| 35.92640| 26.0|
|  6|Bradley                   |ME    |BR      | -68.51740| 44.98180| 26.0|
|  7|Delaware State Forest     |PA    |DF      | -75.01010| 41.30233| 26.0|
|  8|Harvard Forest            |MA    |HF      | -72.18980| 42.53130| 26.4|
|  9|Merriman State Forest     |NH    |MM      | -71.13913| 44.11107| 26.5|
| 10|Sebago Lake               |ME    |SE      | -70.58310| 43.92370| 26.6|
| 11|Hickory State Park        |PA    |HP      | -75.71751| 41.02210| 26.8|
| 12|Rugar Woods               |NY    |RW      | -73.48550| 44.49060| 26.8|
| 13|Bear Brook State Park     |NH    |BE      | -71.34803| 43.09943| 27.1|
| 14|Blackrock Mountains       |NY    |BM      | -74.02140| 41.40405| 27.1|
| 15|East Woods                |VT    |EW      | -73.19690| 44.43970| 27.2|
| 16|Albany Pine Bush          |NY    |AP      | -73.85635| 42.71930| 28.3|
| 17|Bard College              |NY    |BA      | -73.91630| 42.01740| 28.8|
| 18|Nockamixon State Park     |PA    |NK      | -75.25890| 40.43940| 29.1|
| 19|William Penn State Forest |PA    |WP      | -76.07883| 39.72570| 29.3|
| 20|Blackwater Creek Park     |VA    |LA      | -79.18100| 37.42110| 30.7|
| 21|Ljiam Nature Center       |      |IJ      | -83.86400| 35.95570| 30.8|
| 22|Knoxville                 |TN    |DW      | -83.94955| 35.91995| 30.9|
| 23|Durham                    |NC    |RC      | -79.07720| 36.03640| 31.4|
| 24|Uwharrie National Forest  |NC    |UN      | -79.97450| 35.36930| 31.7|
| 25|Hitchcock Woods           |GA    |HW      | -81.73115| 33.55605| 33.1|



  
## Assignments   
1st assignment: [Creating maps in R](RasterPCA_demo.Rmd)


## Final Project    

Below are the set of scripts for my final project.


## Displaying the organizational structure of your project (repository)

1. In the terminal, [install the tree command](https://rschu.me/list-a-directory-with-tree-command-on-mac-os-x-3b2d4c4a4827#.wk0u34bpj)
	* You may have to install the [homebrew](http://brew.sh/)    
2. use the tree command in the terminal

```
2017_Ecological_Genomics andrewnguyen$ tree
.
├── 2017_Ecological_Genomics.Rproj
├── Online_notebook.md
├── README.md
├── RasterPCA_demo.Rmd
├── RasterPCA_demo.html
├── index.Rmd
├── index.html
└── index.pdf

0 directories, 8 files
```
