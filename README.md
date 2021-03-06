compose
=======

String composing with placeholders for JavaScript.

Add the compose.min.js to the \<head> section of your page and start composing strings!

Use:

```javascript
var name = "Marc";
var product = "pears";

var s = "Hi, I'm {0}, I'd like to buy {1}.".compose(name, product);

// Result: Hi, I'm Marc, I'd like to buy pears.
```


Or:
```javascript
var array = ["Marc", "pears"];

var s = "Hi, this is {0}, I'd like to buy {1}.".compose(array);

// Result: Hi, this is Marc, I'd like to buy pears.
```


Also:
```javascript
var product = "pears";

var s = "{0} is the best product ever, nothing compares to {0}.".compose(product);

// Result: pears is the best product ever, nothing compares to pears.
```


Never again:
```javascript
var product = "pears";

var s = product + " is the best product ever, nothing compares to " + product + ".";
```
