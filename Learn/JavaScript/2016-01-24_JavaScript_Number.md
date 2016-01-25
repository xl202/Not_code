# JavaScript

[Website](http://www.w3schools.com/js/default.asp)

## JavaScript Numbers

[JavaScript Numbers](http://www.w3schools.com/js/js_numbers.asp)

### Hexadecimal

JavaScript interprets numeric constants as hexadecimal if they are preceded by 0x.

**Example**

```JavaScript
var x = 0xFF;             // x will be 255
```

 you can use the `toString()` method to output numbers as base 16 (hex), base 8 (octal), or base 2 (binary).

**Example**

```JavaScript
var myNumber = 128;
myNumber.toString(16);     // returns 80
myNumber.toString(8);      // returns 200
myNumber.toString(2);      // returns 10000000
```


### Infinity

`Infinity` (or `-Infinity`) is the value JavaScript will return if you calculate a number outside the largest possible number.

**Example**

```JavaScript
var myNumber = 2;
while (myNumber != Infinity) {          // Execute until Infinity
        myNumber = myNumber * myNumber;
}
```

Division by 0 (zero) also generates Infinity:

**Example**

```JavaScript
var x =  2 / 0;          // x will be Infinity
var y = -2 / 0;          // y will be -Infinity
```

### NaN - Not a Number

`NaN` is a JavaScript reserved word indicating that a value is not a number.

Trying to do arithmetic with a non-numeric string will result in NaN (Not a Number):

**Example**

```JavaScript
var x = 100 / "Apple";  // x will be NaN (Not a Number)
```

**Don't create Number objects. It slows down execution speed.**

**The `new` keyword complicates the code. This can produce some unexpected results:**
