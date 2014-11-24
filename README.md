Dpulex_BSGenome
===============

A Bioconductor/Biostrings Genome (BSGenome) package for the current assembly (v1.1) of Daphnia pulex

After cloning this repository, you can create (or 'forge') a BSgenome object using the following commands (see also http://www.bioconductor.org/packages/release/bioc/vignettes/BSgenome/inst/doc/BSgenomeForge.pdf):

Using R: 

> library(BSgenome)
> forgeBSgenomeDataPkg("path/to/DpTCO_seed")

Once this is complete, exit R and enter the following commands on your Unix/Linux command line: 
(this presumes this is in your working directory, otherwise enter the path to this folder and then the folder name)

> R CMD build BSgenome.Dpulex.JGI.dpulex 
(this builds the tarball object, entitled 'BSgenome.Dpulex.JGI.dpulex_1.1.tar.gz')

> R CMD check BSgenome.Dpulex.JGI.dpulex_1.1.tar.gz
(this ensures that the package will install correctly on your machine)

> R CMD INSTALL BSgenome.Dpulex.JGI.dpulex_1.1.tar.gz
(finally, this will install the package in your R library)

If you have any questions or encounter a problem with this package, please create an issue on his account or email me directory at rtraborn 'at' indiana 'dot' edu.

