# Class 13 Reading Notes
Native applications have an advantage over web applications because the have persistent **local storage** there are lots of solutions for storing data in local apps, and less so in web apps, historically.
- **cookies** were invented and can be used for persistent local storage in small amounts but have some setbacks:
- they slow down the web application by needlessly transmitting the same data over and over
- the send data unencrypted over the internet
- they are limited to about 4kb of data
**the goal:**
- a lot of storage space
- on the client
- that persists beyond a page refresh
- and isn't transmitted to the server

## HTML5 Storage
a specification named **Web Storage**
- provides a way for web pages to store named key/value pairs locally, within the client web browser. 
**Browsers that support it:**
- IE
- Firefox
- Safari
- Chrome
- Opera
- IPhone
-Android
From your JS code, you'll access HTML5 storage through the `localStorage` object on the **global window object**
- you can you **modernizr** to detect support for HTML5 Storage.
- HTML5 Storage is based on **named key/value** pairs. You store data based on a named key, then you can retrieve that data with the same key. 
- The named key is a **string**.
-  The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. However, the data is actually stored as a string.
- If you are storing and retrieving anything other than strings, you will need to use functions like `parseInt()` or ``parseFloat()`` to coerce your retrieved data into the expected JavaScript datatype.
- Calling `setItem()` with a named key that already exists will silently overwrite the previous value. 
- Calling `getItem()` with a non-existent key will return null rather than throw an exception.
- you can treat the localStorage object as an **associative array**. Instead of using the getItem() and setItem() methods, you can use **square brackets**.
- 5 megabytes of named key/value pairs
## Tracking Changes to the HTML5 Storage Area
- If you want to keep track programmatically of when the storage area changes, you can **trap** the storage event. The storage event is fired on the window object whenever `setItem()`, `removeItem()`, or `clear()` is called and actually changes something.
- The storage event is **not cancelable**. From within the `handle_storage` callback function, there is no way to stop the change from occurring. It’s simply a way for the browser to tell you, “hey, this just happened. There’s nothing you can do about it now; I just wanted to let you know.”
## Competeing Visions
- **Gears** was launched by Google in 2007 and led to the creation of the **Web SQL Database**
- **Indexed Data API** 


[Back to Top](#) [Back to Code 201](code201notes.md) [<-- Back](README.md)