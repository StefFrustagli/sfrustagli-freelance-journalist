# TESTING

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

  - No errors were found when passing through the official [(Jigsaw) validator](https://jigsaw.w3.org/css-validator/validator?uri=https%3A%2F%2Fvalidator.w3.org%2Fnu%2F%3Fdoc%3Dhttps%253A%252F%252Fcode-institute-org.github.io%252Flove-running-2.0%252Findex.html&profile=css3svg&usermedium=all&warning=1&vextwarning=&lang=en#css).


