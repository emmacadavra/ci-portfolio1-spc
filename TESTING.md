# **The Sheffield Philharmonic Chorus - Testing**

## **Table of Contents (Testing):**
1. [**Testing Throughout Development**](#testing-throughout-development)
    * [***Overview***](#overview)
    * [***Responsive Design and Functionality***](#responsive-design-and-functionality)
    * [***Testing of Site Features***](#testing-of-site-features)
    * [***Bugs***](#bugs)
    * [***Accessibility***](#accessibility)
1. [**Testing Post-Development**](#testing-post-development)
    * [***Validation***](#validation)
        * [*HTML Validation*](#html-validation)
        * [*CSS Validation*](#css-validation)
        * [*Lighthouse Scores*](#lighthouse-scores)
    * [***Unresolved Bugs***](#unresolved-bugs)

## **Testing Throughout Development**

### Overview

During development, I manually tested the website as I went along by using the 'python3 -m http.server' command in GitPod's VSCode workspace. This created a live version of the website, and every time I saved my work on GitPod I could refresh the page to see whether my code was working as intended. Google Chrome is my default browser, so I was predominantly using Chrome's DevTools to allow me to test the content across different screen sizes, as well as using it as a first point of call for bug fixes, as it enabled me to tweak the code, disable certain elements and add to them without directly impacting the website itself. 

At various stages throughout development, before deploying the website to GitHub Pages, I made the server I was working on public so that I could test it on other devices such as my mobile phone. I would also share it with certain people to see how certain things looked on their devices, asking them to confirm that the site was functional and/or visually appealing so that I could get an idea of how the website performed across a variety of devices.

Once I was happy with the overall design of the website, I deployed it to GitHub Pages so that I could share the link with more people, and begin making necessary tweaks and debugging more efficiently.

### Responsive Design and Functionality

(How I tested responsive design)

The site's functionality has been tested and confirmed as fully responsive across different breakpoints with no issues on the following browsers on both mobile and desktop:

* Google Chrome
* Mozilla Firefox
* Microsoft Edge
* Safari

### Testing of Site Features

(How I tested the features of the website - ie, forms, links, layout)

### **Bugs**

(Bugs, including border-box sizing, horizontal scroll on form-submission, grey bottom of section-three, page not found due to incorrect file paths on form-submission page, w3c issue with hamburger html, etc)

### **Accessibility**

(Testing of accessibility features - including changing from px to rem, testing using broswer default size, etc)

## **Testing Post-Development**

### Validation

In order to validate this website in terms of its HTML code, CSS code, and general overall quality, I used the [**W3C Markup Validation Service**](https://validator.w3.org/), [**W3C CSS Validation Service ('Jigsaw')**](https://jigsaw.w3.org/css-validator/), and [**Google Chrome Lighthouse Tool**](https://chrome.google.com/webstore/detail/lighthouse/blipmdconlkpinefehnmjammfjpmpbjk?hl=en).

#### HTML Validation

The HTML for both index.html and form-submission.html was entered into the [**W3C Markup Validation Service**](https://validator.w3.org/), and both pages passed with no errors being detected.

![W3C Markup Validation Service - no errors found](docs/images/w3c-html-pass.PNG)

#### CSS Validation

The CSS code for this website was entered into the [**W3C CSS Validation Service ('Jigsaw')**](https://jigsaw.w3.org/css-validator/), and passed with no errors found.

![W3C CSS Validation Service - no errors found](docs/images/w3c-jigsaw-css-pass.PNG)

![W3C CSS Validation Icon - Valid CSS!](http://jigsaw.w3.org/css-validator/images/vcss)

#### Lighthouse Scores

When using Lighthouse, I made sure that tests were run in Incognito windows so that there could be no interferance from browser extensions..

Below are screenshots of the results for both the mobile and desktop tests for index.html and form-submission.html:

Desktop Lighthouse test - form-submission.html:



Desktop Lighthouse test - index.html:



Mobile Lighthouse test - form-submission.html:



Mobile Lighthouse test - index.html:



### Unresolved Bugs

(Performance on mobile due to responsive design, that one technical issue with WCAG)