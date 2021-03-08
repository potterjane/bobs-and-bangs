# Bobs & Bangs - Testing details

[Main README.md file](README.md)

[View website in GitHub Pages](https://potterjane.github.io/bobs-and-bangs/)

## Table of Contents

1. [**Automated Testing**](#automated-testing)
    - [**Validation services**](#validation-services)
    - [**Accessibility services**](#accessibilty-services)
    - [**Other Evaluation services via Lighthouse**](#other-evaluation-services-via-lighthouse)
2. [**User Stories Testing**](#user-stories-testing)
3. [**Manual Testing**](#manual-testing)
    - [**Testing on desktop screens**](#testing-on-desktop-screens)
    - [**Testing on tablet and phone screens**](#testing-on-tablet-and-phone-screens)
4. [**Bugs discovered**](#bugs-discovered)
    - [**Solved bugs**](#solved-bugs)
    - [**Unsolved bugs**](#unsolved-bugs)
5. [**Further Testing**](#further-testing)

## Automated Testing

### Validation services
- [W3C Markup Validation]( https://validator.w3.org/) was used to validate all the HTML pages (home, about, services, contact, booking).
No errors or warnings to show on any of the HTML pages.
- [W3C CSS validation](https://jigsaw.w3.org/css-validator/) was used to validate CSS. 
No errors were found, however there were some warnings. 
This [StackOverflow](https://stackoverflow.com/questions/25946111/importing-css-is-ending-up-with-an-error)
post explained that the warning, 'Imported style sheets are not checked in direct input and file upload modes'
meant that it did not validate the imported style sheet on line 1. In other words, not actually a warning, just information.
The other warnings were related to 'webkit', 'moz' and 'o' property. 
However, this developer did not remove these properties because it helps support browser compatibility efforts. 

<div align="center"><h4>Results from CSS validator</h4>
<img src="screenshots/css-validator-results.png" alt="Screenshot: Results from CSS validator" >
</div>

### Accessibility services
- [Lighthouse in ChromeDev Tools](https://developers.google.com/web/tools/lighthouse#devtools) was used to
evaluate the accessibilty on all of the website's page in incognito mode, as recommended (see screenshot below). 
The report generated an Accessibility rate of 100 out of 100.
- [WAVE Web Accessibility Evaluation Tool](https://wave.webaim.org/) was also used to evaluate the accessibilty
on all of the website's pages in incognito mode. No errors were detected.

<div align="center"><h4>Lighthouse error outside incognito mode</h4>
<img src="screenshots/incognito-lighthouse.png" alt="Screenshot: Lighthouse error outside incognito mode" >
</div>

### Other Evaluation services via Lighthouse
- [Lighthouse in ChromeDev Tools](https://developers.google.com/web/tools/lighthouse#devtools) was also used
to evaluate performance, best practices and SEO on all of the website's pages in incognito mode.
The report generated a Performance rate an average of 96 out of 100.
The report generated a Best Practices rate of 100 out of 100.
The report generated a SEO rate of 100 out of 100.

## User Stories Testing

## Manual Testing

### Testing on desktop screens

### Testing on tablet and phone screens

## Bugs discovered

### Solved bugs
1. **Jumping behaviour of the uncollapsed navbar**

    When collapsing and uncollapsing the navbar for mobile and tablet screens, the entire ul presented a 'jump' behaviour.

    **How this developer fixed it:**

    With the help of the [SimplySmartMedia](https://simplysmartmedia.com/2016/06/heres-why-your-bootstrap-collapsed-alert-jumps-when-expanded/)'s post, 
    the ```class="nav-container-collapse"``` was moved from the ```<ul>``` element to the grandparent ```<div>``` element.

    ```html
    <div class="collapse nav-container-collapse" id="navbarToggleExternalContent">
                    <div class="p-4">
                        <nav>
                            <ul>
                                <li>
                                    <a href="index.html"><h5>home</h5></a>
                                </li>
                                <br>
                                <li>
                                    <a href="about.html"><h5>about</h5></a>
                                </li>
                                <br>
                                <li>
                                    <a href="services.html"><h5>services</h5></a>
                                </li>
                                <br>
                                <li>
                                    <a href="contact.html"><h5>contact</h5></a>
                                </li>
                                <br>
                                <li>
                                    <a href="booking.html"><h5>booking</h5></a>
                                </li>
                            </ul>
                        </nav>
                    </div>
    ```

2. **Jumping behaviour of the customer review carousel**

    On the Home page, carousel slide number 2 had an extra paragraph line in comparison to the other slides, 
    which caused the whole carousel to present a 'height jump' behaviour when slide 2 was presented in desktop screens.

    Adjusting the number of paragraph lines to be equal for each slide did not solve the 'height jump' issue for smaller screens.

    **How this developer fixed it:**

    In order for the carousel to be fully responsive and not present a 'height jump' behaviour on any screen sizes,
    ```min-height``` and ```max-height``` was set to the ```#carouselExampleIndicators``` and ```font-size```
    was adjusted for each ```.carousel-item``` under ```@media screen```.

    For example:

    ```css
        @media screen and (max-width: 576px) {

            #carouselExampleIndicators {
                min-height: 18rem;
                max-height: 18rem;
            }

            .carousel-item {
                font-size: 0.95rem;
            }

        }
    ```

    This developer was able to do this with inspiration from this [StackOverflow](https://stackoverflow.com/questions/29985360/bootstrap-carousel-whole-website-jumps-when-image-is-changing) post.

3. **Jumping behaviour of the image carousel**

    Just like the customer review carousel on the Home page, the image carousel presented a jumping behaviour when
    switching slides. This is because the images are not of equal height.
    
    **How this developer fixed it:**

    Similaryly to the previous bug fix, in order for the carousel to be fully responsive and not present a 'height jump' 
    behaviour on any screen sizes, ```min-height``` and ```max-height``` was set to the ```.carousel-inner``` for the 
    ```@media screen``` that presented this bug.

    For example:

    ```css
        @media screen and (max-width: 320px) {

            .carousel-inner {
                min-height: 18rem;
                max-height: 18rem;
            }

        }
    ```

### Unsolved bugs

1. **Adjust the font size of all the 'Choose service' options**

    Regarding the ```<form>``` for the Booking page and for the modal in the Home page, this developer has not found 
    a solution to adjust the font size of all the 'Choose service' options for smaller screens.

2. **Position of the uncollapsed navbar differs between screen sizes**

    Between ```@media screen and max-width``` of 615px - 1199px, the uncollapsed navbar floats near the center of the 
    page instead of the right-hand side of the page right under the navbar icon. This developer has not found a solution 
    for this.

<div align="center"><h4>Incorrect position of the uncollapsed navbar</h4>
<img src="screenshots/position-navbar.png" alt="Screenshot: Incorrect position of uncollapsed navbar" >
</div>

## Further testing

- Used Chrome DevTools repeatedly throughout the project to test the website on all the different
devices and orientations available in the built-in tool.
- Tested out the website on different computer/laptop screen sizes and also on developer's iPhone 6.
- Asked friends and family to test out the website on their devices to see if there were any 
further issues found.