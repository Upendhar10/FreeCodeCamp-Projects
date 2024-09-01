- CSS is the language used to style an HTML document. It describes how HTML elements should be displayed on the screen.
- Internal styling
- You can add style to an element by specifying it in the style element and setting a property for it like this:
  ```
  element {
  property: value;
  }
  ```
- For the styling of the page to look similar on mobile as it does on a desktop or laptop, you need to add a meta element with a special content attribute.
- You can use the id selector to target a specific element with an id attribute. An id selector is defined by placing the hash symbol # directly in front of the element's id value.
- A class selector is defined by a name with a dot directly in front of it, like this:
  ```
  .class-name {
  styles
  }
  ```
- inline-block elements only take up the width of their content
- The default color of a link that has not yet been clicked on is typically blue.
- The default color of a link that has already been visited from a page is typically purple.
- You change properties of a link when the link has actually been visited by using a pseudo-selector that looks like a:visited { propertyName: propertyValue; }.

## Colors

- The HSL color model, or hue, saturation, and lightness, is another way to represent colors.

- The CSS hsl function accepts 3 values: a number from 0 to 360 for hue, a percentage from 0 to 100 for saturation, and a percentage from 0 to 100 for lightness.

- If you imagine a color wheel, the hue red is at 0 degrees, green is at 120 degrees, and blue is at 240 degrees.

- Saturation is the intensity of a color from 0%, or gray, to 100% for pure color. You must add the percent sign % to the saturation and lightness values.

- Lightness is how bright a color appears, from 0%, or complete black, to 100%, complete white, with 50% being neutral.

- A gradient is when one color transitions into another. The CSS linear-gradient function lets you control the direction of the transition along a line, and which colors are used.

- One thing to remember is that the linear-gradient function actually creates an image element, and is usually paired with the background property which can accept an image as a value.

- The linear-gradient function is very flexible -- here is the basic syntax you'll use in this tutorial:
  ```
  linear-gradient(gradientDirection, color1, color2, ...);
  ```
- **gradientDirection** is the direction of the line used for the transition. **color1** and **color2** are color arguments, which are the colors that will be used in the transition itself. These can be any type of color, including color keywords, hex, rgb, or hsl.

- Color-stops allow you to fine-tune where colors are placed along the gradient line. They are a length unit like px or percentages that follow a color in the linear-gradient function.

- If no gradientDirection argument is provided to the linear-gradient function, it arranges colors from top to bottom, or along a 180 degree line, by default.

- Opacity describes how opaque, or non-transparent, something is. For example, a solid wall is opaque, and no light can pass through. But a drinking glass is much more transparent, and you can see through the glass to the other side.

- With the CSS opacity property, you can control how opaque or transparent an element is. With the value 0, or 0%, the element will be completely transparent, and at 1.0, or 100%, the element will be completely opaque like it is by default.

- The rgba function works just like the rgb function, but takes one more number from 0 to 1.0 for the alpha channel:
  ```
  rgba(redValue, greenValue, blueValue, alphaValue);
  ```
- The box-shadow property lets you apply one or more shadows around an element. Here is basic syntax:

  ```
  box-shadow: offsetX offsetY blurRadius color;
  ```

  - Here's how the offsetX and offsetY values work:
    - both offsetX and offsetY accept number values in px and other CSS units
    - a positive offsetX value moves the shadow right and a negative value moves it left
    - a positive offsetY value moves the shadow down and a negative value moves it up
    - if you want a value of zero (0) for any or both offsetX and offsetY, you don't need to add a unit. Every browser understands that zero means no change.
    - The height and width of the shadow is determined by the height and width of the element it's applied to.
    - You can also use an optional spreadRadius value to spread out the reach of the shadow. More on that later.
  - If a blurRadius value isn't included, it defaults to 0 and produces sharp edges. The higher the value of blurRadius, the greater the blurring effect is.

- The rem unit stands for root em, and is relative to the font size of the html element.

As label elements are inline by default, they are all displayed side by side on the same line, making their text hard to read.

## Box Model

- Margin is the area outside of the box, and can be used to control the space between other boxes or elements.

- The border-radius property accepts up to four values to round the top-left, top-right, bottom-right, and bottom-left corners.

- The box-sizing property is used to set this behavior. By default, the content-box model is used. With this model, when an element has a specific width, that width is calculated based only on the element's content. Padding and border values get added to the total width, so the element grows to accommodate these values.

## Flex-box

- Flexbox has a main and cross axis.
- The main axis is defined by the flex-direction property, which has four possible values:

  - row (default): horizontal axis with flex items from left to right
  - row-reverse: horizontal axis with flex items from right to left
  - column: vertical axis with flex items from top to bottom
  - column-reverse: vertical axis with flex items from bottom to top
  - Note: The axes and directions will be different depending on the text direction. The values shown are for a left-to-right text direction.

- The flex-wrap property determines how your flex items behave when the flex container is too small.
- Setting it to wrap will allow the items to wrap to the next row or column.
- nowrap (default) will prevent your items from wrapping and shrink them if needed.

- The justify-content property determines how the items inside a flex container are positioned along the main axis, affecting their position and the space around them.

- The align-items property positions the flex content along the cross axis. In this case, with your flex-direction set to row, your cross axis would be vertical.

- The gap CSS shorthand property sets the gaps, also known as gutters, between rows and columns.
- The gap property and its row-gap and column-gap sub-properties provide this functionality for flex, grid, and multi-column layout. You apply the property to the container element.

- The :not pseudo-selector can be used to select all elements that do not match the given CSS rule.
  ```
  div:not(#example) {
  color: red;
  }
  ```

## Accessibility

- `lang` attribute to your html element. This will assist screen readers in identifying the language of the page.
- The `charset` attribute specifies the character encoding of the page, and, nowadays, UTF-8 is the only encoding supported by most browsers.
- `head`, the `title` element is useful for screen readers to understand the content of a page. Furthermore, it is an important part of SEO.

- Navigation is a core part of accessibility, and screen readers rely on you to provide the structure of your page. This is accomplished with semantic HTML elements.
- The `header` element will be used to introduce the page, as well as provide a navigation menu.
- The `main` element will contain the core content of your page.

- To increase the page accessibility, the role attribute can be used to indicate the purpose behind an element on the page to assistive technologies. 
- The role attribute is a part of the Web Accessibility Initiative (WAI), and accepts preset values.
- Every region role requires a label, which helps screen reader users understand the purpose of the region. 
- One method for adding a label is to add a heading element inside the region and then reference it with the aria-labelledby attribute.

- Typeface plays an important role in the accessibility of a page. Some fonts are easier to read than others, and this is especially true on low-resolution screens.

- Placeholder is actually not a best-practice for accessibility; too often, users confuse the placeholder text with an actual input value - they think there is already a value in the input.

- The footer element is a container for a collection of content that is related to the page. 
- the address element is a container for contact information for the author of the page.

- On the topic of visual accessibility, contrast between elements is a key factor. For example, the contrast between the text and the background of a heading should be at least 4.5:1.