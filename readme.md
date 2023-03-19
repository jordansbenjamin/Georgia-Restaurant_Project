# Herly's Restaurant - Project

## Overview
This project is simply a practice for me, mainly practicing my CSS and in this case specifically my SCSS skills. As I'll be using SCSS to style this fake restaurant web page project. 

The goal is to familiarise myself with core components of CSS styling in general, but also getting used to the workflow of using SCSS. 

Especially with learning how to organise partial files, and using SCSS exclusive properties of using variables, mixins, functions, etc. 

On top of that, I will be using version control and practicing my git as well. I will be pushing this to my GitHub and it will be made public at least for now. 

Here we go.

### Commit 1 (15/03/23)
This is my first commit other than the initial commit, and essentially here I added the first part of the header element component. I created a logo using fontawesome icon and a border. I had to center it using flex which wasn't too bad. 

But then I was struggling to center the logo's text, I thought it had something to do with the display property and the flex. But turns out, it was because both text elements wasn't inside a div container at all. So flex was just treating it weird.

I definitely feel like flex is something I'm still trying to grasp, just need more practice. 

### Commit 2 (17/03/23)
This is the second commit and I'm just continuing what I did before and added the second part of the header element, as the header is actually split into 2 parts. The main header which consists of the logo and title of the restaurant has a class of brand, and the header banner which welcomes visitors to the website which includes a 'reservation' button. 

Since they both require similar centerting properties, I created a mixin to make it easier and actually include a parameter and changed the vlaues accordingly using relative units. Which is pretty awesome it can do that. 

And then after that, I styled the banner and the button. Here I learned more about nesting, and have a better idea of nesting overall. Especially learning how to use ampersand as it indicates parent element which is helpful. 

I'm also starting to see the power of variables and mixins in SCSS now, it's very helpful.

### Commit 3 (17/03/23)
Third commit, pretty simple actually. I just added the structure for the second main section which is the 'About Us' section of the page. All done through HTML, separated this page into sections using divs. 

Even re-used same main and sub heading elements but of course just changed the content. 

### Commit 4 (17/03/23)
Fourth commit, essentially just styled the About us section. 

I gave it a viewport height of 90 to give the visitor a point from where they scrol last which is the main header section. Otherwise if i go 100vh, it will take up the whole screen, perhaps I could even change it to 80 at some point but 90 will do for now. 

Next I positioned the image to left of the page, so as its sticking out from the left side of the screen. I also changed the opacity so it doesnt stand out as much. 

I actually divided the section into 2 parts, left and right. I have a display property of flex here and used align items center to center both sides horizontally. I probably should have start with this first. 

The section on the right include the pages main and sub heading, then a paragraph section and a button beneath it as well.

The only notable thing to mention here is the use of flex to not only align the items on the center but also I used flex direction column so that all the elements within this section aligns vertically. I'm starting to understand flexbox better.

Last thing, I used a pseudo element to select the first letter of the p element and added padding to its left. 

### Commit 5 (17/03/23)
Fifth commit and the fourth commit of the day! This commit conists of building markup strcuture for the next section of the page which is the gallery section. I've also included all the different images of food in there as well. 

### Commit 6 (18/03/23)
This was one was actually rather challenging, Essentially created a photo gallery using flexbox and I got confused when figuring out which container should actually hold the flex property. Turns out that the way I structured the markup was pretty clear already.

The class cards-wrapper is the container that used flex wrap to wrap all the items in that container, and in this case its the images. 

For each image which I labeled as a class of card, I had to set the width with a relative unit and also a viewport width. It also has an overlay layer that contains the food name, pricing and a button to order now. This was quite challenging to get right. 

I had to use the z-index to bring out the layer from the image, otherwise it just blends. Then figuring out it's first position which is outside of the layer, hence why I used a negative value for its asbolute position. Then of course added a transition along with a hover pseudo class to bring the element forward from it being hidden when hovered. 

### Commit 7 (19/03/23)
I completely forgot to update the readme when committing, but essentially during this commit it was simply adding markup for the footer section of the site. 

### Commit 8 (19/03/23)
Here I styled the footer section, I used flexbox to arranged the items within. The mixin here came in handy, I also added a flexdirection of column align the items vertically. 

Styled the social media icons as well, and even added a hover effect to change the color when hovered. 

Other than that, I added a copyright text section at the bottom. I somehow feel as if the footer might be a tad too large, but it's okay for now.

### Commit 9 (19/03/23)
Added markup for navigation section, hoping to create a hamburger menu. I separated the navbar into two sections, left and right. The left will have images just for aesthetics and right will include actual navigation section.  

The navbar itself will appear as an onclick event using checkboxes, this is my first time doing it, so will see how it works out.

### Commit 10 (19/03/23)
During this commit, I did the initial styling to the navigation section. I had to play around with the position of each element so that it would work when bringing up the navigation menu when clicked. 

I had to separate the left and right sections using viewport width, they both have a fixed position, so they would stay there whenever someones access the menu. 

The image section was given a position of absolute so that I can stack them diagonally, I also made it responsive using relative units. At the moment, it doesn't look so good on a large screen. I also gave the images a subtle box shadow to stand out a tiny bit. 

Other than that, there are some more specific styling I did, especially to the right section with the navigation links. I used a transition and hover effect to change the color but also the letter spacing, I thought that this was pretty cool.

### Commit 11 (20/03/23)
Things are getting even more complex now as I'm implementing the hamburger menu and making it work. 

At first, I had to create the shape of the menu which is a small square and positioned it on the top right corner of the page with a fixed position.

I wanted to separate the menu into 3 different lines, and I used the placeholder variable called fullSpace along with a display flex, with a column direction and of course justify content space around. 

The big part was using the pseudo class checked, this is part of the magic of onclick event using checkboxes, when checkbox is checked (in this case the hamburger menu) then the nav elements of right and left comes in. I see its checked position value at 0 to make this work. Otherwise its viewport width of right and left respectively are set to -50.

I added a cubic bezier transition so that when the navigation menu is called, it comes smoothly from both sides. This was awesome to implement. 

Probably the most challenging hurdle was figuring out how to change the hamburger menu to transition to an X. I used transform doing so, rotating its z axis accordingly for all 3 lines by 90deg.

However, to create the X, I had to take out the middle line and set it's opacity to 0. So that when the other 2 lines rotate to now a 40 degree angle, the middle line dissapeared. I also had to set the transform origin to its right side. 

More importantly, I had to use transition to give a delay so its animated smoothly.

This was by far the most challenging feature of the site so far.

### Commit 12 (20/03/23)
For this commit, it's all exclusively setting media breakpoints for certain elements of the webpage from the heading to the logo, description and button for the images so far. Responsive design is quite interesting, I'm still trying to wrap my head around this one.

There are other elements I have to add breakpoints to, but I thought the more obvious ones should be done first. I need a break.