# Scout

**Description**:

This repo is used as a starting point for experimenting with R inside of Jupyter notebooks

## Installation

These steps are for Mac installation.  (R steps from [here](https://www.datacamp.com/community/blog/jupyter-notebook-r))

```
$ <clone this repo to a local path>
$ brew install python R
$ pip3 install -r requirements.txt
$ R

> install.packages(c('repr', 'IRdisplay', 'evaluate', 'crayon', 'pbdZMQ', 'devtools', 'uuid', 'digest'))

...(hundreds of build lines)

> devtools::install_github('IRkernel/IRkernel')
> IRkernel::installspec(user = FALSE)
> q()
```

#### Verify installation

##### Terminal 1

```
$ jupyter notebook
```

##### Browser - http://localhost:8888/tree

1. Click on `iris-cart.ipynb`
1. The notebook should be able to run
