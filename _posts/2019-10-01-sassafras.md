---
title: I coded a thing, if you use GoogleScholar you might find it useful too
date: 2019-10-01
permalink: /posts/2019/10/sassafras
tags: 
  - academiclife 
  - GScholar 
  - javascript
---
I have always had trouble navigating the huge amount of new papers, pre-prints, and tweets that come out every day. I always felt like I was the last one to know about other people’s research until I went to a conference or stumbled upon it during the literature research for a new paper. I still haven’t figured out Twitter, but I did figure out how to have a list of new papers and pre-prints as they come out. It might not be the smartest way, but last year I coded a small script to compactify all the Google Scholar alerts I subscribe to.

**How does Google Scholar Alerts work?**  
Google Scholar is a freely accessible web search engine that indexes the full text or metadata of scholarly literature across an array of publishing formats and disciplines 
[[Wikipedia](https://en.wikipedia.org/wiki/Google_Scholar)]. Every researcher can have their own page with their verified indexed research in the systems and suggestions of new research in their areas. I find it very useful when doing some literature review for new projects, or discovering other peoples’ research. It is possible to sign-up for weekly email alerting you of new papers indexed in the systems that are relevant to your research, somebody else’s research, new papers by your favorite scientists or related to certain keywords. Even though Google Alerts can be very useful, receiving *10 emails a week* about the same paper can be quite annoying, so I decided to do something about it.


**What does Sassafras do?**  
The script searches for unread Google Scholar Alert emails and parses the text extracting the titles, authors, and links of the new indexed papers in all the alerts into a single SpreadSheet in Google Drive.  

There are optional functions for sending a summary email with the most common papers and pre-prints across all the alerts that have been parsed. A script that adds a custom drop-down menu to your SpreadSheet in Google Drive with the sassafras functions. A function for organizing the papers into different Sheets according to custom keywords fund in the title, or adding the keywords in a column for better sorting.  

It is not perfect, but it has helped me keep up with some of the new research out there and maybe it can help you too.  

You can find the code on my Git [Sassafras Repo](https://github.com/alpatania/sassafras), together with some instructions on how to set it up and run the script automatically every week.
