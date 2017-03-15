
# Installing the R kernel (IRkernel) for Jupyter notebooks in Ubuntu

If you're installing in Windows or Mac, it should be pretty easy.  First, make sure R is installed, then enter the R shell by typing

`R`

in a terminal.  In Windows, you will want to press the windows key (or click the start button), type 'cmd', then right-click and run as administrator.  Then type `C:\Program Files\R\R-3.3.2\bin\R.exe` and press enter -- you may need to adjust the filepath for your version of R if it's not 3.3.2 (hint hint -- tab completion), then follow the steps [here](https://irkernel.github.io/installation/#binary-panel):

```R
install.packages(c('repr', 'IRdisplay', 'evaluate', 'crayon', 'pbdZMQ', 'devtools', 'uuid', 'digest'))
devtools::install_github('IRkernel/IRkernel')
IRkernel::installspec(user = FALSE)
```

If you're in Linux (Ubuntu for me) first, we need to install R in Ubuntu:

`sudo apt-get install r-base-core -y`

Then we need some things before we can install devtools:

`sudo apt-get install libcurl4-openssl-dev libxml2-dev libssl-dev install libcurl4-gnutls-dev -y`

Then we can do the same steps as before, after doing `sudo R` in the terminal:

```R
install.packages(c('repr', 'IRdisplay', 'evaluate', 'crayon', 'pbdZMQ', 'devtools', 'uuid', 'digest'))
devtools::install_github('IRkernel/IRkernel')
IRkernel::installspec(user = FALSE)
```
