# JavaScript

[Website](http://www.w3schools.com/js/default.asp)



## JavaScript String Methods

[JavaScript String Methods](http://www.w3schools.com/js/js_string_methods.asp)

### indexOf() VS search()

The two methods, indexOf() and search(), are equal.

They accept the same arguments (parameters), and they return the same value.

The two methods are equal, but the search() method can take much more powerful search values.

You will learn more about powerful search values in the chapter about regular expressions.

### substring() VS slice()

substring() is similar to slice().

The difference is that substring() cannot accept negative indexes.

### replace()

The replace() method can also take a regular expression as the search value.

By default, the replace() function replaces only the first match. To replace all matches, use a regular expression with a g flag (for global match):

**Example**

``` JavaScript
str = "Please visit Microsoft!";
var n = str.replace(/Microsoft/g,"W3Schools");
```

### Accessing a String as an Array is Unsafe

You might have seen code like this, accessing a string as an array:

``` JavaScript
var str = "HELLO WORLD";

str[0];                   // returns H
```

This is unsafe and unpredictable:

* It does not work in all browsers (not in IE5, IE6, IE7)
* It makes strings look like arrays (but they are not)
* str[0] = "H" does not give an error (but does not work)

If you want to read a string as an array, convert it to an array first.

### Converting a String to an Array

* A string can be converted to an array with the split() method
* If the separator is "", the returned array will be an array of single characters:


