# Doctor Diana-Voronina-Akhvlediani's website

The goal to this project was to create landing webpage only using HTML5, CSS3 and Bootstrap


## Demo
A live demo can be found [here](https://aleksandre19.github.io/ucmp/).

## UX

### User stories
The user of this website should understand what is the site about, what are keys and way it is special. 

### Strategy
My goal in the design was to catch user's attantion straight in the first look  and then expand and show sequently the key features and specifications.  

### Scope
To achive my goal I wanted to create some pleasant animation with hight quality images and some really eye caching text animiation to give them understanding: what is website about, what can they get and give a message about author's personality. Then continue sequently expanding and explaining information by smoothly moving from one section to another section. And finally finishing the page with section of free consultation.    

### Structure
I choosed landing page style. First section is for eye catching animation. Second section I use to expand information about method and whow how can it be done. Third section I use to show  by whom can it be done. Forth section I use to show author's experience by providing her's videos. Fifth section I use for feedbacks and finally in the end of the page when users probably should have the arised interest I provide the ability to get more information by sign up for free consultation.    

### Skeleton
[The sketch file on balsamiq](https://github.com/Aleksandre19/files/blob/master/daiana-website/dianas-website-sketch-balsamiq.pdf)

### Surface
On the [Adobe website](https://color.adobe.com/explore) I choosed the following schema:
[Color schema](https://github.com/Aleksandre19/files/blob/master/daiana-website/color-schema.jpg)

After determation of colors I drew design in Adobe Photoshop CC which can be viewed here:
[PSD file](https://github.com/Aleksandre19/files/blob/master/daiana-website/index.psd.zip)

## Technologies
1. HTML
2. CSS
3. Bootstrap (4.4.1)


## Features
This site uses the scrollSpy feature in Bootstrap with an extra JavaScript function added to create a 'smooth scrolling' effect. On the mobile divices the navbar is collapsed and it expands on tablets and desktop devices. The menu's links uses Hover.css effect to move up on hovering. I use Bootstrap's Scrollspy feature to mark menu's link when user is on appropriate section by changing color and making underline on the link . The site uses Bootstrap's Modal to pop up the singup form by clicking on Sign Up button in the first section. In the first section I use SVG file for WEIGHT & HEALTH's text to sequently animate strokes of this text with CSS3.


### Features Left to Implement
In the future I would like to: add sublinks to video's link to categorise and expand video's section, add blog section, write animation's script in Javsscript/Jquery, make to work registration's section, improve video section's look, animate modal's pop up window with Javascript/Jquery. 

# Describing the sections: 


## First - Animation Section
This is first section and it appears as soon as the page loads. User gets messages about webpage by animating texts and the images under those texts. This animation is done only by CSS3.
The WEIGTH & HEALTH text animation was done by using stroke-dasharray and stroke-dashoffset in CSS3 and animating them. The CSS code of this text's animation can be fount in /assets/css/style.css from line 439 to the line 658. 
Finally there is Sign Up Button. When user clicks on that button the Bootstrap's Modal window opens.

## Individual approach's section
In the beginning of this section user finds text which describes point of view of the health and it's connection to the weight. 
After this text comes the section’s title with icon which hides on the tablets and mobile devices. After the title comes blocks of steps each one by their's own icon. 
They are: gathering information, separation of pathologies and doing of research. On the mobile devices they are located vertically. On tablets and desktop devices those steps sections are located side by side. 
The style of the steps changes depending on the devices. On IPod Pro and desktop devices each steps’s title has background-image with it’s own color and also left side in the each step’s block has vertically right forwarded shadow.
Section’s background image changes in sizes depending on the devices. On the desktop devices with resolution in the width more than 1300px the section’s max-width is 1300px and margins to the left and right are auto. So it becomes centered.


## About Me's Section
This sections starts with title. The title has icon and underline. After the title comes a text about Doctor's biography. In the mobile divice the image is hidden.
The image to the right side is partly hidden on tablets and it becoms more visible as a device’s width increases  and it appears fully visible on the desktop devices.
Background image’s size changes depending on the devices. On mobiles and tablets background-attachment is scroll and on the desktop devices it has background-attachment: fixed; 
On the desktop devices with resolution in the width more than 1300px the section’s max-width is 1300px and margins to the left and right are auto. So it becomes centered.


## Video’s section
This section starts with title. The title has icon and underline. The icon shows on the tablets and desktop devices. On the tablets the icons is under the title and on the desktop it is beside to the title.
On the mobile and tablet devices there are two videos. On the desktop devices there are three videos which are horizontally aligned. On the tablets horizontally alignment stays and it changes to the vertically alignment on the mobile devices.
There is no background image on the mobile devices. It appears on tablet devices and has background-attachment: scroll. On the desktop devices the size of the background images changes appropriate to the desktop.
Also the background-attachment: scroll changes to background-attachment: fixed;

## Feedbacks section
This section also starts with title of section which has icon and underline. Icon appears on the tablet devices. On the tablets It is under the title’s underline and it aligns to the left on the desktop devices. 
On the mobile devices there are three quotes with the images. The images seats on the top of the quote’s blocks and crosses theirs border with almost half part of them selfs.
On the tablets and desktop devices the images of the quotes changes the positions and aligns to the left of the quotes. There appears also one vertical line under the middle of the images which starts from the top images and ends with last one.
The number of the quotes increases by one on tablets and desktop devices. This section has background image which size changes accordingly to the devices. On the mobile and tablet devices it has background-attachment : scroll and it changes to the background- attachment: fixed on the desktop devices.

## Consultation’s section
This section starts with question and one paragraph text. Then comes registration form with three inputs elements and one submit button. First and second are text type elements and they have required attribute.
Third one is for email and if a user doesn’t enter a email it alerts to use email format for this input. The email input element has required attribute. The form tag has two attributes: action and method.
First one has value # and second one has the value POST. This section has background image which’s size and style changes deppending on devices it was viewed. On the iPod Pro and desktop devices I use two div tags with CSS property position: absolute and z-index: 1 to set and adjust left and right background images.

## Footer
The footer consists with three columns. The right one is a column for section’s links including the ones which are not in main menu. They are: Individual approach and feedback’s sections.
The links changes a colours as same as other links in the footer by hovering over them. The change is done by CSS3’s transitions property. 
Each column on the mobile devices except for the first one have top border which disappears on the tablets and desktops devices. Second column is for social links and third column is for videos links.
To achieve something like a content balance in the footer the social links and the videos links swaps the places on the tablets and desktop devices. Which is done by bootstrap’s class: d-none and d-md-block.
In the very end of the footer there is copyright text.


# Testing

If you try to submit the registration form with an invalid email address, there will be an error noting that there is invalid email address. Furthermore, the 'required' attribute is added to the 'name, and ‘last name’ fields, so if those fields are not filled , the form will not be submited. If all field are valid, the page will reload.

All video links will open in a new tab using 'target="_blank”.  All links have been manually tested to ensure that they are pointing to the correct destination.

This site was tested in all modern browsers (Chrome, Safari, Internet Explorer, FireFox), on some mobile devices (iPhone 6: Chrome and Safari, iPad, Samsung Galaxy) and in google chrome inspect to ensure compatibility and responsiveness. During the testing phase, I realized that background-attachment: fixed was not compatible with iOS browsers. On Chrome and Safari in iOS, the background photos appeared zoomed-in and blurry. To fix this, the background-attachment: scroll property value was added in a media query. 

  I found also that registration form had the margin problem on mobile devices and it was fixed by media query in style.css file. 

  In the about me section on the mobile device the text’s hight was more than section and was overlapping the section under it. It was fixed also with media query.

  In the Safari browser there was about me link’s problem in top menu. It was breaking. It was fixed by CSS property white-space: nowrap; 

# Deployment 

This site is hosted using GitHub pages, deployed directly on the master branch.
The link can be found [here]( https://aleksandre19.github.io/cv-ucmp/)
The deployed site will update automatically upon new commits to the master branch. In order for the site to deploy correctly on GitHub pages, the landing page must be named index.html.
To run locally, you can clone this repository directly into the editor of your choice by pasting git clone (https://aleksandre19.github.io/ucmp/)
into your terminal. To cut ties with this GitHub repository, type git remote rm origin into the terminal.
 
# Credits

## Content

All content was written by me.

## Media

The photos for animation I purchased on https://www.istockphoto.com/se. 

Other photos for different sections was downloaded from https:/www.pexels.com. 

Videos was taken from Diana’s YouTube page.

Feedback images are my and my family’s photos.

# Acknowledgements


The scrollSpy delay JavaScript function was found here [here](https://github.com/Code-Institute-Solutions/StudentExampleProjectGradeFive).

The SVG file's animation i found [here](https://www.youtube.com/watch?v=vJNVramny9k).

I used Hover.css library to make menu links jumping effect on hovering. The link for that is [here](https://ianlunn.github.io/Hover/)  

To active the link in the top menu at appropriate webpage i use this [here](https://getbootstrap.com/docs/4.0/components/scrollspy/)


