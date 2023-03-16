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

### Commit 3 (17/03/22)
Third commit, pretty simple actually. I just added the structure for the second main section which is the 'About Us' section of the page. All done through HTML, separated this page into sections using divs. 

Even re-used same main and sub heading elements but of course just changed the content. 