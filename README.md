# Football Web Scraping Project

## Introduction

This project was created as training on how to scrape webpages and analyze football datasets. I scraped data from [FBref](https://fbref.com/en/) on the statistics of Manchester City and Spain player Rodrigo Hernández Cascante "Rodri" to compare two seasons of his career (2022/2023 and 2023/2024), trying to confirm my idea of him playing better in his Ballon d'Or winning season than the treble winning season.

## The Dataset

The data was collected by scraping the **FBref** website.

**About FBref**

> A website dedicated to tracking statistics for football teams and players from around the world.
> Created by Sports Reference, the team behind popular stats websites like Baseball-Reference and Basketball-Reference.
> They also cover American football, hockey, and college sports.

The data was scraped with ease using only one line of code.
using only pandas function read_html

```
df = pd.read_html('https://fbref.com/en/players/6434f10d/all_comps/Rodri-Stats---All-Competitions',
                  attrs={"id":"stats_standard_collapsed"})[0]
```

## Cleaning the data

the data was cleaned to in the desired shape for analysis, multiple steps were taken:
* removing the multi level column names
* droping unwanted columns
* renaming the columns
* converting the data types
* subseting the required seasons


## Analyzing the data

graphs were made to compare the most important stats

![download](https://github.com/user-attachments/assets/24892758-548c-4bf3-b04e-96d3afb36071)
 
