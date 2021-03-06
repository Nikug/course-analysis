# Palaute
> Plot, Analyze, Learn And Understand Topic Emotions

**Palaute** is an R Shiny application for analyzing text data. Text analysis is performed using
structural topic model (STM) algorithm in combination with emotion and sentiment analysis.

Palaute is deployed [here](http://86.50.253.215/)

Palaute was created as a part of my master's thesis. The thesis can be found [here](http://urn.fi/URN:NBN:fi-fe2020052238644)

## Installation
Palaute requires some packages to run and the packages require all of their dependencies. The used packages are listed below:
```
shiny
shinythemes
dplyr
stm
tm
syuzhet
ggplot2
proxy
wesanderson
Rtsne
corpus
scales
readr
SnowballC
```

After installing the above packages, you should be able to run the application from the R-studio. Open the file `app.R` in R-studio and select `Run App`.

## Docker
Docker image of the server can be downloaded with
```
docker pull nikugronberg/palaute:latest
```
and ran with:
```
docker run --rm -p 80:3838 palaute
```
