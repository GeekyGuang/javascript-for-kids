- 编程环境
> Google Chrome
> about:blank
> Ctrl + Shift + J
> shift + enter 换行

- comments and console
```javascript
// =^.^=
// Draw as many cats as you want!

/*
Draw as many cats
as you want!
*/
var drawCats = function (howManyTimes) {
    for (var i = 0; i < howManyTimes; i++) {
        console.log(i + " =^.^=");
    }
};

drawCats(10);

```

- three basic types of data: numbers, strings, Booleans
```javascript
var nick;
// undefined
// Creating a variable in JavaScript doesn’t return a value, so the interpreter prints undefined .

// variable
var numberOfSiblings = 1 + 3;  // camel case
var numberOfCandies = 8;
numberOfCandies / numberOfSiblings;

var secondsInAMinute = 60;
var minutesInAnHour = 60;
var hoursInADay = 24;
var daysInAYear = 365;
var secondsInAYear = daysInAYear * hoursInADay * minutesInAnHour * secondsInAMinute;
var age = 29;
age * secondsInAYear
// 914544000


// decrementing and incrementing
var highFives = 0;

// 先返回值后++/--
highFives++;
// 0
highFives
// 1
highFives--;
// 1

// 先++/--后返回值
++highFives;
// 1
--highFives;
// 0


var score = 10;
score += 7;  // plus-equals
// 17
score -= 3;  // minus-equals
// 14

// *=, /= 
```
