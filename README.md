# How to use this website

First, you need to understand what this website is exactly. It is designed for minimal maintanance and to make changes as low effort as possible while making information easily accessible to the reader, in a consistent format.

To do that, most of it is generated automatically, using these things called Jekyll and Liquid. Jekyll is what converts all the pages into the html your browser needs and Liquid is the way that you automate repetetive tasks. You will see it with the curly braces scattered through the files of this website. Most of it can be ignored forever, with the only changes being a tweak to a data file here or there or some editing of a .md file which is just plain text with a few extras.


## Changing information about a sport

Information is found in 2 places for baseball and hockey and 3 places for soccer: there is the SPORTNAME.md file and the navigation.yml file located in the _data folder.

The navigation.yml file is a collection of information that we want in the site in many places. Having it in this format allows us to make changes in one spot that affect the links everywhere (so as to make it easy for the user to opperate the website) with minimal effort. So a change to the email address will only need to happen there to update every page to have a link accessible to the user.

The SPORTNAME.md file--say hockey.md for example--is the specific information about the sport that is **only needed on that page**. Edits there will only affect that sport's page. That is all in plain text with a little bit of markdown. The # symbol on the pages at the beginings of things just tell jekyll that that is a heading and to format it as such. 2 of them as is the case on that page mean that it is a second level heading.

Soccer is the special case as we have traditionally put more information on our page about the differences between the age groups. To make it manageable, they are divided into their respective ages in the _soccer folder. These again are just markdown files.

There are a couple of empty folders called _baseball and _hockey. They are not currently used for anything.

## Changing board member information

All board member information is found in the _data folder in the executives.yml and the navigation.yml files. navigation.yml has the info for the coordinators while executives.yml has the information about the executives.

If you want to change the contact info page, you can edit contact.md.

## Changing registration links

It should just update automatically through teamlinkt, but if we move from that it will need to be changed. To change them you'll need to edit the links in navigation.yml in the _data folder. Just cntrl-f for the current one and replace all instances with the new one(s).

## Changing the look

This website uses a newer version of css called scss to determine how it looks. The main thing you'll want to change in all likelihood is the colours. There are 4 main ones that you can do and they are all found at the very top of the page preceded by 2 dashes (--variableName). Changing one of these will change it's corresponding page uses, whether the text colour, the background colour, the highlight colour, and the accent colour. Remember to change them for both light and dark themes.

You can find that file in the _sass folder called main.scss. Remember, the values are near the top.

## Changing the logo

In assets folder, there is the images folder. In there are all the different versions of our logo used to put it in all the places one might want it. Just replace them with files of the same name and same dimensions of the new logo and that will be easiest.

If you want a new logo name, there are a couple places you'll need to change to reflect the new one in default.html around line 21 and then
