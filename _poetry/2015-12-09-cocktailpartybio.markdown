---
layout: post
title: Cocktail Party Biology
date: 2015-12-09
description: Google App Engine based website
---
<a class="poem-title" href="https://cocktailpartybio.appspot.com/"> Cocktail Party Biology Website </a>
<br>
Note: You will need to create an account for use but you do not need to use a real email address. In order to access the quizzes, you will need to watch the videos and move sequentially through the levels. The 'reset' button was included for testing.

<a class="poem-title" href="https://github.com/jvmakin/final-project-jvmakin"> Source Code </a>

# A video-based introduction to a few 'cocktail party level' topics in biology.
Written as a final project for the U of C CS Masters Bioinformatics course.
<br>

# Abstract
Cocktail Party Biology (CPB) is an online learning website created to engage non-professional users with common biological topics. This project was inspired by the gap between scientific and media reports of such subjects as well as by a perceived lack of casual-level adult learning programs. The website was implemented using Google App Engine and webapp2 for python. The result is a webpage that allows users to create accounts, view tutorials, and prove their knowledge with short quizzes. In future, CPB could be extended to include more tutorials or topic modules.
<br>

# Introduction
Scientific topics (especially those pertaining to health and wellness) frequently make the headlines of top newspapers and magazines but even highly educated people lack a reference frame to analyze their validity and context. It seems clear, however, by the popularity of these topics and their relevance to day-to-day life that there is a market for a learning framework to enable self-study of some popular topics. Cocktail Party Biology (CPB) is a website that allows users to watch ‘quick and dirty’ tutorials that provide a jumping off point (as well as factual basics) for motivated learners to glean a more thorough understanding of a few key topics. Users can then test their understanding with short quizzes and continue their journey of biological discover. In short, CPB fills a current void in adult education of commonly discussed (but often poorly understood) biological themes.
<br>

# Background
One need only glance at their Facebook feed or at the front page of online periodicals to see that scientific topics are popular points of discussion. That said, the way findings are often presented in these types of media is opaque (if not misleading) and doesn’t provide a solid reference to readers hoping to better understand a given topic.

This problem is frequently discussed, both in the media and in scientific circles. A
2014 NPR article described the gap by comparing headlines from reputable media sources (such as Time, the Washington Post, and USA Today) with the published results. While the articles described a causative effect between marijuana usage and brain changes, the study described did not claim causation—merely describing the observation that there were differences in brain structure. The article noted that the solution was ‘better, broader, more open discussion…of scientific results’ (Noë 2014). A more exhaustive study of the ‘gap between science and media’ published in PNAS similarly concluded that there was a colossal communication barrier between scientific and media sources (Peters 2013).

Discussion and communication are the buzzwords for improving the public’s grasp of scientific topics, but it is unclear how this admittedly noble goal can proceed if curious laypeople do not have the educational framework to discuss biology. While self-study programs exist (like popular websites Coursera or MIT OpenCourseWare, they are often more exhaustive and time-consuming than is merited for a ‘cocktail party level’ conversation. Plus, they’re not especially fun or engaging for users. CPB provides an alternative possibility- users are able to get the ‘TL;DR’ basics of a topic so that they can engage in a dialog on commonly reported issue without getting mired in long, boring lectures.
<br>

# Methods
The CPB website was created using Google App Engine in conjunction with the webapp2 python framework. Google App Engine was chosen in part because the author already had a vague understanding of how it worked, but mostly because it is an easy to use framework for creating a website. The code required to generate the pages (see the README file for a more exhaustive description) implemented CSS to create a template and HTML code to modify and store variables.

Most of the technical aspects of the webpage (such as user signup, login, verification, and password handling) was modified from a previous implementation of the webapp2 user functionality (Bahgat 2014). A User model extended the webapp2 user class to include a level variable for a given user. Using these functions, a user is able to generate an account that stores their name, login information, and level. In addition, pages were created to host a home page, about page, and various tutorial, quiz, and grading pages.

The tutorial videos were created using GoAnimate, an online program to streamline short animated videos, and then uploaded to YouTube. The tutorials were written by the author with information gleaned from a variety of sources (Pedersen 2015; Williamson and Feyer 2000; “Are You Getting Enough Sleep?” 2015; “Cancer Basics” 2015; “Short- and Long-Term Effects of Sleep Deprivation” 2015). The quiz module was implemented by generating Quiz and Test classes in python that parsed csv files containing quiz questions. Tests could then be generated within the main python file and passed as variables to the associated pages. For development purposes, a page to reset a user’s level was included.
<br>

# Results
The product of these methods was (fortunately) a functional CPB website. Several beta testers (mainly relatives and friends of the author) were able to successfully create accounts and use the tutorial and quiz pages without incident. Furthermore, they were able to logout of their accounts and login on different machines and their information was not altered.

Initially, the quiz function was going to be created using the SQL programming language but due to Google App Engine constraints (the author was very unwilling to pay for Google’s database hosting service) it was coded using python instead.
<br>

# Discussion
CPB proved very successful in its attempts to create a workable website and interesting, informative tutorials. The current tutorials include a ‘how to’ for using CPB, a ‘how to discuss science for assholes’ guide, a brief introduction to cancer biology, and a discussion of sleep deprivation. Two more videos were initially meant to be included on antibiotic resistance and media coverage of natural medicine, but were time prohibitive. The quizzes for the same first four topics were also sufficiently straightforward. The author would highly recommend taking the last two quizzes (even though they are empty) as there is an amusing ‘Easter egg’ when the final level is completed.

In future, CPB could very easily be extended. The obviously possibility would be simply to add more tutorial videos on popular topics. It would also be helpful (but proved surprisingly challenging) to provide more specific feedback on quizzes, i.e. which questions were answered incorrectly and hints as to why the answer was incorrect. Another modification could be to create ‘modules’ on a given topic. For instance, instead of one video on cancer biology, there could be a separate series of videos and tutorials pertaining to that topic. This would function similarly to the level system currently used by CPB except that users would be able to proceed through levels within the module itself. The result of this change would be that users could focus more on topics that specifically interested them.

Hopefully, CPB provided an interesting and informative diversion for the users who worked through the various levels. While it was challenging to make, the result is functional and might provide a jumping off point for other attempts to encourage a more fruitful discussion of biology.
<br>

# References
“Are You Getting Enough Sleep?” 2015. CDC. Accessed December 7. http://www.cdc.gov/features/sleep/.

Bahgat, Alessandro. 2014. webapp2-User-Accounts. Python.

“Cancer Basics.” 2015. American Cancer Society. Accessed December 7. http://www.cancer.org/cancer/cancerbasics/index.

Noë, Alva. 2014. “When Science Becomes News, The Facts Can Go Up In Smoke.” NPR. May 4. http://www.npr.org/sections/13.7/2014/05/02/308926616/when-science-becomes-news-the-facts-can-go-up-in-smoke.

Pedersen, Traci. 2015. “24 Hours Without Sleep Can Lead to Schizophrenia-Like Symptoms.” Psych Central. Accessed December 7 http://psychcentral.com/news/2014/07/12/24-hours-without-sleep-can-lead-to-schizophrenia-like-symptoms/72414.html.

Peters, Hans Peter. 2013. “Gap between Science and Media Revisited: Scientists as Public Communicators.” Proceedings of the National Academy of Sciences 110 (Supplement 3): 14102–9.

“Short- and Long-Term Effects of Sleep Deprivation.” 2015. Palo Alto Medical Foundation. Accessed December 7. http://www.pamf.org/sleep/about/healtheffects.html.

Williamson, A, and A Feyer. 2000. “Moderate Sleep Deprivation Produces Impairments in Cognitive and Motor Performance Equivalent to Legally Prescribed Levels of Alcohol Intoxication.” Occupational and Environmental Medicine 57 (10): 649–55. doi:10.1136/oem.57.10.649.
