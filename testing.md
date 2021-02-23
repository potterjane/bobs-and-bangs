# Bobs & Bangs - Testing details

[Main README.md file](README.md)

[View website in GitHub Pages](https://potterjane.github.io/bobs-and-bangs/)

## Table of Contents

1. [**Validation services**](#validation-services)
2. [**User Stories Testing**](#user-stories-testing)
3. [**Manual Testing**](#manual-testing)
    - [**Testing on desktop screens**](#testing-on-desktop-screens)
    - [**Testing on tablet and phone screens**](#testing-on-tablet-and-phone-screens)
4. [**Bugs discovered**](#bugs-discovered)
    - [**Solved bugs**](#solved-bugs)
    - [**Unsolved bugs**](#unsolved-bugs)
5. [**Further Testing**](#further-testing)

## Validation services
The following validation services were used to check the validity of the website code.
- [W3C Markup Validation]( https://validator.w3.org/) was used to validate HTML.
- [W3C CSS validation](https://jigsaw.w3.org/css-validator/) was used to validate CSS.

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

### Unsolved bugs

## Further testing

- This developer asked friends and family to test out the website on their devices to see if there were any 
further issues found.