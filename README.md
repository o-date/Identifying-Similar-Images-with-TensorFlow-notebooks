# Identifying-Similar-Images-with-TensorFlow

You can launch this jupyter notebook in an executable environment by clicking on the button below.

[![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/o-date/Identifying-Similar-Images-with-TensorFlow-notebooks/HEAD)

[![DOI](https://zenodo.org/badge/132169566.svg)](https://zenodo.org/badge/latestdoi/132169566)

If you haven't worked with jupyter notebooks before, try the 'Getting Started' notebook first. Otherwise, go with the 'Finding Similar Images' one. Then, you can try examining the results with the 'Affinity propagation' notebook, or the 'visualizing as a network' notebook. Please note that for both of those subsequent notebooks, you _will_ have to make some adjustments to some of the resulting .json or .csv files from 'finding similar images'. Nothing serious.

'Finding similar images' is based on Douglas Duhaime's tutorial [identifying similar images with tensorflow](http://douglasduhaime.com/posts/identifying-similar-images-with-tensorflow.html) which is very clearly laid out and explained. In this notebook, I've compressed the steps. The 'images' directory only has 25 images in it for demo purposes. In Duhaime's post, the images folder (that you grab with `wget` has about 2000 images in it). If you clone this repo locally, you can easily load more images into that folder. Alternatively, you might want to clone this repo into something like [Google Colab](colab.research.google.com/) and connect it to your GDrive (where you might have a folder with hundreds of images ready to go).

Thank you to Douglas Duhaime for the original code, and to Katherine Davidson, Eric Hobson, and Iain Davidson for testing, troubleshooting, and the json-to-csv code.

Other things - 

the `requirements.txt` file should list the python bits and pieces need to be installed, so that should save us from having to `!pip` install. There is a package called `RPy2` that can be loaded this way, that then lets us do bits and bobs of R mixed in with python - see [this post](https://medium.com/@mbussonn/baf064ca1fb6).

to get the R kernel so that I can have just an R notebook we need the `runtime.txt` file. Inside that, we have a single line that says `r-2018-04-01` (where the date stamp comes from [this](https://mran.microsoft.com/timemachine)).

to preload and R packages, put the name of the package in the `install.R` file in normal R syntax, like so: `install.packages("ggplot2")`.

And there we have it! Sometimes the binder fails to launch. Just reload. Keep reloading.

