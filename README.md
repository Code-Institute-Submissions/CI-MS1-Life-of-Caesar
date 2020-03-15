# The Life of Julius Caesar

The internet is full of high quality sources to help students of history, teachers and enthusiasts of history-studies access primary sources. These are however often overshadowed by more accesible sites with less thorough or vetted information such as wikipedia. A primary reason for users prefering the ease of use of Wikipedia is that Wikipedia was designed for browser-reading from the start. Most sites presenting historical documents online tend to either be direct copies of the text and sometimes actual photo-copies of the physical document!

The purpose of this site is to provide an educational site, designed to be used by teachers, students and enthusiasts of the Roman period. I have elected to take a 1911 translation of the Life of Julius Caesar, in the public domain, and republish it in a digital format with a design centered around providing modal-views explaining difficult concept as well as a thorough list of suggested further reading. The hope is that repackaging the content in this way will make reading Suetonius more accesible and fun, increasing interest in the user to read more about the Roman period.

# UX

This website is for the following three groups:

Teachers, looking to provide their students with a more accessible way to study the life of Julius Caesar.
Students, looking to find the original source material faithfully reproduced but also with annotations to make it easier to follow.
Enthusiasts, people who enjoy reading history, who will benefit from getting the original words of Suetonius while also finding links to further reading on the period.

As I have contacts who work in library and information science, I discussed the formatting of the read-now.html site extensively with them, to ensure it was easily browsed by readers. Eventually the decision was made to cut the full lenght text into 6 separate pages and add browsing between these pages through a bootstrap navbar dropdown and a pair of "back" and "forth" buttons stickied to the navbar.

## User stories:

# A teacher who wants to make Suetonius more accessible to their class could go straight for the "Read now!" link in the Navigation section and find the text reproduced in full.

# A student who is writing a paper on Caesar could utilize the chapter-browsing feature to quickly  find information and quotes in the read now segment

# Enthusiasts can use the further-reading segment to find a variety of resources to find more information about the Roman period, ranging from podcasts to books to documentaries.



# Features

A full-length reproduction of the Life of Caesar in a 1911 translation whose copyright has expired.
Browsing-by-chapter through the Navbar in relevant pages
A gallery of images related to the life of Caesar
A series of suggested further readings

## Testing process

I went through multiple stages of testing, before and after deployment. 

# Stage One - Pre-deployment testing 26/2

In this stage, I implemented boilerplate html-templating. I used Visual Studio Code to write all code, with added bootstrap functionality from a Marketplace add-in to generate template for basic bootstrap and grid function on index.html. ( Relevant link: https://marketplace.visualstudio.com/items?itemName=thekalinga.bootstrap4-vscode )

Once I had generated a workable general layout that matched my design in wireframes, I used the chrome DevTools to test a variety of resolutions and to test responsiveness. 
Once I was satisfied with this stage of the process, I performed my first commit on February 27th.

# Stage Two - Content testing 30/2

The site being primarily intended as a e-reading aide, UXD design for the chapters was very important for readability. I have friends in publishing and in library work and consulted
on the design of the chapter and navbar. Multiple iterations were gone through, with updates performed to the design for readability and navigation, particularily on small screens. Final CSS designs and all content was implemented on the 9th of March, at which point I did a new commit and push.

# Stage Three - Temporary deployment 8/3

I deployed the site to a temporary URL on a free hosting-service and shared the URLs with a set of testers, asking them to try different resolutions and report anything amiss. Testing was conducted on the following devices:

iPhone 5/6/7/8
Samsung Galaxy 7
Asus Zenphone 
iPad 4
Microsoft Surface Go
Desktop (Resolution: 1920x1080)

In addition, testing was done with DevTools on a variety of common resolutions.

A series of display errors on small resolution screens, related to the contact form. Multiple errors had occured on the pages labelled in this build as read-now-*, with chapters that were outside their display-box. This was a HTML error in the template I had made for this series of pages.

# Stage Four - REM compatibility 13/3

On the 12th of March, I was checking Slack for input on industry standards to make sure I was in compliance. I was informed that styling should be done in REM units, for better responsiveness. I reworked my CSS sheet to make it compatible with REM as the standard font-sizing measurement. While ensuring I was in compliance with other industry standards, I also found that I had mislabelled all read-now-*.html files, in that I had included dashes in their filenames. After manually testing the REM units to ensure there were no major display errors caused, I did a new git.
