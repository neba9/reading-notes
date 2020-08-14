
# Forms

- **Form**: to refer to different elements that allow you to collect information from visitors to your site.Whether you are adding a simple search box to your website or
you need to create more complicated insurance applications,
HTML forms give you a set of elements to collect data from
your users.

# Form Structure:
- ```<form>```:Form controls live inside a <form> element. This element should always carry the action attribute and will usually have a method and id attribute too.

- **action**:Every <form> element requires an action attribute. Its value is the URL for the page on the
server that will receive the information in the form when it is submitted.

- **method**:Forms can be sent using one of two methods: get or post.

- **Id**:the value is used to identify the form distinctly from other elements on the page.

- **Form Controls**:There are several types of form controls that you can use to collect information from visitors to your site. 

1. **ADDING TEXT**:
- **Text input (single-line)**: Used for a single line of text such as email addresses and names.
- Ex: ```<form action="http://www.example.com/login.php">```
```<p>Username:```
```<input type="text" name="username" size="15"```
```maxlength="30" />```
```</p>```
```</form>```

- The ```<input>``` element is used to create several different form controls. The value of the type attribute determines what kind of input they will be creating.

- **type="text"**:When the type attribute has a value of text, it creates a singleline text input.

- **name**:When users enter information into a form.

- **size**: The size attribute should not be used on new forms. It was used in older forms.

- **maxlength**:You can use the maxlength attribute to limit the number of characters.

### other fome controls:

- **Password input**:Like a single line text box but it masks the characters entered.

- **Text area (multi-line)**: For longer areas of text, such as messages and comments.

2. **Making Choices**:
- **Radio buttons**:For use when a user must select one of a number of options.
- **Checkboxes**:When a user can select and unselect one or more options.
- **Drop-down boxes**:When a user must pick one of a number of options from a list.

3. **Submitting Forms**:
- **Submit buttons**: To submit data from your form to another web page.
- **Image buttons**:Similar to submit buttons but they allow you to use an image.

4. **Uploading Files**:
- **File upload**:Allows users to upload files (e.g.images) to a website.

# Lists, Tables and Forms

- **lists**:The list-style-type property allows you to control the shape or style of a bullet point (also known as a marker).
- It can be used on rules that apply to the ```<ol>, <ul>, and <li>``` elements.

- **Unordered Lists**:For an unordered list you can use the following values:none, disc, circle, square.

- **Ordered Lists**:For an ordered (numbered) list you can use the following values:decimal 1 2 3,decimal-leading-zero 01 02 03,lower-alpha a b c,upper-alpha A B C, lower-roman i. ii. iii,upper-roman I II III.

- Ex:```ol {```
```list-style-type: lower-roman;}```

- **list-style-image**:You can specify an image to act
as a bullet point using the list-style-image property.

- Ex:```ul {```
```list-style-image: url("images/star.png");}```
```li {```
```margin: 10px 0px 0px 0px;}```

- **list-style-position**:lists are indented into the page
by default and the list-styleposition property indicates
whether the marker should appear on the inside or the
outside of the box containing the main points.

- This property can take one of two values:outside or inside.
- Ex: ```ul.illuminations {```
```list-style-position: outside;}```

### Table properties:

- **width**: to set the width of the .table

- **padding**: to set the spacebetween the border of each table cell and its content

- **text-transform**: to convert the content of the table headers to uppercase

- **letter-spacing, font-size**:to add additional styling to the content of the table headers

- **border-top, border-bottom**:to set borders above and below the table headers

- **text-align**:to align the writing to the left of some table cells and to the right of the others

- **background-color**: to change the background color of the alternating table rows

- **hover**: to highlight a table row when a user's mouse goes over it

- Ex:
```<table>```
```<tr>```
```<th>Author</th>```
```<th>Title</th>```
```<th class="money">Reserve Price</th>```
```<th class="money">Current Bid</th>```
```</tr>```
```</table>```

```th {```
```text-transform: uppercase;```
```letter-spacing: 0.1em;```
```font-size: 90%;```
```border-bottom: 2px solid #111111;```
```border-top: 1px solid #999;```
```text-align: left;}``` 

# Events

- **HOW EVENTS TRIGGER JAVASCRIPT CODE**:

- When the user interacts with the HTML on a web page, there are three steps involved in getting it to trigger some JavaScript code.Together these steps are known as event handling.

1. Select the element node(s) you want the script to respond to.

2. Indicate which event on the selected node(s) will trigger the response.

3. State the code you want to run when the event occurs.

- **There are three types of event handlers**.

1. **HTML EVENT HANDLERS**

2. **TRADITIONAL DOM EVENT HANDLERS**

3. **DOM LEVEL 2 EVENT LISTENERS**:Event listeners are a more recent approach to handling events.They can deal with more than one function at a time but they are not supported in older browsers.

- Ex: element.addEventlistener('event', functionName [, Boolean]) ;
- Element:DOM element node to target.
- Event: event to bind node(s) to in quote marks.
- code(function):name of function to call.
- event flow (Boolean):indicates something called capture,and  is usually set to false.

- Ex: **USING PARAMETERS WITH EVENT LISTENERS**

```var elUsername = document.getElementById('username');``` // get username input
```var elMsg = document.getElementById('feedback');``` //get feedback element

```function checkUsername(minlength) {``` //Declare function
```if (elUsername.value.length<minLength>){``` //if usrename too short
//Set the error message 
```elMsg.textContent = 'username must be ' + minlength + 'characteer or more';```
 ```}else {``` //otherwise
```elMsg.innerHTML ='';``` //clear msg
 ```}```
```}```
```elUsername.addEventListener('blur, function() {``` //when it loses focus
```checkUsername(5);``` //pass arguments here
```},false);```

- 
