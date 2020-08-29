# The Past, Present and Future of local storage for web application.

- **Present local storage**:storage is one of the areas where native client applications have held an advantage over web applications. For native applications, the operating system typically provides an abstraction layer for storing and retrieving application-specific data like preferences or runtime state. These values may be stored in the registry, INI files, XML files, or some other place according to platform convention. If your native client application needs local storage beyond key/value pairs, you can embed your own database, invent your own file format, or any number of other solutions.

- **HTML storage**:is a specification named **Web Storage**.**HTML5 Storage** Simply put, it’s a way for web pages to store named key/value pairs locally, within the client web browser.like cookies,this data persists even after you navigate away from the web site, close your browser tab, exit your browser, or what have you. Unlike cookies.
-  this data is never transmitted to the remote web server (unless you go out of your way to send it manually).

- the latest version of pretty much every browser supports HTML5 Storage… even Internet Explorer!

- **HTML5 STORAGE SUPPORT**:
- IE 8.0+, FIREFOX 3.5+, SAFARI 4.0+, CHROME 4.0+, OPERA10.5+, IPHONE 2.0+, ANDROID2.0+ 

- From your JavaScript code, you’ll access HTML5 Storage through the localStorage object on the global window object. Before you can use it, you should detect whether the browser supports it.

- **check for HTML5 Storage**:

- ```function supports_html5_storage() {```
  ```try {```
    ```return 'localStorage' in window && window``````['localStorage'] !== null;```
  ```} catch (e) {```
    ```return false;```
  ```}```
```}```

- **USING HTML5 STORAGE**:HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key.

-  The named key is a string.
- The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. However, the data is actually stored as a string.

-  If you are storing and retrieving anything other than strings, you will need to use functions like **parseInt()** or **parseFloat()** to coerce your retrieved data into the expected JavaScript datatype.

-  you can treat the localStorage object as an associative array. Instead of using the getItem() and setItem() methods, you can simply use square brackets.For example

- ```var foo = localStorage.getItem("bar");```
// ...
```localStorage.setItem("bar", foo);```

- could be rewritten to use square bracket syntax instead:

- ```var foo = localStorage["bar"];```
// ...
```localStorage["bar"] = foo;```

- There are also methods for removing the value for a given named key, and clearing the entire storage area (that is, deleting all the keys and values at once).

- Ex: ```interface Storage {```
  ```deleter void removeItem(in DOMString key);```
  ```void clear();```
```};```

- Calling **removeItem()** with a non-existent key will do nothing.

- Finally, there is a property to get the total number of values in the storage area, and to iterate through all of the keys by index (to get the name of each key).

- Ex: ```interface Storage {```
  ```readonly attribute unsigned long length;```
 ```getter DOMString key(in unsigned long index);```
```};```

- If you call key() with an index that is not between 0–(length-1), the function will return null.

- **TRACKING CHANGES TO THE HTML5 STORAGE AREA**:If you want to keep track programmatically of when the storage area changes, you can trap the storage event. The storage event is fired on the window object whenever setItem(), removeItem(), or clear() is called and actually changes something.The storage event is supported everywhere the localStorage object is supported.

- **HTML5 STORAGE IN ACTION**:If your browser supports HTML5 Storage, the demonstration page should magically remember your exact position within the game, including the number of moves you’ve made, the position of each of the pieces on the board, and even whether a particular piece is selected.

- For example, the flag for whether there is a game in progress (gGameInProgress) is a Boolean. In the saveGameState() function, we just stored it and didn’t worry about the datatype:

- ```localStorage["halma.game.in.progress"] = gGameInProgress;```

- But in the resumeGame() function, we need to treat the value we got from the local storage area as a string and manually construct the proper Boolean value ourselves:
- ```gGameInProgress = (localStorage["halma.game.in.progress"] == "true");```

- Similarly, the number of moves is stored in gMoveCount as an integer. In the saveGameState() function, we just stored it:
- ```localStorage["halma.movecount"] = gMoveCount;```

- But in the resumeGame() function, we need to coerce the value to an integer, using the parseInt() function built into JavaScript:
- ```gMoveCount = parseInt(localStorage["halma.movecount"]);```

- Web SQL Database (formerly known as “WebDB”) provides a thin wrapper around a SQL database, allowing you to do things like this from JavaScript:

- The Web SQL Database specification has been implemented by four browsers and platforms.