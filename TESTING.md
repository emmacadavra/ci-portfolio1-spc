# **The Sheffield Philharmonic Chorus - Testing**

## **Table of Contents (Testing):**
1. [**Testing Throughout Development**](#testing-throughout-development)
    * [***Overview***](#overview)
    * [***Responsive Design and Functionality***](#responsive-design-and-functionality)
    * [***Testing of Site Features***](#testing-of-site-features)
    * [***Bugs***](#bugs)
        * [*Validation Issues*](#validation-issues)
    * [***Accessibility***](#accessibility)
1. [**Testing Post-Development**](#testing-post-development)
    * [***Validation***](#validation)
        * [*HTML Validation*](#html-validation)
        * [*CSS Validation*](#css-validation)
        * [*Lighthouse Scores and PageSpeed Insights*](#lighthouse-scores-and-pagespeed-insights)
    * [***Unresolved Bugs***](#unresolved-bugs)

## **Testing Throughout Development**

### **Overview**

During development, I manually tested the website as I went along by using the 'python3 -m http.server' command in GitPod's VSCode workspace. This created a live version of the website, and every time I saved my work on GitPod I could refresh the page to see whether my code was working as intended. Google Chrome is my default browser, so I was predominantly using Chrome's DevTools to allow me to test the content across different screen sizes, as well as using it as a first point of call for bug fixes, as it enabled me to tweak the code, disable certain elements and add to them without directly impacting the website itself. 

At various stages throughout development, before deploying the website to GitHub Pages, I made the server I was working on public so that I could test it on other devices such as my mobile phone. I would also share it with certain people to see how certain things looked on their devices, asking them to confirm that the site was functional and/or visually appealing so that I could get an idea of how the website performed across a variety of devices.

Once I was happy with the overall design of the website, I deployed it to GitHub Pages so that I could share the link with more people, and begin making necessary tweaks and debugging more efficiently.

### **Responsive Design and Functionality**

(How I tested responsive design)

The site's functionality has been tested and confirmed as fully responsive across different breakpoints with no issues on the following browsers on both mobile and desktop:

* Google Chrome
* Mozilla Firefox
* Microsoft Edge
* Safari

### **Testing of Site Features**

(How I tested the features of the website - ie, forms, links, layout)

### **Bugs**

(Bugs, including border-box sizing, horizontal scroll on form-submission, grey bottom of section-three, page not found due to incorrect file paths on form-submission page, w3c issue with hamburger html, etc)

#### **Validation Issues**

(issues with performance)

### **Accessibility**

(Testing of accessibility features - including changing from px to rem, testing using broswer default size, etc)

## **Testing Post-Development**

### **Validation**

In order to validate this website in terms of its HTML code, CSS code, and general overall quality, I used the [**W3C Markup Validation Service**](https://validator.w3.org/), [**W3C CSS Validation Service ('Jigsaw')**](https://jigsaw.w3.org/css-validator/), [**Google Chrome Lighthouse Tool**](https://chrome.google.com/webstore/detail/lighthouse/blipmdconlkpinefehnmjammfjpmpbjk?hl=en) and [**PageSpeed Insights**](https://pagespeed.web.dev/).

#### **HTML Validation**

The HTML for both index.html and form-submission.html was entered into the [**W3C Markup Validation Service**](https://validator.w3.org/), and both pages passed with no errors being detected.

![W3C Markup Validation Service - no errors found](docs/images/w3c-html-pass.PNG)

#### **CSS Validation**

The CSS code for this website was entered into the [**W3C CSS Validation Service ('Jigsaw')**](https://jigsaw.w3.org/css-validator/), and passed with no errors found.

![W3C CSS Validation Service - no errors found](docs/images/w3c-jigsaw-css-pass.PNG)

![W3C CSS Validation Icon - Valid CSS!](http://jigsaw.w3.org/css-validator/images/vcss)

#### **Lighthouse Scores and PageSpeed Insights**

When using Lighthouse, I made sure that tests were run in Incognito windows so that there could be no interferance from browser extensions.

Below are screenshots of the final, post-development results for both the mobile and desktop Lighthouse tests for index.html and form-submission.html. They were very consistent across multiple browsers and devices, with some tests coming back with perfect 100 scored in all categories, however these screenshots are ones I've taken from my own PC:

Desktop Lighthouse test - index.html:

![Desktop Lighthouse test - index.html](docs/images/index-desktop-lighthouse.png)

Desktop Lighthouse test - form-submission.html:

![Desktop Lighthouse test - form-submission.html](docs/images/form-submission-desktop-lighthouse.png)

Mobile Lighthouse test - index.html:

![Mobile Lighthouse test - index.html](docs/images/index-mobile-lighthouse.png)

Mobile Lighthouse test - form-submission.html:

![Mobile Lighthouse test - form-submission.html](docs/images/form-submission-mobile-lighthouse.png)

Below are screenshots of the final, post-development results for both the mobile and desktop PageSpeed Insights tests for index.html and form-submission.html. The desktop scores were consistent across multiple browsers and devices, but the mobile versions fluctuated fairly significantly, which I mention in the **'Unresolved Bugs'** section below these screenshots:

Desktop PageSpeed Insights test - index.html:

![Desktop PageSpeed Insights test - index.html](docs/images/index-pagespeed-insight-desktop.png)

Desktop PageSpeed Insights test - form-submission.html:

![Desktop PageSpeed Insights test - form-submission.html](docs/images/form-submission-pagespeed-insight-desktop.png)

Mobile PageSpeed Insights test - index.html:

![Mobile PageSpeed Insights test - index.html](docs/images/index-pagespeed-insight-mobile.png)

Mobile PageSpeed Insights test - form-submission.html:

![Mobile PageSpeed Insights test - form-submission.html](docs/images/form-submission-pagespeed-insight-mobile.png)

### Unresolved Bugs

There are two main noteworthy things about this website that I would consider unresolved bugs:

**PageSpeed Insights Performance Scores on Mobile**

The biggest and most important unresolved bug is that, when testing the mobile versions of index.html and form-submission.html on PageSpeed Insights, the Performance score often fluctuates. As mentioned in the **'Validation Issues'** section under **'Bugs'**, initially I found that the website scored much lower than desired in its Performance scores due to the high resolutions of the images used on the website (particularly for index.html), and a lack of explicit image widths and heights due to the responsive design model. I was able to improve this score by fixed by compressing the images as well as introducing a srcset rule to the HTML, so that the browser would load a lower resolution version of the image for screens under 1280px wide.

While this was enough to significantly raise the Performance score on Lighthouse to above 90, it was not enough to see the same consistency in PageSpeed Insights. As shown above in the final screenshots, the average high score I could get is 88, however the tests would vary, with one tester seeing average scores of around 85, but even in my own testing I sometimes received scores of 70 - 80. I do believe that a potential solution for this would be to resize the images again and add an additional srcset rule for small mobile screens, however I did find that a consistent issue I came across was due to the efficiency of GitHub's cache policy - which is beyond my control. Regardless, this is something I will keep in mind for the future, as well as learning how to use programs like GIMP that would allow me to resize, compress, and save images in next-gen formats such as WEBP.

**WCAG Colour Contrast Checker Failure**

When testing the website pages with the WCAG Colour Contrast Checker, I found that there were failures on my Form Submission page around the images. Although I understand that this is due to the background colour of the image containers, and the contaning div element - and that they do not actually contain any text - I would still consider this an issue that I would like to spend more time working out how to avoid.