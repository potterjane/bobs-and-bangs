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

    **How I fixed it:**

    With the help of the [SimplySmartMedia](https://simplysmartmedia.com/2016/06/heres-why-your-bootstrap-collapsed-alert-jumps-when-expanded/)'s post, 
    I moved the ```class="nav-container-collapse"``` from the ```<ul>``` element to the grandparent ```<div>``` element.

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



### Unsolved bugs

## Further testing

- Asked friends and family to test out the website on their devices to see if there were any further issues found.