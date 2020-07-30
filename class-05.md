
# Images:

- There are many reasons why you might want to add an image to a web page: you might want to include a logo, photograph, illustration, diagram, or chart.

- **Images should**...
1. Be relevant
2. Convey information
3. Convey the right mood
4. Be instantly recognisable
5. Fit the color palette

- If you are building a site from scratch, it is good practice to create a folder for all of the images the site uses.all of the images are stored in a folder called **images**.

- **Adding Images**

- To add an image into the page you need to use an ```<img>`` lement. This is an empty element (which means there is no closing tag). It must carry the following two attributes:

1. **src**: This tells the browser where it can find the image file. This will usually be a relative URL pointing to an image on your own site.

2. **alt**: This provides a text description of the image which describes the image if you cannot see it.

- **title**:  You can also use the title ttribute with the ```<img>``` element to provide additional information about the image.

- You will also often see an ```<img>``` element use two other attributes that specify its size:

1. **height**: This specifies the height of the image in pixels.
2. **width**: This specifies the width of the image in pixels.

- **Where to Place Images in Your Code**

1. before a paragraph The paragraph starts on a new line after the image.

- EX: ```<img src="image" alt="image-name" width="100" height="100/>```
```<p> your paragraph...  </p>```

2. inside the start of a paragraph The first row of text aligns with the bottom of the image.

- Ex: ```<p><img src="image" alt="image-name" width="100" height="100/> and then your paragraph...</p>```

3. in the middle of a paragraph The image is placed between the words of the paragraph that it appears in.

- Ex: ```<p>your paragraph and then.... <img src="image" alt="image-name" width="100" height="100/> and then your paragraph...</p></p>```

- **Three Rules for Creating Images**:

1. **Save images**: in the right format Websites mainly use images in jpeg, gif, or png format.

2. **Save images at the right size**: You should save the image at the same width and height it will appear on the website. If the image is smaller than the width or height that you have specified.

3. **Use the correct resolution**: Computer screens are made up of dots known as pixels. Images used on the web are also made up of tiny dots. Resolution refers to the number of dots per inch, and most computer screens only show web pages at 72 pixels per inch.

# Color:can really bring your pages to life.

- The color property allows you to specify the color of text inside an element. You can specify any color in CSS in one of three ways:

1. **rgb values**: These express colors in terms of how much red, green and blue are used to make it up. For example: rgb(100,100,90)
- ```p {```
```color: rgb(100,100,90);}```

2. **hex codes**: These are six-digit codes that represent the amount of red, green and blue in a color, preceded by a pound or hash # sign. For example: #ee3e80
- ```h2 {```
```color: #ee3e80;}``` 

3. **color names**:There are 147 predefined colornames that are recognized by browsers. For example:DarkCyan
- ```h1 {```
```color: DarkCyan;}```

- **background-color**: CSS treats each HTML element as if it appears in a box, and the background-color property sets the color of the background for that box.

**Understanding Color**:Every color on a computer screen is created by mixing amounts of red,green, and blue. To find the color you want, you can use a color picker.

- **opacity, rgba**:CSS3 introduces the opacity property which allows you to specify the opacity of an element and any of its child elements. The value is a number between 0.0 and 1.0 (so a value of 0.5 is 50% opacity and 0.15 is 15% opacity).

- Ex: ```p.two {```
```background-color: rgb(0,0,0);```
```background-color: rgba(0,0,0,0.5);}```

- **hsl, hsla**:The hsl color property has been introduced in CSS3 as an alternative way to specify colors. The value of the property starts with the letters hsl, followed by individual values inside parentheses for:

- Ex: ```p {```
```background-color: #ffffff;```
```background-color: hsla(0,100%,100%,0.5);}```
- **hue**:This is expressed as an angle (between 0 and 360 degrees).

- **saturation**: This is expressed as a percentage.

- **lightness**: This is expressed as a percentage with 0% being white, 50% being normal, and 100% being black.

- **alpha**: This is expressed as a number between 0 and 1.0. For example, 0.5 represents 50% transparency, and 0.75 represents 75% transparency.

# Text

- The properties that allow you to control the appearance of text can be split into two groups:

1. hose that directly affect t ●● he font and its appearance (including the typeface, whether it is regular, bold or italic, and the size of the text)

2. Those that would have the same effect on text no matter what font you were using (including the color of text and the spacing between words and letters)

- **The font-family property**:allows you to specify the typeface that should be used for any text inside the element(s) to which a CSS rule applies. The value of this property is the name of the typeface you want to use.

- Ex:```h1 {```
```font-family: "Courier New", Courier,monospace;}```

- **font-size property**: enables you to specify a size for the font. There are several ways to specify the size of a font. The most common are:
1. **pixels**:are commonly used because they allow web designers very precise control over how much space their text takes up. The number of pixels is followed by the letters px.

2. **percentages**:The default size of text in browsers is 16px. So a size of 75% would be the equivalent of 12px, and 200% would be 32px.

- Ex:```h1 {font-size: 200%;}```
```h2 {font-size: 1.3em;}```

- **The font-weight property**: allows you to create bold text. There are two values that this property commonly takes:(normal and bold)```h1 {font-weight: bold;}```

- **font-style**:it can be normal, italic and oblique.
- Ex:```h1 {font-style: italic;}```

- **The text-transform property**:is used to change the case of text giving it one of the following values:it can be uppercase,lowercase and capitalize(first latter of each word to appear capitalized)
- Ex:```h1 {text-transform: uppercase;}```

- **letter-spacing, word-spacing**:
- Ex:```h1 {font-weight: bold;```
```word-spacing: 1em;```
```letter-spacing: 0.2em;}```

- **The text-align property**; allows you to control the alignment of text. The property can take one of four values:left, right, center and justify(This indicates that every line in a paragraph, except the last line, should be set to take up the full width of the containing box.).

- Ex:```p {text-align: justify;}```

- **text-shadow**:It is used to create a drop shadow, which is a dark version of the word just behind it and slightly offset.
- Ex:```p {background-color: #eeeeee;```
```text-shadow: 1px 1px 0px #000000;}```

- **first-letter, :first-line**:You can specify different values for the first letter or first line of text inside an element using.

- Ex:```p:first-line {font-weight: bold;}

- **link, :visited**:Browsers tend to show links in blue with an underline by default,but we can changes

- **link**:This allows you to set styles for links that have not yet been visited.```a:link {color: deeppink;}```

- **visited**:This allows you to set styles for links that have been clicked on.```a:visited {color: black;}```
