# Daily Scientific Citation Tracker

Covid-19 research represent one of the most intense scientific efforts in the modern history of science. In sheer volume of production in just under five months, it it the most concentrated production of scientific knowledge on a single topic in human history. Bibliometric services like Pubmed index literally hundreds of new Covid-19 articles on a daily basis. We need new tools to track the citation behavior of the covid ecosystem. All modern bibliometric record yearly citation count for scientific papers [how many times a paper is cited yearly since the year of publication]. Giving the rapid pace of Covid-19 research, what we need is a tigher level of temporal granularity. That is, we need more than the number of yearly citations, we need the number of daily citations [how many times a paper is cited daily since the date of publication].

The Daily Scientific Citation Tracker is the first bibliometric tool to record how many times an article is cited every day since the date of publication. The current beta version indicates the daily citation count at the publication-level. The current development under way will add two level of aggregation: journal and themes.

![](images/DSCT_top_6.jpg)

What can we do with this level of time-granularity? At the "keyword/theme"-level, the Daily Scientific Citation Tracker can showcase which type(s) of Covid-19 research is gainign or loosing momentum over time. Also, since the database provides the date of publication for most Covid articles, it is possible to visualize a host of patterns not just in citation, but in publication as well. Generally speaking, the tool is intended for both Covid-19 researchers in their daily navigation of a thick research literature as well as information & social scientists, and historians of science studying what shall be considered one of the most pivotal moments in the recent history of science.

# Link-Cov-P Dataset

What Covid-19 bibliometric data are you using for this project?

The Daily Scientific Citation Tracker build on another of my ongoing project. As a daily stream data project, Link Cov P dataset is a record linkage effort linking Cord-19, LitCovid, and WHO datasets on a daily basis. To build the Daily Tracker, we need two key variables: (1) the earliest date of publication and (2) a full references list of cited works. See documentation for methodology. To collect those two data-points, I query multiple APIs and harvest online full text pdfs online.

* for more on the making of [Link-Cov-P Dataset](https://github.com/lanbufan/subFIELD.lab-Covid-19-pub-database), see my other repo.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

For researchers or data scientists looking to explore the dataset, you only need to donwload:

* the latest beta version of daily tracker in CSV format.

For those interested in the "back-end" of things, or in hepling the development of this project, you will need to download:

* the latest version of the references files in CSV format.
* the latest version of the Python source code matching references-as-publications to generate the daily tracker.
* + config.py

For those interested in the "back-end" of the Link-Cov-P dataset, please see my other repo.

### Prerequisites

What things you need to install the software and how to install them

* Python 3

* Python Packages: fuzzywuzzy, json, pandas, re, os

### Installing

A step by step series of examples that tell you how to get a development env running

With Python and dependencies installed and CSV downloaded, just:

* all the full path of where the CSV is located on your local machine in the config.py file.

End with an example of getting some data out of the system or using it for a little demo

## Running the tests

Please note the current beta version of the code to generate the daily tracker is serial. The parr. of the process still needs to be implemented.
Therefore, as of today running the code to generate the daily tracker takes between 15 to 30 minutes. A little slow, I know.

## Contributing

Plese feel free to email [me](f.lachapelle@alumni.ubc.ca) if you have any questions or if you are interested in contributing.

## Authors

* Francois Lachapelle - subFIELD.lab

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

At its foundation, this project is a Record Linkage initiative. Therefore, it would not be possible without the great work of researchers at:

* Goldbloom et al., 2020 - [CORD-19](https://www.kaggle.com/allen-institute-for-ai/CORD-19-research-challenge)
* Lu, Chen, & Allot, 2020 - [LitCovid](https://www.ncbi.nlm.nih.gov/research/coronavirus/)
* Garnica-Carreno, Jose, 2020 [WHO]

For advisory support:

* John McLevey - [UWaterloo](https://github.com/mclevey)

