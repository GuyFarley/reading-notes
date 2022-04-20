# Code 201 - Class 13 - Local Storage

## Why this matters

- Occasionally we will need our web sites to include the capability to store data locally. For instance, if we create a game and we don't want our user to lose their progress upon reloading the page - we would need the ability to store their game's progress and re-access upon reload. The tools in the reading will allow us to do that.

## [“The Past, Present, and Future of Local Storage for Web Applications”](http://diveinto.html5doctor.com/storage.html)

- Web apps have historically struggled with local storage. Ideally, web applications would have lots of storage space, that exists on the client, persists beyond a page refresh, and isn't transmitted to the server
- **HTML5 Storage** (or **Web Storage**) provides a way for web pages to store key-value pairs locally within the client's web browser
- HTML5 Storage is accessed through the `localStorage` object on the global `window` object
- Since it is based on key-value pairs, you can store data based on a key, then access the locally-stored data with the same key name
- **IMPORTANT:** The locally-stored data is always saved as a string, so you'll need to use `parseInt` or `parseFloat` to change the string to an integer if a number is needed
- A `storage` event can be used to keep track of changes to the storage area. Example (from the HTML5 Doctor article):

```
if (window.addEventListener) {
  window.addEventListener("storage", handle_storage, false);
} else {
  window.attachEvent("onstorage", handle_storage);
};
```

## Things I want to know more about

- API's (Application Programming Interfaces)
- More examples of practical uses of Web Storage

[Back to Home](../README.md)
