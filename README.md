## MyQuery
MyQuery is my own version of [JQuery](https://jquery.com).JQuery is a JavaScript Library that focuses on DOM manipulation, [AJAX](https://developer.mozilla.org/en-US/docs/Glossary/AJAX) and Event handling. The usage is very similar to jQuery:
```js
// alerts Hello World after the page finished loading
$(document).ready(() => {
    alert("Hello World");
    // adds a click listener to a button with the 'myButton' id
    $("#myButton").click(() => {
        alert("You clicked me!");
    });
})

// creates a new div with the name 'myDiv'
const myDiv = $.create("div",{name: "myDiv"});
```

### Features
**Selector**

- `$(element)`
- `$("#id")`
- `$("div")`
- `$("div.class")`

**Action**

- `.on(eventName, callback)`
- `.click(callback)`
- `.data(key, value)`
- `.add(...classNames)`
- `.remove(...classNames)`
- `.toggleClass(className)`
- `.append(element)`
- `.appendTo(parent)`
- `.text(text?)`
- `.html(html?)`
- `.css(key, value)`
- `.css(styleObject)`
- `.hide()`
- `.show()`
- `.value(newValue)`
- `.value()`
- `.toggle()`

**Static Actions**

- `.wait(milliseconds)`
- `.post(url, data, callback)`
- `.get(url, callback)`
- `.create(tagName, attributes?, children?)`