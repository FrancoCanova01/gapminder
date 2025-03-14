# Gapminder
Factfulness by Hans Rosling greatly challenged the world view I had at the time. After finishing the book, I became interested in the online resources they published together with the book. The purpose of this repository is to play around with the various kinds of data they offer, from building visualizations to trying out various ML algorithms.

![Factfulness](https://www.alethya.com/wp-content/uploads/2019/04/factful.jpg)

I highly recommend anyone interested in general world statistics to test their knowledge by taking [this quiz](https://upgrader.gapminder.org/t/2017-gapminder-test?tab=q) which is the Gapminder 2017 Test. The test consists of 12 questions. The surprising thing is that most people get these questions wrong, with 80% of respondents scoring below random guessing!
## How to navigate the repository

| File | Description |
| -------| ------------| 
| GapminderTest2017 | Take the Gapminder 2017 Quiz and view the results 12000 people got accross 14 different countries. |

Source: [Gapminder](https://www.gapminder.org/)

## Setup
To run locally, a docker image is provided. To build the image run from root of the project: ```docker build . -t gapminder-image``` later to run the container and link it to your local drive: ```docker run -it --name gapminder-container -v "%cd%:/usr/src/app/" gapminder-image```. Any changes to files inside the container will be reflected in your local PC directory.
