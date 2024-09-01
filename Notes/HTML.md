## Img Tag

- HTML attributes are special words used inside the opening tag of an element to control the element's behavior.
- The src attribute in an img element specifies the image's URL (where the image is located)
- All img elements should have an alt attribute. The alt attribute's text is used for screen readers to improve accessibility and is displayed if the image fails to load

## Anchor Tag

- To open links in a new tab, you can use the target attribute on the anchor (a) element.

- The target attribute specifies where to open the linked document. target="\_blank" opens the linked document in a new tab or window.

## Section Element

- Before adding any new content, you should make use of a section element to separate the cat photos content from the future content.

- The section element is used to define sections in a document, such as chapters, headers, footers, or any other sections of the document. It is a semantic element that helps with SEO and accessibility.

## Figure element

- The figure element represents self-contained content and will allow you to associate an image with a caption.
- A figure caption (figcaption) element is used to add a caption to describe the image contained within the figure element.

## strong element

- The strong element is used to indicate that some text is of strong importance or urgent.

## Forms

- The form element is used to get information from a user like their name, email, and other details.
- The action attribute indicates where form data should be sent.
- The input element allows you several ways to collect data from a web form. Like img elements, input elements are a void element and do not need closing tags.
- There are many kinds of inputs you can create using the type attribute. You can easily create a password field, reset button, or a control to let users select a file from their computer.
- In order for a form's data to be accessed by the location specified in the action attribute, you must give the text field a name attribute and assign it a value to represent the data being submitted.
- Placeholder text is used to give people a hint about what kind of information to enter into an input
- To prevent a user from submitting your form when required information is missing, you need to add the required attribute to an input element. There's no need to set a value to the required attribute. Instead, just add the word required to the input element, making sure there is space between it and other attributes.
- The button element is used to create a clickable button.The default behavior of clicking a form button without any attributes submits the form to the location specified in the form's action attribute.
- The button you added will submit the form by default. However, relying on default behavior may cause confusion. Add the type attribute with the value submit to the button to make it clear that it is a submit button.
- You can use radio buttons for questions where you want only one answer out of multiple options.
- label elements are used to help associate the text for an input element with the input element itself (especially for assistive technologies like screen readers).
- The id attribute is used to identify specific HTML elements. Each id attribute's value must be unique from all other id values for the entire page.
- Notice that both radio buttons can be selected at the same time. To make it so selecting one radio button automatically deselects the other, both buttons must have a name attribute with the same value.
- The fieldset element is used to group related inputs and labels together in a web form. fieldset elements are block-level elements, meaning that they appear on a new line.
- The legend element acts as a caption for the content in the fieldset element. It gives users context about what they should enter into that part of the form.
- Forms commonly use checkboxes for questions that may have more than one answer. The input element with a type attribute set to checkbox creates a checkbox.
- There's another way to associate an input element's text with the element itself. You can nest the text within a label element and add a for attribute with the same value as the input element's id attribute
- Like radio buttons, form data for selected checkboxes are name / value attribute pairs. While the value attribute is optional, it's best practice to include it with any checkboxes or radio buttons on the page.
- In order to make a checkbox checked or radio button selected by default, you need to add the checked attribute to it.
- The footer element is used to define a footer for a document or section. A footer typically contains information about the author of the document, copyright data, links to terms of use, contact information, and more.
- All page content elements that should be rendered to the page go inside the body element. However, other important information goes inside the head element.
- The head element is used to contain metadata about the document, such as its title, links to stylesheets, and scripts. Metadata is information about the page that isn't displayed directly on the page.
- The title element determines what browsers show in the title bar or tab for the page.
- The html element is the root element of an HTML page and wraps all content on the page.
- We can specify the language of your page by adding the lang attribute to the html element.
- All pages should begin with `<!DOCTYPE html>`. This special string is known as a declaration and ensures the browser tries to meet industry-wide specifications.
- `<!DOCTYPE html>` tells browsers that the document is an HTML5 document which is the latest version of HTML.
- You can set browser behavior by adding meta elements in the head.

## HTML Forms

- The method attribute specifies how to send form-data to the URL specified in the action attribute. The form-data can be sent via a GET request as URL parameters (with method="get") or via a POST request as data in the request body (with method="post").

- Specifying the type attribute of a form element is important for the browser to know what kind of data it should expect. If the type is not specified, the browser will default to text.

- The email type only allows emails with a @ and a . in the domain.
- The password type obscures the input, and warns if the site does not use HTTPS.

- The first input element with a type of submit is automatically set to submit its nearest parent form element.
- To handle the form submission, after the last fieldset element add an input element with the type attribute set to submit and the value attribute set to Submit.

- With type="password" you can use the pattern attribute to define a regular expression that the password must match to be considered valid.
- Add a pattern attribute to the password input element to require the input match: [a-z0-5]{8,}.The above is a regular expression which matches eight or more lowercase letters or the digits 0 to 5.

## Resources

https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg
https://freecatphotoapp.com
