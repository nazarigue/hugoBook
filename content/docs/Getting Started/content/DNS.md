---
title: 'Domain Name System'
draft: false
weight: 2
bookComments: true
---
## DNS

What is the Domain Name System?

Let's think a bit. You have a computer in front of you. You want to open a special program called browser and get content from some pages you know. 

We have

- computer
- internet
- browser
- website

A computer is the hardware, connected to the internet, accessible through browser to get to the website, that is reachable with a specific address.

In order to reach the destination, it should be live somewhere. Like your computer, if it's off, nobody can reach it. Logically derived, there should be some machine making the website available all the time, in order for you to reach it wherever you need it.

How does it work.

This is what you get visualised when you search for explaining this.

![https://miro.medium.com/max/2908/1*mOLfDYXBnFm8ggrHWeyXtA.jpeg](https://miro.medium.com/max/2908/1*mOLfDYXBnFm8ggrHWeyXtA.jpeg)

It does not help to explain the basics.

Let's define it in a simple manner.

We said you have:

- computer
- internet
- browser
- website

So, when you want to reach another website, you go and type into the browser, whats called URL. **Uniform Resource Locator. Address basically.**

That means, somewhere, let's repeat, is a live website, that is waiting for you to come. You type(URL): www.google.com

Your computer is sending the request, to some other live computer, and saying: "Hey, if you are www.google.com, share with me what should be on this address"

What you should get as a response, if your request is correct, is the website: [www.google.com](http://www.google.com) that looks like this.

![https://9to5google.com/wp-content/uploads/sites/4/2019/03/google-search-material-theme-cover.jpg?quality=82&strip=all&w=1600](https://9to5google.com/wp-content/uploads/sites/4/2019/03/google-search-material-theme-cover.jpg?quality=82&strip=all&w=1600)

That's not  yet! What is **Domain Name System?**

Look, we are humans. We need names. We recognise stuff by giving them names. You remember, what was doing the first human on earth? Naming stuff. 

Machines, are computing stuff, so they are more into numbers. On deeper level they operate with ZERO's and ONE's. In DNS case, what is actually happening, is Domain Name Serves, to humans is showed in words, but machines read them in numbers. What? 

They don't need words and they don't give damn a about them. Each address is actually a number. 

Domain Name System is actually:

# 93.184.216.34

That's all you need to know now. It's actually a number. There are several types of them but you don't need to know that more, it's useless.

> Outcome. Domain Name System, is human readable request to reach a destination, which is URL (website) but in reality it is a set of numbers, that by typing you will reach the same place.

What do we learn from here?

There are 2 types of information out there. **Human readable** and **machine-readable.** Many people do not know that and think computers don't compute but smoke cigars and think about meaning of life.

This is what it actually is. Now forget it.

![https://upload.wikimedia.org/wikipedia/commons/thumb/7/74/Ipv4_address.svg/2880px-Ipv4_address.svg.png](https://upload.wikimedia.org/wikipedia/commons/thumb/7/74/Ipv4_address.svg/2880px-Ipv4_address.svg.png)

## OK, I got it. But what is: **www.?**

It's called subdomain. It's just a part of root domain. It can be whatever you want. It's helping to categorise stuff.

- go.now.com
- next.now.com
- be.now.com
- present.now.com

 You name it!

## Right. But what is .com?

It's called Top Level Domain. It can be:

- co.uk
- .fr
- .de
- .whatever

**There are many of them, you can check it out. BUT NOT NOW.**

**Server**

![https://www.evernex.com/wp-content/uploads/2016/10/Untitled-1-1.jpg](https://www.evernex.com/wp-content/uploads/2016/10/Untitled-1-1.jpg)

> On this level, we just know that server is an online, always working, machine, that is storing files. Since you cannot share stuff from your laptop all the time, you need something to be online without you.

## Servers are used to store information and allow other computers to get it.

When you type www.google.com, server will respond to you with an answer. Server responds with HTTP statuses, successfully with status **200**. Keep in mind, number 200.

That's it for now.

**Website Structure**

So, we have:

- computer
- internet
- browser
- URL with domain in it
- server

What happens when we go to [wikipedia.com](http://wikipedia.com). Server says, right, i have it, i'll send you stuff for wikipedia.com, i'll show it in your browser.

![https://www.legalmorning.com/wp-content/uploads/2013/03/English-Wikipedia-Translation-Service-1024x601.png](https://www.legalmorning.com/wp-content/uploads/2013/03/English-Wikipedia-Translation-Service-1024x601.png)

And here you go. It's a page with some layout and content.

# Wait, but how did that work?

Guess: Someone created all this content, put on a server, and allows you to have an access.

> These are actual files, on a server. You can check that by pressing F12 on your keyboard and click sources tab. You see some stuff there right?

![https://developers.google.com/web/tools/chrome-devtools/images/sources-page-pane.png](https://developers.google.com/web/tools/chrome-devtools/images/sources-page-pane.png)

## Are you lost?

Again

What are you doing? Asking to show the website you want to go to. URL is a way to reach files on a server. Server is giving files to the browser. And by doing magic, you get this nice website. It's actually a set of files, interpreted by browser.

**What's inside the files?**

We will start with simple explanation of the set, that is simple to understand. 

You see content. Content consists of text and text consists of words