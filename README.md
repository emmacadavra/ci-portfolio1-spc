# **The Sheffield Philharmonic Chorus**
## **Site Overview**
The Sheffield Philharmonic Chorus is the foremost large mixed-voice choir in Sheffield, South Yorkshire, and the purpose of this website is to act as a first stop for people interested in joining the choir. The choir’s ethos is to share its love of a large range of choral music by performing it periodically, and to continue to do this they rely on new members seeking them out and joining them.
​
![Am I responsive screenshot](screenshot of amiresponsive)

## Table of contents:
1. [**Site Overview**](#site-overview)
1. [**Planning stage**](#planning-stage)
    * [***Target Audiences***](#target-audiences)
    * [***User Stories***](#user-stories)
    * [***Site Aims***](#site-aims)
    * [***Colour Scheme***](#colour-scheme)
    * [***Typography***](#typography)
1. [**Current Features Common to All Pages**](#current-features-common-to-all-pages)
    * [***Header and Navigation Bar***](#header-and-navigation-bar)
    * [***Section Images***](#section-images)
    * [***SPC Logo***](#spc-logo)
    * [***Sign-Up Form***](#sign-up-form)
    * [***Form Submission Page***](#form-submission-page)
    * [**Footer**](#footer)
1. [**Future-Enhancements**](#future-enhancements)
1. [**Testing Phase**](#testing-phase)
1. [**Deployment**](#deployment)
1. [**Tech**](#tech)
1. [**Credits**](#credits)
    * [**Honourable mentions**](#honourable-mentions)
    * [**General reference**](#general-reference)
    * [**Content**](#content)
    * [**Media**](#media)

## **Planning stage**
### **Target Audiences:**

* Users interested in singing choral music with other like-minded people
* Users interested in performing choral music as part of a large choir
* Users who have seen or heard the Sheffield Philharmonic Chorus and want to find out more
* Users interested in joining a choir in the Sheffield area who do not know about the Sheffield Philharmonic Chorus

### **User Stories:**

* As a user, I want to see the subject matter of the page.
* As a user, I want to navigate the page to find what I require quickly and easily.
* As a user, I want to learn more about what the choir does.
* As a user, I want to learn more about when the choir rehearses.
* As a user, I want to register to join the choir.

### **Site Aims:**

* To inform the user about the choir and its rehearsals
* To maintain the choir's professional reputation whilst demonstrating its friendly approach
* To inform the user about how they can register their interest to join the choir

### **Colour Scheme:**

(INFO ABOUT COLOURS)

## **Typography:**

* Throughout the page, there are 3 fonts used:
    * Playfair Display
    * Roboto Serif
    * Roboto Slab
​
* The ‘Playfair Display’ font was chosen to match the Sheffield Philharmonic Chorus logo, seen in the logo in the ‘Join Us’ sections of the site.
* Roboto Slab was chosen as the font for the majority of the body of the site as it maintains readability whilst appearing sophisticated.
* Roboto Serif was chosen for the opening paragraph due to it being better suited to italic styling than Roboto Slab.
* All fonts were sourced from Google fonts, as stated in the credits.

## **Current Features Common to All Pages**
#### **Header and Navigation Bar**

The header sits atop the page in a fixed position, so that the site title is always visible to the user, for a simple and pleasant user experience. Within the header, there is a navigation bar, which appears in two separate forms depending on the screen size of the user.

(screenshot of larger screen)

On larger screens, such as laptops and desktops, the navigation bar displays all three navigation links in the top-right corner of the screen.

(screenshot of mobile screen - menu closed)
(screenshot of mobile screen - menu open)

On smaller screens, such as tablets and mobile phones, the navigation bar menu appears as a hamburger menu in the top-right corner, which expands when clicked on to reveal the page links. The purpose of this is to prevent the header from taking up too much room on smaller screens, providing an optimal experience.

In each case, the links are obvious and readable for a smooth user experience.

#### **Section Images**

Sections one and two (‘Home’ and ‘About Us’) feature a large image that makes up 50% of the section as a whole. The decision to include images that take up a large part of each section was made in order to make the site more visually eye-catching and appealing, with the additional benefit of not overloading the user with too much text at once.

(screenshot of smaller screen)

On smaller screens, the images appear landscape, and are positioned below the content of the section.

(screenshot of larger screen)

On larger screens, the images appear next to the content of the section, with section two’s order having been reversed for an engaging visual effect.

(section one image)

Section one’s image was chosen for its eye-catching location’s grandeur, and sets a very professional and serene tone. It also suggests an important level of inclusiveness for those who prefer to wear masks since the outbreak of the Covid-19 pandemic.

(section two image)

Section two’s image is a lot more casual, and this is to show the other side of the chorus which is friendly, approachable, and full of smiles. This is so that users of the website can see that the choir is both professional, and also relaxed and welcoming.

The images are responsive, and will adapt to the screen size and position without stretching or shrinking.

#### **SPC Logo**

Section three contains the Sheffield Philharmonic Chorus logo, in reverse colours to that of the header. This contrast is visually pleasing, and helps to establish the brand in the eyes of the users. It appears circular so as to stand out from the other images on the page.

(screenshot of logo on smaller screen)

On smaller screens, the logo appears at the very bottom of the page, above the footer.

(screenshot of logo on larger screen)

On larger screens, the logo appears on the left-hand side of the screen, before the sign-up form.

The logo image is responsive, and a maximum width has been set so that it does not distort or stretch above the image’s maximum dimensions.

#### **Sign-Up Form**

Section three of the site also contains a sign-up form, which is a crucial element to this website as its aim is to provide people with a way of joining the choir. The form features two fieldsets which clearly define which information is required from the user.

(screenshot of fieldset one)

The first fieldset asks for personal details and includes three input fields - two text fields (clearly labelled 'First Name' and 'Last Name') and an email field (clearly labelled 'Email Address') - all three of which are marked as 'required'.

(screenshot of fieldset two)

The second fieldset uses radio button input so that the user can select which voice part they would sing in the choir. The first radio button input is marked as required so that one of the eight options must be selected in order to validate the form. Each option is clearly labelled and separated into four separate voice parts.

(screenshot of form on mobile)

(screenshot of form on desktop)

The form is responsive, with the fieldsets and additional text being set to display as columns on smaller screens, and rows on larger screens. This is achieved using Flexbox CSS rules.

The Submit button is made distinct from the rest of the form by using the inverse of the form's colours - rather than dark grey text on yellow, the button itself is dark grey with yellow text that is larger than the form's text. 

#### **Form Submission Page**

The form submission page was created to emulate the experience of submitting a form. In this particular instance, because this website is for education purposes and is not designed to collect data, no form method has been defined. However, in order to create a professional looking website, the form-submission page acts as a confirmation of form validation that the user can understand. It also includes the same header and footer as the main site page, so that the user can quickly and easily navigate back to the homepage and other sections.

(screenshot of form submission page)

#### **Footer**

The footer sits at the bottom of the webpage and includes four social media links, all of which are indicated by a logo from Font Awesome. As they are logos only, they also include an aria-label so that screen readers can easily understand the purpose of each icon. All links are set to open in a new tab, so that they do not disrupt the user experience.

(screenshot of footer)

## **Future-Enhancements**

As this is my first major project as part of Code Institute's Full Stack Software Development course, I am limited by the current scope of my knowledge.

If I had more time and knowledge, I would see the following enhancements made:

* JavaScript: I feel that use of JavaScript would greatly improve the functionality of this website, and allow for even more interactive elements to be included on the website. For example, where a hamburger menu has been created in CSS for the purpose of this project, I would replace it with a more intuitive JavaScript hamburger menu. I would also like to include a live Twitter feed, and interactive view of upcoming concerts.
* Functional sign-up form: As mentioned above, for the purposes of this project the sign-up form I have created does not collect any data from users, but a future enhancement could be to create a sign-up form that fulfils its purpose, with a corresponding database set up ready to receive and store the information.
* Additional content: As mentioned in the credits, a large portion of this site's content was taken from the Sheffield Philharmonic Chorus' website - though the information provided in this project pales in comparison to the rich amount of information and detail given on their official website. Given more time, I would have liked to include more of this information, such as with a page about the SPC's history, and another with a gallery, et cetera.
* Improved accessibility: This website utilises viewport heigh calculations for laptop and desktop screen sizes, which looks slick and appealing to users. However, it is noted in the 'Bugs' section below that while the units of measurement I have used wherever possible are rem and em so that increased default font sizes can be taken into account, the viewport height calculations interfere with this level of accessibility. Extra time would be needed to investigate how best to maintain the look of the website (with this viewport height styling rule in mind) whilst also removing barriers for those who use larger font sizes in their browsers.

## **Testing Phase**

During development, I manually tested the website in Chrome, predominantly by using Chrome's DevTools to allow me to test the content across different screen sizes.

I also made the server public and shared it with several people, asking them to test it on their devices. This was at varying stages of the development, and across different devices so that I could get an idea of whether the site looked good to different people at different sizes.

The site has also been tested and confirmed as fully responsive with no issues on the following browsers:
* Google Chrome
* Mozilla Firefox
* Microsoft Edge

## **Bugs**



## **Deployment**


## **Tech**

The technologies used in the making of this website are:
* HTML5
* CSS3

## **Credits**
### **Honourable mentions**

* [Damon Kreft](https://github.com/damon-kreft) - Thank you for your unwavering patience and support, and your enthusiasm and encouragement when I have struggled. Your experience is invaluable to me.

* [Richard Wells](https://github.com/D0nni387) - Thank you for your mentorship so far, and for always going out of your way to make sure I'm on the right track. I appreciate your advice and guidance very much.

* [The Sheffield Philharmonic Chorus](https://sheffieldphil.org/) - Thank you to the Sheffield Philharmonic Chorus, in particular to Anne Adams who is the SPC administrator, for allowing me to use their content in order to progress my skills in software development. I'm proud to be a member of the chorus!

### **Code:**


### **Content:**


### **Media:**