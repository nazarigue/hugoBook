---
title: 'HTML and XPath'
date: 2019-02-11T19:27:37+10:00
draft: false
weight: 2
---


# Understanding HTML

HTML is a markup language used to communicate content in the web.

Here are the tags what we should know.

Each paragraph has the opening tag like ```<h1>``` and closing tag ```</h1>```


|tag|Purpose|
|---|---|
|``` <h1> ```|For heading1|
|``` <h2> ```|For heading2|
|``` <h3>```|For heading3|
|``` <p> ```| For paragraphs|
|``` <title>```| For page title|
|```<ul>```| For unordered list|
|```<ol>```| For ordered list|
|```<li>```| For list element|
|```<td>```| For table data|
|```<tr>```| For table row|
|```<th>```| For table header cell|
|```<table>```| For table|


# Understanding XPATH

XPATH is the method, highly used in web scraping, to get content inside HTML tags.

Get ALL elements XPATH

|XPATH|Purpose|
|---|---|
|```//h1```|find all ```<h1>``` tags|
|```//h2```|find all ```<h2>``` tags|
|```//h3```|find all ```<h3>``` tags|
|```//ul```|find all ```<ul>``` tags|

Go deeper in path

|XPATH|Purpose|
|---|---|
|```//h1/a```|find all ```<h1>``` with ```<a>``` anchor tag|
|```//h1[@class="column"]```|find all ```<h1>``` with ```<class>``` column tag|
|```//*[@id="column"]']```|find all elements with ```<id>```equals column tag|


