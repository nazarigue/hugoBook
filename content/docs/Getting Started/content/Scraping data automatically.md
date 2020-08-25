---
title: 'Automated Data Scraping '
bookFlatSection: true
date: 2019-02-11T19:27:37+10:00
draft: false
weight: 4
---

There are multiple ways how you can automate data scraping.

1. Use Google Sheets
2. Use services that can have simple GUI
3. Code yourself a scraper

## 1. Scraping data in Google Sheets

There are 3 formulas to scrape online data by default that you can use with Google Sheets.
1. `=importxml` - to get any data from web via having URL and XPath
2. `=importfeed` - to get structured ATOM or RSS feed
3. `=importhtml` - retrieve only list or table element from URL

### We will start from the most simple one, `importfeed`


Take any news portal and find if they have any RSS feed available.


Usually the easiest way is to find it from inspect console.

![](/2020-08-14-14-39-05.png)

We take any of the URL-s and add it to SHEETS formula.

`=IMPORTFEED("https://feeds2.feedburner.com/delfiuudised","items summary",false,100)`

- First we provide url
- Second, elements we want to have
- Third, headers if we want to include `true` or `false` 
- Fourth, amount of feed items

You can check documentation on specific query details [here](https://support.google.com/docs/answer/3093337?hl=en-419).

Another example:

`blog.google` 

Look for RSS feed

![](/2020-08-14-16-25-38.png)

Here is how the URL looks like and the content in it

![](/2020-08-14-16-25-54.png)

With query `=IMPORTFEED("https://blog.google/rss","items",true,100)` we get these results:

![](/2020-08-14-16-30-48.png)

Summaries are really long, so we want to have only titles and URL-s

For title cell `=IMPORTFEED("https://blog.google/rss","items title",true,100)`

For url cell `=IMPORTFEED("https://blog.google/rss","items url",true,100)`

![](/2020-08-14-16-33-14.png)

Looks much better!

___

## 2. Next we will use `importhtml`

`importhtml`

So, `importhml` pulls lists and tables from the page.

First use the formula

`=IMPORTHTML("https://en.wikipedia.org/wiki/List_of_countries_by_GDP_(nominal)","table",8)`

So, the structure is as follows:

1. Url where the table is
2. choose "table" or "list" element
3. the index of the element, in our case is the 8th table on the page, since there are many of them
  
![](/2020-08-14-17-02-11.png)

and we are getting the table content to our table.

___

## 3. The hardest part: `importxml`
Here is what we will do:

Take a website and pull out data to Google sheets via `=IMPORTXML()` function. [Formula documentation we can find here](https://support.google.com/docs/answer/3093342?hl=en "IMPORTXML Google Sheets").

##

[Here we have a data](https://learnui.design/blog/100-things-ux-ui-designer-know.html "100 things designer should know"), where we have a list of elements and inside that list there is a hidden element that is opening up with expanding it.

Here's the XPath that will will use: `=IMPORTXML("https://learnui.design/blog/100-things-ux-ui-designer-know.html","//ol[@class='hundred-things']/li")`


[Sheets file XPath](https://docs.google.com/spreadsheets/d/1fy2en_Ql-8kMj5e_suqOEuehTAPo55lwBp3gFY2Sr9M/edit?usp=sharing "XPath Sheets Link" )