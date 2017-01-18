
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




  
## Assignments   
1st assignment: [Creating maps in R](RasterPCA_demo.html)


## Final Project    

Below are the set of scripts for my final project.


## Organizing your project (repository)

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
