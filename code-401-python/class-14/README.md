
# Web Scrape

* **Web scraping** is a technique to automatically access and extract large amounts of information from a website

![](https://res.cloudinary.com/practicaldev/image/fetch/s--KLJcR1tz--/c_imagga_scale,f_auto,fl_progressive,h_900,q_auto,w_1600/https://thepracticaldev.s3.amazonaws.com/i/mplqezmxfupbu7x7d90k.jpg)

## Important notes about web scraping

* Make sure you are not downloading data at too rapid a rate because this may break the website. You may potentially be blocked from the site as well.
* Read through the website’s Terms and Conditions to understand how you can legally use the data. Most sites prohibit you from using the data for commercial purposes.

## Inspecting the Website

* The first thing that we need to do is to figure out where we can locate the links to the files we want to download inside the multiple levels of HTML tags.
* Simply put, there is a lot of code on a website page and we want to find the relevant pieces of code that contains our data

)

# Beautiful Soup


* **Beautiful Soup** is a Python library designed for quick turnaround projects like screen-scraping. Three features make it powerful:

* Beautiful Soup provides a few simple methods and Pythonic idioms for navigating, searching, and modifying a parse tree: a toolkit for dissecting a document and extracting what you need. It doesn't take much code to write an application
* Beautiful Soup automatically converts incoming documents to Unicode and outgoing documents to UTF-8. You don't have to think about encodings, unless the document doesn't specify an encoding and Beautiful Soup can't detect one. Then you just have to specify the original encoding.
* Beautiful Soup sits on top of popular Python parsers like lxml and html5lib, allowing you to try out different parsing strategies or trade speed for flexibility.
