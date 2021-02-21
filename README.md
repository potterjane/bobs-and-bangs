## Table of Contents
1. [**UX**](#ux)
    - [**Project Goals**](#project-goals)
        - [**User Goals**](#user-goals)
        - [**User Stories**](#user-stories)
        - [**Site Owner Goals**](#site-owner-goals)
    - [**Design Choices**](#design-choices)
    - [**Wireframes**](#wireframes)

2. [**Features**](#features)
    - [**Existing Features**](#existing-features)

3. [**Technologies used**](#technologies-used)

4. [**Testing**](#testing)

5. [**Deployment**](#deployment)
    - [**How to run this project locally using a command line**](#how-to-run-this-project-locally-using-a-command-line)

6. [**Credits**](#credits)
    - [**Content**](#content)
    - [**Media**](#media)
    - [**Code**](#code)
    - [**Acknowledgements**](#acknowledgements)

7. [**Disclaimer**](#disclaimer)

## UX

### Project Goals

The primary goal of the Bobs & Bangs website is to provide information about the company, what services they offer and how they can book appointment or contact the company.
The design of the website should also reflect the style of the hair salon: a blended mixture of feminine and masculine traits.
Features include images and videos of the hair salon and the two owners, Tilda (hair stylist) and Mathias (barber and skin care professional), modal button on the front page and a booking page 
to easily book appointments, reviews from customers, social links to provide a different way to learn more about the company and get more peer reviews, and a contact page with various ways to
contact the company.
Bobs & Bangs has three target audiences: New customers, retained customers and potential new employees (hair stylist, barbers or skin care professionals).

#### User Goals

New and retained customer's goals are:
- A website that is not drowning in too much text and images
- Clear and concise list of the services the company offers, with prices
- A page where they can read more about who is behind the company and what they value
- To know what other customers thought about the company's services, already on the Home page
- Images and videos that gives them an insight on what it is like inside the hair salon
- An easy and quick way to book appointments
- To know the hair salon's openings hours so they can know which days they are available
- Easy access to different communication channels to contact the company, including social links
- Address and map that shows where the hair salon is located

Potential new employee's goals are:
- A page where they can read more about who is behind the company and what they value
- Easy accessible contact link for job seekers to send in their resume/CV
- Get a feeling of what customers think of their services and if it lives up to the company's values
- A contact page or section with different communication channels to contact the company
- Address and map that shows where the hair salon is located
- To know the hair salon's opening hours to see if it would fit their work schedule

#### User Stories

As a new customer, I want:
1. To be able to know the background of the company, what other customers think about their services via reviews or social links, so that I can come to a decision on whether or not
to try out their services. 
2. To be able to book an appointment with as little clicks as possible, so that I spend as little of my time of my day booking an appointment.
3. To know if there are any special offers/discounts already on the Home page, so that I know straight away if I should book an appointment now or later.
4. To be able to contact the company in different ways, depending on my personal preference, so that I can contact the company if I have any questions or want to book/rebook/cancel an appointment.
5. To see images/videos of the hair salon, so that I can gain a better insight on what it is like inside the hair salon.

As a retained customer, I want:
1. To be able to book an appointment with as little clicks as possible, so that I spend as little of my time of my day booking an appointment. 
2. To know if there are any new special offers/discounts already on the Home page, so that I know straight away if I should book a new appointment now or later.
3. To be able to have access to their list of services, so that I can see if they have updated their services and if there is anything new I can try out.
4. To be able to contact the company in different ways, depending on my personal preference, so that I can contact the company if I have any questions or want to book/rebook/cancel an appointment.

As a hair stylist/barber looking for a new place of work, I want:
1. To be able to know the background of the company, what other customers think about their services via reviews or social links, so that I can come to a decision on whether or not
to send in my resume/CV.
2. To be able to contact the company in different ways, depending on my personal preference, so that I can contact the company if I have any more questions about them.

#### Site Owner Goals

The couple that owns the hair salon/barbershop wants the website to reach out to new and retained customers but also to potential new employees (hair stylist, barbers and 
skin care professionals) that are interesting in working at the company.

### Design Choices

The overall feel of the website should be one that attracts people from all walks of life, with a blended mixture of feminine and masculine characteristics.

**Structure**

- The header is always fixed on the top of the pages of the website, containing the company logo on the left-hand side and the navigation bar on the right-hand side. 
- From left to right, the navigation bar is in the order of importance: Home page, About page, Services page, Contact page and Booking page.
- The footer is always located at the bottom of the pages on the website, containing company's contact information (visiting address, phone number and e-mail address), opening hours, social links
to Facebook, Instagram, Youtube and LinkedIn. It also contains the developer's disclaimer and LinkedIn page.
- All of the pages can be scrolled vertically and should not be any room to be scrolled horizontally.
- The Home page is the first page that the user lands on when they enter the website. This page acts like an introductory page for user and it should be obvious within seconds on what kind of
website this is. This developer used a hero section on this page, where they placed the background image, company title and slogan, and a modal button and text about special offers
to entice the user to book an appointment now. When user scrolls down further, they will also find a customer review carousel so that the users can immediately get feedback from other 
customers who have used the company's services. Both the hero and the customer review section is aligned at the center of the page. On tablet and mobile screens, the background image is removed
in order to create less clutter on the page.
- The About page is the second page on the navigation bar. Users click here when they want to read more about who is behind the company, what their values are and find an image carousel that
gives users an insight on how it looks inside the hair salon. On larger desktop screens, the image carousel is floating on the right, next to the text. On smaller desktop screens or on larger
tablet screens, thetext wraps around the image carousel. On mobile screens, the image carousel is placed under the text.
- The Services page is the third page on the navigation bar. Users click here when they want to know what services the company offers and to what price. These are listed in a table.
They can also find videos on autoplay (muted and on a loop) which shows the faces behind the people who offering their services. On desktop and tablet screens, the videos are floating on the right, 
next to the tables. On mobile screens, the videos are placed right under each table, respectively.
- The Contact page is the fourth page on the navigation bar. Users click here when they want to see all the different communication channels that the company offers. The following is structured
on desktop and tablet screens: On the top-left, they find the e-mail address for job seekers. On the top-right, they find information om what to do when they want to rebook/cancel an appointment. 
On botton left, they find an embedded Google maps that shows the location of the hair salon. On the bottom-right, they find a contact form as an alternative option to contact the company 
when they have questions. On mobile screens, each of these parts are vertically structured from top-left to bottom-right.
- The Booking page is the fifth and last page on the navigation bar. Users click here when they want to book an appointment. This is an alternative way to book other than the modal button on the
Home page. It is the exact same form as one in the modal button with 7 input fields and one Submit-button. The structure of this form is consistent on all screen sizes.

**Backgrounds**

- The dark charcoal background colour that covers all pages of the website was chosen to represent the masculine feeling of the hair salon but also to make the other elements on the page 
stand out more.
- The background image for the hero section on the Home page was chosen to reflect the rustic aesthetic of the hair salon. The image of the brush, scissors and razors on the wooden table
complements the text in the hero section, "Bobs", "Bangs" and "cut".

**Fonts**

- The primary font called **Major Mono Display** was initially attractive for the developer because of the monospace makes the text for the heading elements clear and readable in any size. 
It was the design of the uppercase typeface that made this font the ultimate choice because it gives room for colour to be added in a stylish way.
- The secondary font called **Roboto** was chosen because it was one of the popular pairings according to [Google Fonts](https://fonts.google.com/specimen/Major+Mono+Display) but also 
because the compact design complements the primary font.

**Colours**

- The two primary colours of light purple (#b288ca) and darker shade of white ('blanchedalmond') were chosen for the company logo, titles, icons, buttons, table borders, heading elements 
and most of the paragraph elements because the light purple colour represents the feminine feeling of the hair salon and the darker shade of white contrast but complements the purple colour well.
- The standard black colour for the text and the light brown ('burlywood') background colour were used for the mark element, which is considered not a permanent element of the website. 
This element is used to inform the user's that the company currently has a discount offer and the colours make the element stand out from the rest of the website. 
It also makes the user's focus drawn straight to the discount offer.

**Icons**

- Icons were used for the social links in the footer element and for the customer reviews in the Home page. They were chosen because they are universally understood and because
their obvious meaning and purpose removes the need for text for explanation.

**Images**

- The images were chosen for the About page to give the users an insight on what it is like inside the hair salon.

**Videos**

- The videos were chosen for the Services page to show the faces of the owners and (currently) the sole employees of the hair salon. The videos also show the owners working with their 
respective customer. The videos complement the tables that lists all of the services that is offered to all customers. 

### Wireframes

These wireframes were created using [Balsamiq](https://balsamiq.com/). The first version of the mobile and desktop mockups was made during the design and planning process for this project. 
The second version of the mobile and desktop mockup was made when the project was almost at the point of completion.

- [First version](https://github.com/potterjane/bobs-and-bangs/blob/29beb82abe6f7bced87dd899abb743d32003d710/wireframes/bb-wireframes-version-1.pdf)
- [Second version]()

## Features
 
### Existing Features

1. **Booking modal**
    - This Bootstrap modal can be found on the Home page. The modal opens only when the user clicks on the "Book Now" button in the hero section.
    - This feature gives users the option to book their appointment immediately from the Home page instead of the Booking page by having them filling out a form.
    - The users can also choose to close the modal by clicking on the modal “backdrop”.

<div align="center"><h4>Booking modal on Home page</h4>
<img src="features/booking-modal.png" alt="Screenshot: Booking modal" >
</div>

2. **Review and image carousel**
    - Bootstrap's carousels were used in two places, one for the customer reviews in the Home page and on for the images in the About page. 
    - It gives the website a sense of movement and removes the hassle of scrolling through several images and reviews, manually.
    - This feature allows users to control the transition duration by holding down on the review/image. 

<div align="center"><h4>Customer review carousel on Home page</h4>
<img src="features/review-carousel.png" alt="Screenshot: Review carousel" >
</div>

<div align="center"><h4>Image carousel on About page</h4>
<img src="features/images-carousel.png" alt="Screenshot: Image carousel" >
</div>

3. **Navigation bar for desktop and mobile**
    - Standard navigation bar is used for desktop screens, aligned on the top-right side of all the pages.
    - Bootstrap's 'hamburger' navbar is used to collapse the navigation content for mobile and tablet screens. This is to remove any unneccesarry clutter for the users.
    - This feature allows users to easily navigate through each part of the website with minumum number of clicks.

<div align="center"><h4>Desktop navbar</h4>
<img src="features/desktop-navbar.png" alt="Screenshot: Navbar for desktop screens" >
</div>

<div align="center"><h4>Mobile and tablet navbar</h4>
<img src="features/mobile-navbar.png" alt="Screenshot: Navbar for mobile and tablet screens" >
</div>

4. **Links in the footer**
    - Target blank links to all the external social websites and contact information is found here.
    - This feature allows users to contact the company or to find more about the company with just one click, no matter which page the users are currently on.

<div align="center"><h4>Desktop footer</h4>
<img src="features/footer-desktop.png" alt="Screenshot: Footer on desktop" >
</div>

## Technologies Used

**This project used:**
- HTML and CSS programming languages. 
- [Bootstrap](https://getbootstrap.com/docs/5.0/getting-started/introduction/)'s CSS and Javascript library, version 5.0.
- [Google Fonts](https://fonts.google.com/) to style the website's fonts.
- [Font Awesome](https://fontawesome.com/)'s free kit of icons.
- [Pexels](https://www.pexels.com/) for free stock photos & videos.
- [GitHub](https://github.com/) to store and share all project codes.
- [GitPod](https://www.gitpod.io/) for their IDE (integrated development environment) while building the website.

## Testing 

This information can be found in separate [testing.md](testing.md) file

## Deployment

This project was created and developed using the [GitPod IDE](https://www.gitpod.io/), and then added, committed and pushed to [GitHub](https://github.com/) to store and share all project codes.

The followings steps were taken by the developer in order to deploy Bobs & Bangs to GitHub Pages:
1. Log into GitHub
2. Choose from the list the repositories, [bobs-and-bangs](https://github.com/potterjane/bobs-and-bangs)
3. Select 'Settings' from this repository's menu bar.
4. Scroll down to the 'GitHub Pages' section.
5. Under 'Source' and from the drop-down menu labelled 'None', select the 'master' branch and then click 'Save'.
6. When the page is refreshed, scroll back down to the 'GitHub Pages' section to retrieve the link to the [deployed website](https://potterjane.github.io/bobs-and-bangs/). 

### How to run this project locally using a command line

The project can be run locally by cloning the repository from GitHub. Below are the steps that the developer took to clone this project using HTTPS and the command line. 
Read this [GitHub document](https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository) to find other ways to run this project locally.

1. Log into GitHub
2. Choose from the list the repositories, [bobs-and-bangs](https://github.com/potterjane/bobs-and-bangs)
3. From the drop-down menu labelled 'Code', select the HTTPS section and then click on the icon to copy the URL of the repository.
4. Open the local terminal.
5. Change the current working directory to the location where the cloned directory is to be stored.
6. When directory has been changed and location is selected, type ```git clone``` and then paste the URL of the repository that was copied in step 3.
```console
git clone https://github.com/potterjane/bobs-and-bangs.git
```
7. Press 'Enter'.

## Credits

### Content

- All text in this project was written by the developer.

### Media

#### Images
- The images were sourced from user [cottonbro](https://www.pexels.com/@cottonbro)'s [Pexels](https://www.pexels.com/) free library.

#### Videos
- The videos were sourced from user [cottonbro](https://www.pexels.com/@cottonbro)'s [Pexels](https://www.pexels.com/) free library.

### Code
- Bootstrap's [grid system](https://getbootstrap.com/docs/5.0/layout/grid/), [containers](https://getbootstrap.com/docs/5.0/layout/containers/), 
[custom button styles](https://getbootstrap.com/docs/5.0/components/buttons/), [tables](https://getbootstrap.com/docs/5.0/content/tables/) 
and [forms](https://getbootstrap.com/docs/5.0/forms/overview/) were used.
- 'Hamburger' or collapsed navbar was taken from [Bootstrap](https://getbootstrap.com/docs/5.0/components/navbar/).
- The carousel for the images and the customer reviews was taken from [Bootstrap](https://getbootstrap.com/docs/5.0/components/carousel/).
- Modal code taken from [Bootstrap](https://getbootstrap.com/docs/5.0/components/modal/).
- Code for date control was taken from this [W3Schools](https://www.w3schools.com/tags/att_input_type_date.asp) post.
- Code on how to make the textarea act responsive was taken from this 
[StackOverflow](https://stackoverflow.com/questions/39068128/how-can-i-make-a-textarea-that-fits-within-the-width-of-the-current-viewport/39068155) post.
- Code on how to wrap text around an image is taken from this [GeeksforGeeks](https://www.geeksforgeeks.org/how-to-wrap-the-text-around-an-image-using-html-and-css/) post.
- Code on how to embedd Google Maps was found in one of Code Institute's HTML module about [iframe](https://learn.codeinstitute.net/courses/course-v1:CodeInstitute+HE101+2020/courseware/fcc67a894619420399970ae84fc4802f/13db720675f94dbca6b0fe79467628ca/).
- Code on how to disable the horizontal scroll on all pages was taken from this [StackOverflow](https://stackoverflow.com/questions/17756649/disable-the-horizontal-scroll) post.
- Code on how to center an image was taken from this[W3Schools](https://www.w3schools.com/howto/howto_css_image_center.asp) post.

### Acknowledgements

Special thanks to: 
- Code Institute Mentor Mo for his time and for always offering his support and suggestions on what this developer needs to focus on in order to complete the project.
- Boyfriend Fredrik, friends Alex and Emelie and sisters Marie and Erin for testing the website and giving this developer positive and constructive feedback.

#### Disclaimer
The content of this website, including the images and videos used, are for educational purposes only.