
# Images

- Controlling the size and alignment of your images using CSS keeps rules that affect the presentation of your page in the CSS and out of the HTML markup.

- You can control the size of an image using the width and height properties in CSS, just like you can for any other box.

- Ex: ```img.large {```
```width: 500px;```
```height: 500px;}```

- then you might have a selection of image sizes that are commonly used on all pages, such as:

- Small portrait: 220 x 360
- Small landscape: 330 x 210
- Feature photo: 620 x 400

- **AligNi ng images Using CSS**:using the <img> element's align attribute, web page authors are increasingly using the float property to align images. There are two ways that this is commonly achieved:

1. The float property is added to the class that was created to represent the size of the image (such as the small class in our example).

2. New classes are created with names such as align-left or align-right to align the images to the left or right of the page.These class names are used in addition to classes that indicate the size of the image.

- Ex: ```<p><img src="images/magnolia-medium.jpg"```
```alt="Magnolia" class="align-left medium" />```

- ```img.align-left {```
```float: left;```
```margin-right: 10px;}```

- **Centering images Using CSS**:By default, images are inline elements. This means that they flow within the surrounding text. In order to center an image, it should be turned into a blocklevel element using the display property with a value of block.

- there are two common ways in which you can horizontally center an image:
1. On the containing element, you can use the text-align property with a value of center.

2. On the image itself, you can use the use the margin property and set the values of the left and right margins to auto.

- **Background Images**:The background-image property allows you to place an image behind any HTML element. This could be the entire page or just part of the page. By default, a background image wil  repeat to fill the entire box.The path to the image follows the letters url, and it is put inside parentheses and quotes.

- Ex 1:you can see a background image being applied to an entire page (because the CSS selector applies to the ```<body> element).  body {```
 ```background-image: url("images/pattern.gif");}```

- Ex 2: the background image just applies to a paragraph.
```p {background-image: url("images/pattern.gif");}```

- The background-repeat property can have four values:

- **repeat**:The background image is repeated both horizontally and vertically (the default way it is shown if the backgroundrepeat property isn't used).

- **repeat-x**: The image is repeated horizontally only (as shown in the first example on the left).

- **repeat-y**: The image is repeated vertically only.

- **no-repeat**:The image is only shown once. The background-attachment property specifies whether a background image should stay in one position or move as the user scrolls up and down the page. It can have one of two values:

1. **fixed**: The background image stays in the same position on the page.

2. **scroll**: The background image moves up and down as the user scrolls up and down the page.

- Ex:```body {background-image: url("images/tulip.gif");``
```background-repeat: no-repeat;```
```background-attachment: fixed;} ```

- When an image is not being repeated, you can use the background-position property to specify where in the browser window the background image should be placed. This property usually has a pairof values. The first represents the horizontal position and the second represents the vertical.

- left top
- left center
- left bottom
- center top
- center center
- center bottom
- right top
- right center
- right bottom

- The background property acts like a shorthand 
- The properties must be specified in the following order, but you can miss any value if you do not want to specify it.
1. background-color
2. background-image
3. background-repeat
4. background-attachment
5. background-position

# Practical Information

- **Search Engine Optimization (SEO)**: is a huge topic and several books have been written on the subject. The following pages will help you understand the key concepts so you can improve your website's visibility on search engines.

- **The Basics**:Search engine optimization (or SEO) is the practice of trying to help your site appear nearer the top of search engine results when people look for the topics that your website covers.

- **On-Page Techniques**:On-page techniques are the methods you can use on your web pages to improve their rating in search engines.

- **Off-Page Techniques**:Getting other sites to link to you is just as important as on-page techniques. Search engines help determine how to rank your site by looking at the number of other sites that link to yours.

- **On-Page SEO**:In every page of your website there are seven key places where keywords (the words people might search on to find your site) can appear in order to improve its findability.

1. **Page Title**:The page title appears at the top of the browser window or on the tab of a browser. It is specified in the <title> element which lives inside the <head> element.

2. **URL / Web Address**:The name of the file is part of
the URL. Where possible, use keywords in the file name.

3. **Headings**:If the keywords are in a heading <hn> element then a search engine will know that this page is all about that subject and give it greater weight than other text.

4. **Text**:Where possible, it helps to repeat the keywords in the main body of the text at least 2-3 times.

5. **Link Text**:Use keywords in the text that create links between pages (rather than using generic expressions such as "click here").

6. **Image Alt Text**:Search engines rely on you providing accurate descriptions of images in the alt text.

7. **Page Descriptions**:The description also lives inside the <head> element and is specified using a <meta> tag.
It should be a sentence that describes the content of the
page. (These are not shown in the browser window but they
may be displayed in the results pages of search engines.)

- **How to Identify Keywords and Phrases**:Determining which keywords to use on your site can be one of the
hardest tasks when you start to think about SEO. Here are six steps that will help you identify the right keywords and phrases for your site.

1. **Brainstorm**:List down the words that someone might type into Google to find your site.

2. **Organize**:Group the keywords intoseparate lists for the differentsections or categories of your website.

3. **Research**:There are several tools that let
you enter your keywords and then they will suggest additional keywords.

4. **Compare**:It is very unlikely that your site will appear at the top of the search results for every keyword. This is especially true for topics where there is a lot of competition.

5. **Refine**:Now you need to pick which keywords you will focus on. These should always be the ones that are most relevant to each section of your site.

6. **Map**:Now that you have a refined list of keywords, you know which have the most competition, and which ones are most relevant, it is time to start picking which keywords you will use for each page.

### Analytics: 

- **Learning about your Visitors**:As soon as people start coming to your site, you can start analyzing
how they found it, what they were looking at and at what point they are leaving. One of the best tools for doing this is a free service offered by Google called Google Analytics.
1. **Signing Up**The Google Analytics service
relies on you signing up for an account.
2. **How it Works**:Every time someone loads a page of your site, the tracking code sends data to the Google servers where it is stored.
3. **The Tracking Code**:A tracking code is provided by Google Analytics for each website you are tracking.

- **Domain Names & Hosting**:In order to put your site on the web you will need a domain name and web hosting.
 
1. **Domain Names**: Your domain name is your web address (e.g. google.com or bbc.co.uk). There are many websites that allow you to register domain names. Usually you will have to pay an annual fee to keep that domain name.

2. **Web HOsting**:So that other people can see your site, you will need to upload it to a web server. Web servers are special computers that are constantly connected to the Internet.

- To transfer your code and images from your computer to your hosting company, you use something known as File Transfer Protocol.allows you to transfer files across the
Internet from your computer to the web server hosting your site.

- 