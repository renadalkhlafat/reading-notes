# Local Storage
The localStorage object stores data with no expiration date. The data will not be deleted when the browser is closed, and will be available the next day, week, or year.The localStorage property is read-only

HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. However, the data is actually stored as a string. If you are storing and retrieving anything other than strings, you will need to use functions like parseInt() or parseFloat() to coerce your retrieved data into the expected JavaScript datatype.


    interface Storage {
    getter any getItem(in DOMString key);
    setter creator void setItem(in DOMString key, in any data);
    }; 



    var foo = localStorage["bar"];
    // ...
    localStorage["bar"] = foo;

If you want to keep track programmatically of when the storage area changes, you can trap the storage event. The storage event is fired on the window object whenever setItem(), removeItem(), or clear() is called and actually changes something. For example, if you set an item to its existing value or call clear() when there are no named keys, the storage event will not fire, because nothing actually changed in the storage area.


    if (window.addEventListener) {
    window.addEventListener("storage", handle_storage, false);
    } else {
    window.attachEvent("onstorage", handle_storage);
    };

The `handle_storage` callback function will be called with a StorageEvent object, except in Internet Explorer where the event object is stored in window.event.

    function handle_storage(e) {
     if (!e) { e = window.event; }
      }
At this point, the variable e will be a StorageEvent object