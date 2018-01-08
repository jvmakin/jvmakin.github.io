---
layout: post
title: Creepy Chicago App
date: 2016-08-31
---
<a class="poem-title" href="https://github.com/jvmakin/mpcs51030-2016-summer-project-jvmakin"> Source Code </a>

# An app which allows users to take an interactive tour of the creepy side of the Windy City
This app was created as a final project for the iOS Application Development course. It has not been updated to run with Swift 3 and the Backendless license has expired, but the source code is still available.

# Application Rationale
When visiting a new city or exploring the city you live in, it isn’t hard to find bus or walking tours of a the main attractions. Unfortunately, if you’re the kind of person who finds themself wondering about what lies beneath the gleaming monuments, tourist traps, and generic museums, that type of tour is going to disappoint. Creepy Chicago seeks to provide a different viewpoint on the Windy City: one that horror fans, true crime aficionados, and curious locals can appreciate. This app curates free ‘creepy’ tours of Chicago that shows this great city through the lens of the most disturbing events that have occurred here. Not only are the tours painstakingly researched and refreshingly unique, they also allow the user to explore the sights at any time and at their own pace. Plus, each tour provides a cohesive picture of a specific theme – be it the life and crimes of one of Chicago’s many serial murderers or a rundown of the most paranormally active hotspots.

Currently, the App Store features a broad range of tour-based apps for a wide variety of cities, including Chicago. Most of these, however, are of the tourist-trap ilk and are either paid apps or require in-app purchases. Of the apps that cater to the demographic served by Creepy Chicago (including a Jack the Ripper themed tour app), none are available in the Midwest nor do most of them offer multiple tour options. Creepy Chicago will therefor fill the chalk-outline shaped hole left in the hearts of Midwest dwellers who want to take tours but only if they are unlikely to sleep the following night.

# Application Implementation
Creepy Chicago utilizes two different methods of data storage to provide a seamless user experience. User information, such as username, password, and progress through the various tours and stops, are stored on the Backendless platform. Backendless is a second-party framework that provides for hosting of simple data (i.e. strings, integers etc.) on their servers. This allows users to login from any iPhone device and access the same experience plus ensures rapid and accurate updating of the user interface. Tour information (tour names, location coordinates, and short summaries) and audio files for the tours are stored on the app itself to limit the number of network calls made to download large files and to ensure that a slow network does not preclude enjoyment of the app.

The user experience is driven in large part by location-based features as well as the integration of audio recordings. Creepy Chicago uses user location to provide directions to a tour stop as well as to unlock stop descriptions. Much like Pokemon Go did, this could encourage people to get outside, be active, and nose around decades-old murder scenes. Once unlocked, the audio files, which are quite creepy and theatrical, allow users to immerse themselves in the experience. The visual user interface probably violates every single one of Apple’s minimalist and elegant design standards, but does so knowingly and with the intention of creating a campy, B horror movie vibe.

# Screenshots
<div>
<img class="border-right" src="{{ site.url }}/img/App1.png" alt="" width="209.4" height="372.6"/>

<img class="border-right" src="{{ site.url }}/img/App2.png" alt="" width="209.4" height="372.6"/>

<img class="border-right" src="{{ site.url }}/img/App3.png" alt="" width="209.4" height="372.6"/>
</div>

<div>
<img class="border-right" src="{{ site.url }}/img/App4.png" alt="" width="209.4" height="372.6"/>

<img class="border-right" src="{{ site.url }}/img/App5.png" alt="" width="209.4" height="372.6"/>

</div>
