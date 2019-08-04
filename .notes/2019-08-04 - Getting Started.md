# Goal - R in Jupyter notebook

## Useful Links

1. https://www.datacamp.com/community/blog/jupyter-notebook-r
1. https://www.datacamp.com/community/tutorials/tutorial-jupyter-notebook
1. https://minimaxir.com/2015/11/nyc-ggplot2-howto/
1. https://github.com/minimaxir/nyc-taxi-notebook/blob/master/Rstart.R

# No R, no nothin

### Python Version?

```
$ python --version
Python 2.7.10
```

End of life is Jan 2020, so let's update

```
$ brew update
$ brew upgrade python
```

### Install Jupyter

```
$ pip3 install -r requirements.txt
$ jupyter --version
jupyter core     : 4.5.0
jupyter-notebook : 6.0.0
qtconsole        : 4.5.2
ipython          : 7.7.0
ipykernel        : 5.1.1
jupyter client   : 5.3.1
jupyter lab      : not installed
nbconvert        : 5.5.0
ipywidgets       : 7.5.1
nbformat         : 4.4.0
traitlets        : 4.3.2
```

### Install R

```
$ brew install R
$ R --version
R version 3.6.1 (2019-07-05) -- "Action of the Toes"
Copyright (C) 2019 The R Foundation for Statistical Computing
Platform: x86_64-apple-darwin18.6.0 (64-bit)
```

### Install R Kernel

This is so that R can be run inside a Jupyter notebook

```
$ R

> install.packages(c('repr', 'IRdisplay', 'evaluate', 'crayon', 'pbdZMQ', 'devtools', 'uuid', 'digest'))

...(hundreds of build lines)

> devtools::install_github('IRkernel/IRkernel')
> IRkernel::installspec(user = FALSE)
> q()
```

### Verify R is in the notebook

###### Terminal 1

```
$ jupyter notebook
```

###### http://localhost:8888/tree

"R" is available as a New Notebook
