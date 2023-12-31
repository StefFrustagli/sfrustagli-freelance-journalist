# Stefania Frustagli, Freelance Journalist Portfolio - Testing details

[Main README.md file](README.md) <br>
[View the website in GitHub Pages](https://github.com/StefFrustagli/sfrustagli-freelance-journalist.git)


## Validator Testing
### HTML

The [W3C validator](https://validator.w3.org/nu/?doc=https%3A%2F%2Fcode-institute-org.github.io%2Flove-running-2.0%2Findex.html) returned an error, some warnings and info messages that were promptly corrected.

- Error:

![Error message: Element div not allowed as child of element h1 in this context.](https://i.ibb.co/YTKjN3t/Screenshot-2023-08-29-at-19-28-35.png)

**How it was fixed**: I replaced `div` with `span`.

- Warnings:

![Warning: Section lacks heading](https://i.ibb.co/nBj9CYS/Screenshot-2023-08-29-at-19-30-20.png)


![Warning: Section lacks heading](https://i.ibb.co/vkPqgq4/Screenshot-2023-08-29-at-19-29-59.png)

**How it was fixed**: I added hidden headings.

![Warning: Consider using the h1 element as a top-level heading only](https://i.ibb.co/KbyJsZy/Screenshot-2023-08-29-at-19-45-12.png)

**How it was fixed**: I replaced h1 with h2.

- Info:

![Info message: Trailling slash on void element has no effect and interract badly with unquoted attribute values](https://i.ibb.co/8xc0PGD/Screenshot-2023-08-29-at-19-29-10.png)

As the trailing slashes were automatically generated when formatting the document, these messages were ignored.

After the fix, the result was as follows:

![Document checking completed. No errors or warnings to show.](https://i.ibb.co/hddrgq4/Screenshot-2023-08-29-at-20-38-56.png "Document checking completed")


### CSS

No errors were found when passing through the official [(Jigsaw) validator](https://jigsaw.w3.org/css-validator/validator.html.en).


## Manual testing

| To be tested | Test Action                                                                                                           | Expected Outcome                                                                                                                                          | Test Outcome |
|--------------|-----------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------|--------------|
| Logo         | Navigate to the header and click on the logo "Stefania Frustagli".                                                    | When clicked on the About and Contact pages, the logo should take you back to the homepage.                                                               | Pass         |
| Navbar       | Navigate to the 'burger icon' ≡ (on devices) or 'Contact' and 'About' (on larger screens) in the header on the right. | All pages should have an 'About' and 'Contact' menu.                                                                                                      | Pass         |
|              |                                                                                                                       | It should be possible to access the following pages through the navbar: About and Contact.                                                                | Pass         |
|              |                                                                                                                       | The text should be underlined and colored when hovered over in the navbar on desktops and larger screens.                                                 | Pass         |
| Footer       | Navigate to the footer at the bottom of the page.                                                                     | A footer with three social media icons should appear on all pages.                                                                                        | Pass         |
|              |                                                                                                                       | By clicking on the icons, you should be able to access social media profiles in a new tab.                                                                | Pass         |
| Hero image   | Navigate to the homepage. The hero image is located below the logo.                                                   | On all devices, it should be visible and responsive.                                                                                                      | Pass         |
| Homepage     | Navigate to the homepage. A section called 'Selected writings' appears beneath the Hero image.                        | There is a link at the end of each article's preview that should lead to the full article on another website. It should be opened in a new tab.           | Pass         |
| About page   | Navigate to the About page by clicking on the navbar menu.                                                            | The round image and the text should look responsive on all devices.                                                                                       | Pass         |
| Contact page | Navigate to the Contact page by clicking on the navbar menu.                                                          | The text and form should look responsive on all devices.                                                                                                  | Pass         |
| Form         | Navigate to the Contact page by clicking on the navbar menu.                                                          | The form should work if all fields are filled out.                                                                                                        | Pass         |
|              |                                                                                                                       | A "Congratulations" message should appear after submitting the form correctly.  It is addressed to Code Institute: <https://formdump.codeinstitute.net/>  | Pass         |
|              |                                                                                                                       | A "Fill out this field" message should appear if we fail to fill out the Full name field and submit the form.                                             | Pass         |
|              |                                                                                                                       | An "Enter an email address" message should appear if we fail to fill out the Email address field and submit the form.                                     | Pass         |
|              |                                                                                                                       | A 'Leave a message here' field should appear if we fail to fill out the Message field and submit the form.                                                | Pass         |


## Browser Compatibility

Below are the browsers that have been tested:

- Chrome Version 116.0.5845.140
- Firefox Version 117.0
- Safari Version 16.6

## Responsiveness
I tested the website on a variety of screen sizes from iPhone 5 (320px wide) to a 5K iMac Pro (5120 x 2880 px) and it appears to be responsive on all of them.

## Lighthouse test

I performed this test using Chrome Dev tools in an incognito window (as Chrome extensions negatively affected the page's load performance).

The result, with a mobile setup, was the following:
- Performance: 88
- Accessibility: 96
- Best practises: 100
- SEO: 100
  
Since the hero image is already in a *webp* format, I've decided not to make any further changes for the time being.

![Test result: 88 Performance, 96 Accessibility, 100 Best Practices, 100 SEO](https://i.ibb.co/XLMpCgN/Screenshot-2023-08-30-at-19-48-52.png)

The result, with a desktop setup, was the following:
- Performance: 99
- Accessibility: 96
- Best practises: 100
- SEO: 100
  
![Test result: 99 Performance, 96 Accessibility, 100 Best Practices, 100 SEO](https://i.ibb.co/T1B6sCz/Screenshot-2023-08-30-at-19-45-38.png)

## Bugs resolved

As far as I could tell, there weren't any significant bugs. The minor changes I've made were intended to improve the website's aesthetics, readability and responsiveness. For examples:
- I've decided to add a media query for small devices to improve the hero image's output on mobile phones.
- Thanks to my mentor's guidance, I was able to make the website responsive on a 5k screen (e.g. 5K iMac Pro):
     - I gave the `body` a `max-width: 2000px` and center it in the document using the `margin-left` and `margin-right` to auto. 
     - I gave the `header` and  `left:0`, `top:0` and `width:100%`;
     - I created a contained inside `header` and moved everything inside that container;
     - To make the hero image go edge to edge, I moved it to its own `div` called `hero` inside the section.
     - I gave the section the same background color as the `header`, set `postition:absolute`, `left:0`, `top` as the height of the header and `width:100%`;
     - I set `postition:relative` on `<html>`.
  
## Future improvements
- Performance on mobile devices is something I would like to improve going forward.
  