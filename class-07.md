
# Table

- A table represents information in a grid format.
- The ```<table>``` element is used to create a table. The contents of the table are written out row by row.

- ```<tr>```: You indicate the start of each row using the opening <tr> tag. (The tr stands for table row.) It is followed by one or more <td> elements (one for each cell in that row). At the end of the row you use a closing </tr> tag.

- ```<td>```: Each cell of a table is represented using a <td> element. (The td stands for table data.) At the end of each cell you use a closing </td> tag.

- ```<th>```: The <th> element is used just like the <td> element but its purpose is to represent the heading for either a column or a row. (The th stands for table heading.)

- Even if a cell has no content,you should still use a <td> or <th> element to represent the presence of an empty cell otherwise the table will not render correctly. (The first cell in the first row of this example shows an empty cell.)

- EX: ```<table>```
```<tr>```
```<th></th>```
```<th scope="col">Saturday</th>```
```<th scope="col">Sunday</th>```
```</tr>```
```<tr>```
```<th scope="row">Tickets sold:</th>```
```<td>120</td>```
```<td>135</td>```
```</tr>```
```<tr>```
```<th scope="row">Total sales:</th>```
```<td>$600</td>```
```<td>$675</td>```
```</tr>```
```</table>```

- **Spanning ColumnS**:

- **Sometimes**: you may need the entries in a table to stretch across more than one column. The colspan attribute can be used on a <th> or <td> element and indicates how many columns that cell should run across.

- Ex: ```<table>```
     ```<tr>```
     ```<th>Monday</th>```
     ```<td colspan="2">Geography</td>```
     ```</tr>```
     ```</table>```

- **Spanning Rows**:You may also need entries in a table to stretch down across more than one row. The rowspan attribute can be used on a <th> or <td> element to indicate how many rows a cell should span down the table.

- Ex:```<table>```
     ```<tr>```
     ```<th>6pm - 7pm</th>```
     ```<td rowspan="2">Movie</td>```
     ```<td>Comedy</td>```
     ```</tr>```
     ```</table>```

- **Long Tables**:There are three elements that help distinguish between the main content of the table and the first and last rows (which can contain different content).

1. ```<thead>``` The headings of the table should sit inside the <thead> element.

2. ```<tbody>``` The body should sit inside the <tbody> element.

3. ```<tfoot>``` The footer belongs inside the <tfoot> element.

# Function, Methods and Objects

- creating an object:constructor notation:The new keyword and the object constructor create a blank object.you can then add properties and methods to the object.

- Ex: ```var hotel = new object();```
      ```hotel.name = 'Quay';```
      ```hotel.roooms = 40;```
      ```hotel.booked = 25;```

      ```hotel.checkAvailability = function(){```
      ```return this.room - this.booked;```
    ```};```

- to creat an empty object using literal notation use 
 ```var hotel = {}``` the curly brackets creat an empty object.

 - to update the value of properties,use dot notation or square brackets.object name followed by square brackets and the property name is inside them and a new value for the property is add after the assignment opretor.
 - Ex: ```hotel.name = 'park';```    you use
       ```hotel['name']='park';```
 
 - the work on objects created using literal or constractor notation.
 - Ex: 
 
- to delete a property, use delete keyword.
- Ex: ```delete hotel.name;```

- if you just want to clear the value of a property,you could set it to a bank string.
- Ex: ```hotel.name ='';```

- **RECAP: WAYS TO CREATE OBJECTS**

- **CREATE THE OBJECT, THEN ADD PROPERTIES & METHODS**

- In both of these examples, the object is created on
the first line of the code sample. The properties and
methods are then added to it afterwards.

1. **LITERAL NOTATION**:

- Ex: 
```var hotel = {}```

```hotel .name= 'Quay';```
```hotel .rooms = 40;```
```hotel.booked = 25;```
```hotel.checkAvailabil ity =function()```
```return this . rooms - this .booked;```
```} ;```

- **CREATING AN OBJECT WITH PROPERTIES & METHODS**:
- **LITERAL NOTATION**:A colon separates the key/value pairs.There is a comma between each key/value pair.

-Ex: 
```var hotel = {```
```name: 'Quay',```
```rooms: 40,```
```booked: 25,```
```chec kAvailability: function() {```
```return this.rooms - this .booked;```
```}```
```} ;```

2. **OBJECT CONSTRUCTOR NOTATION**
- Ex:
```var hotel = new Object();```

```hotel.name = 'Quay';```
```hotel .rooms = 40 ;```
```hotel . booked= 25;```
```hotel.checkAvailability =function()```
```return this .rooms - this .booked;```
```} ;```

- **CREATING AN OBJECT WITH PROPERTIES & METHODS**:
- **OBJECT CONSTRUCTOR NOTATION**:The function can be used to create multiple objects.The this keyword is used instead of the object name.

- Ex; 
```function Hotel(name, rooms, booked) {```
```this.name = name;```
```this.rooms = rooms;```
```this.booked = booked;```
```this.checkAvailability = functio n()```
```return this . rooms - this.booked;```
```} ;```

```var quayHotel =new Hotel('Quay', 40 , 25);```
```var parkHotel =new Hotel('Park', 120, 77);```

- **In JavaScript**, data is represented using name/value pairs.To organize your data, you can use an array or object to group a set of related values. In arrays and objects the name is also known as a key.

- **VARIABLES**:A variable has just one key (the variable name) and one value.
Variable names are separated from their value by an equals sign (the assignment operator):
```var hotel= 'Quay' ;```
To retrieve the value of a variable, use its name:II This retrieves Quay:hotel ;

- **ARRAYS**:Arrays can store multiple pieces of information.Each piece of information is separated by a comma.The order of the values is important because items
in an array are assigned a number (called an index).

Values in an array are put in square brackets, separated by commas:
```var hotels = [```
```'Quay ',```
```'Park',```
```'Beach',```
```'Bloomsbury'```
```]```
You can think of each item in the array as another
key/value pair, the key is the index number, and the
values are shown in the comma-separated list.

To retrieve an item, use its index number:
II Thi s retrieves Park:
hote1s [l] ;

- **Arrys**:are object actually special type of object.they hold a related set of key/value pairs(like all objects),but the keyfor each value is its index number.

- Ex:an object has property and value
- ```costs = {```
  ```room1:420,```
  ```room2:460,```
  ```room3:230,```
  ```room4:620```
```};```

- Ex: an Array has index number and value

- ```costs = [420,460,230,620];```

- you can combine arrays and objects to create complex data structures ;Arrays can stord of **object**(and remember their order)Object can olso hold **arraya**(as values of their properties)

- **Arrays in an object**:the property of any object can hold an array.on the left.```costs.rooom1.items[0];``` 
      property:     value:
- Ex: room1:       items[420,40,10]
      room2:       items[460,20,20]

-  **objects in an Array**:the value of any element in an array can an object. ```costs[2].phone;```
      index number;    value:
- Ex:     0  :   {accom:420,food:40,phone:10}
          1  :   {accom:460,food:20,phone:20}

