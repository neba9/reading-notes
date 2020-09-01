# CSS Transforms

- Now general layout techniques can be revisited with alternative ways to **size**, **position**, and **change elements**. All of these new techniques are made possible by the **transform property**.

- The transform property comes in two different settings, **two-dimensional** and **three-dimensional**. Each of these come with their own individual properties and values.

- **Transform Syntax**:including the transform property followed by the value. The value specifies the transform type followed by a specific amount inside parentheses.

- ```div {```
  ```-webkit-transform: scale(1.5);``
     ```-moz-transform: scale(1.5);```
       ```-o-transform: scale(1.5);```
          ```transform: scale(1.5);```
```}```

1. **2D Transforms**: Two-dimensional transforms work on the x and y axes, known as horizontal and vertical axes. 
- The transform property accepts a handful of different values.Using a positive value will rotate an element clockwise, and using a negative value will rotate the element counterclockwise.

-  **2D Rotate**:The rotate value provides the ability to rotate an element from 0 to 360 degrees.
- ```.box-1 {```
  ```transform: rotate(20deg);}```

- **2D Scale**:allows you to change the appeared size of an element. The default scale value is 1.
- ```.box-1 {```
  ```transform: scale(.75);}```

- **2D Translate**: translate value works a bit like that of relative positioning, pushing and pulling an element in different directions without interrupting the normal flow of the document.
- ```.box-2 {```
  ```transform: translateY(25%);}```

- **2D Skew**: skew, is used to distort elements on the horizontal axis, vertical axis, or both.Using the skewX value distorts an element on the horizontal axis.
- ```.box-1 {```
  ```transform: skewX(5deg);```

- **Combining Transforms**:It is common for multiple transforms to be used at once, rotating and scaling the size of an element at the same time for example.
- ```.box-1 {```
  ```transform: rotate(25deg) scale(.75);}```
- ```.box-2 {```
  ```transform: skew(10deg, 20deg) translateX(20px);}```

2. **3D Transforms**: Three-dimensional transforms work on both the x and y axes, as well as the z axis. These three-dimensional transforms help define not only the length and width of an element, but also the depth. 

- **3D Rotate**:With three-dimensional transforms we can rotate an element around any axes. To do so, we use three new transform values, including rotateX, rotateY, and rotateZ.
- ```.box-3 {```
  ```transform: perspective(200px) rotateZ(45deg);}```

- **3D Scale**:By using the scaleZ three-dimensional transform elements may be scaled on the z axis.
- ```.box-1 {```
  ```transform: perspective(200px) scaleZ(1.75) rotateX````(45deg);}```

- **3D Translate**: A negative value here will push an element further away on the z axis, resulting in a smaller element. Using a positive value will pull an element closer on the z axis, resulting in a larger element.
- ```.box-1 {```
  ```transform: perspective(200px) translateZ(-50px);```

- **3D Skew**:Skew is the one two-dimensional transform that cannot be transformed on a three-dimensional scale.

# Transitions & Animations

- **Transitions** provide a change from one state to another, while animations can set multiple points of transition upon different keyframes.

- There are **four transition related properties** in total Not all of these are required to build a transition, with the first three are the most popular.

1. **transition-property**:not all properties may be transitioned,only properties that have an identifiable halfway point. Colors, font sizes, and the alike may be transitioned from one value to another.
- ```.box {```
  ```background: #2db34a;```
  ```border-radius: 6px;```
  ```transition-property: background, border-radius;```
  ```transition-duration: .2s, 1s;```
  ```transition-timing-function: linear;```
```}```
```.box:hover {```
  ```background: #ff7b29;```
  ```border-radius: 50%;```
```}```

2. **transition-duration**:The value of this property can be set using general timing values, including seconds (s) and milliseconds (ms). These timing values may also come in fractional measurements, .2s for example.

3. **transition-timing-function**: property is used to set the speed in which a transition will move.

4. **transition-delay**: The delay sets a time value, seconds or milliseconds, that determines how long a transition should be stalled before executing.

- **Animations**:when more control is required, transitions need to have multiple states. In return, this is where animations pick up where transitions leave off.

- **Animations Keyframes**:To set multiple points at which an element should undergo a transition, use the @keyframes rule. The @keyframes rule includes the animation name, any animation breakpoints, and the properties intended to be animated.
- ```@keyframes slide {```
  ```0% {```
    ```left: 0;```
    ```top: 0;}```
 ```50% {```
    ```left: 244px;```
    ```top: 100px;```
  ```}```
  ```100% {```
    ```left: 488px;```
    ```top: 0;```
 ```}```
```}```

- **Vendor Prefixing the Keyframe Rule**:The @keyframes rule must be vendor prefixed, just like all of the other transition and animation properties. The vendor prefixes for the @keyframes rule look like the following:
- @-moz-keyframes
- @-webkit-keyframes
- @-o-keyframes

- **The transition property** has three values: the properties to transition (in our case all of them) the speed of the transition (in our case 0.3 seconds) and a third value which lets you change how the acceleration and deceleration is calculated, but we’ll stick with the default by leaving this blank.

- Ex:```<style type="text/css">```
```body > div```
```{```
            ```width:483px;```
            ```height:298px;```
            ```background:#676470;```
            ```transition:all 0.3s ease;```
```}```
```</style>```

- ### 8 SIMPLE CSS3 TRANSITIONS THAT WILL WOW YOUR USERS.

1. **Fade in**:Fade in effects are coded in two steps: first, you set the initial state; next, you set the change, for example on hover:
- ```.fade```
```{```
        ```opacity:0.5;```
```}```
```.fade:hover```
```{```
        ```opacity:1;```
```}```

2.  **Change color**:we just set the div’s class to “color” and specify the color we want in our CSS:
- ```.color:hover```
```{```
        ```background:#53a7ea;}```

3. **Grow & Shrink**:To grow an element, you used to have to use its width and height, or its padding. But now we can use CSS3’s transform to enlarge.Set your div’s class to “grow” and then add this code to your style block:
- ```.grow:hover```
```{```
        ```-webkit-transform: scale(1.3);```
        ```-ms-transform: scale(1.3);```
        ```transform: scale(1.3);}```

- Shrinking an element is as simple as growing it. To enlarge an element we specify a value greater than 1, to shrink it, we specify a value less than 1:

4. **Rotate elements**:CSS transforms have a number of different uses, and one of the best is transforming the rotation of an element. Give your div the class “rotate” and add the following to your CSS:
- ```.rotate:hover```
```{```
        ```-webkit-transform: rotateZ(-30deg);```
        ```-ms-transform: rotateZ(-30deg);```
        ```transform: rotateZ(-30deg);}```

5. **Square to circle**:A really popular effect at the moment is transitioning a square element into a round one, and vice versa. With CSS, it’s a simple effect to achieve, we just transition the border-radius property.

- Give your div the class “circle” and add this CSS to your styles:
- ```.circle:hover```
```{```
        ```border-radius:50%;}```

6. **3D shadow**:This effect is achieved by adding a box shadow, and then moving the element on the x axis using the transform and translate properties so that it appears to grow out of the screen.
- Give your div the class “threed” and then add the following code to your CSS:
- ```.threed:hover```
```{```
        ```box-shadow:```
                ```1px 1px #53a7ea,```
                ```2px 2px #53a7ea,```
                ```3px 3px #53a7ea;```
        ```-webkit-transform: translateX(-3px);```
        ```transform: translateX(-3px);}```

7. **Swing**: We can also create highly complex animations using @keyframes, animation and animation-iteration.
- In this case, we’ll first define a CSS animation in your styles. You’ll notice that due to implementation issues, we need to use @-webkit-keyframes as well as @keyframes (yes, Internet Explorer really is better than Chrome, in this respect at least).

8. ** Inset border**:Give your div the class “border” and add the following CSS to your styles:
- ```.border:hover```
```{```
        ```box-shadow: inset 0 0 0 25px #53a7ea;}```



