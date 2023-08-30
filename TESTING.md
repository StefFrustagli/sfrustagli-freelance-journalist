# Stefania Frustagli, Freelance Journalist Portfolio - Testing details

[Main README.md file](/README.md) <br>
[View the website in GitHub Pages](https://github.com/StefFrustagli/sfrustagli-freelance-journalist.git)


## Validator Testing
### HTML

The [W3C validator](https://validator.w3.org/nu/?doc=https%3A%2F%2Fcode-institute-org.github.io%2Flove-running-2.0%2Findex.html) returned an error, some warnings and info messages that were promptly corrected.

- Error:

![Error message: Element div not allowed as child of element h1 in this context.](https://i.ibb.co/YTKjN3t/Screenshot-2023-08-29-at-19-28-35.png)

How it was fixed: I replaced div with span.

- Warnings:

![Warning: Section lacks heading](https://i.ibb.co/nBj9CYS/Screenshot-2023-08-29-at-19-30-20.png)


![Warning: Section lacks heading](https://i.ibb.co/vkPqgq4/Screenshot-2023-08-29-at-19-29-59.png)

How it was fixed: I added hidden headings.

![Warning: Consider using the h1 element as a top-level heading only](https://i.ibb.co/KbyJsZy/Screenshot-2023-08-29-at-19-45-12.png)

How it was fixed: I replaced h1 with h2.

- Info:

![Info message: Trailling slash on void element has no effect and interract badly with unquoted attribute values](https://i.ibb.co/8xc0PGD/Screenshot-2023-08-29-at-19-29-10.png)

As the trailing slashes were automatically generated when formatting the document, these messages were ignored.

After the fix, the result was as follows:

![Document checking completed. No errors or warnings to show.](https://i.ibb.co/hddrgq4/Screenshot-2023-08-29-at-20-38-56.png "Document checking completed")


### CSS

No errors were found when passing through the official [(Jigsaw) validator](https://jigsaw.w3.org/css-validator/validator?uri=https%3A%2F%2Fvalidator.w3.org%2Fnu%2F%3Fdoc%3Dhttps%253A%252F%252Fcode-institute-org.github.io%252Flove-running-2.0%252Findex.html&profile=css3svg&usermedium=all&warning=1&vextwarning=&lang=en#css).


## Manual testing

#### Logo 
The logo allows you to return to the homepage when clicked, and it works on all pages.

#### Navbar
On tablets and larger screens, the navbar shows an 'About' and 'Contact' menu on all pages. It was tested and both links worked correctly.

Mobile devices can access the "About" and "Contact" pages using the Burger Bar instead. It was tested and worked correctly.

On desktops and larger screens, hovering over a navbar element should underline and colour the text. It was tested and worked correctly.

#### Footer

In the footer, social media profiles are accessible by clicking on the icons. All HTML pages have the same footer code. They have been tested and work.

#### Hero image

The hero image behaves as expected on all device widths.

Homepage page with selected writings
External links in all articles work properly. When a link is clicked, a new tab is opened.

#### About page

I have verified that the round image and the text look right on all devices by reducing and expanding the window width.

#### Contact page

**Form**

If all fields are filled out, the form works. It is addressed to Code Institute: <https://formdump.codeinstitute.net/> <br>
When the form has been submitted correctly, a "Congratulations" message appears.

If we fail to fill out the Full name or Email address fields, a "Fill out this field" or "Enter an email address" message appears. The 'Leave a message here' field was not required, so I added a required attribute to the textarea as well. I've tested it and it works as expected.
