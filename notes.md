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
> anywhere you can use a number or a string, you can also use a variable containing a number or a string.

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


// STRING
"9" + 9  // "99"

"skdjskjjsds".length;
var myAwesomeString = "awesome";
myAwesomeString.length;

// [] square brackets
// () parentheses
// . period
// , comma
// ; semicolon

var codeWord1 = "are";
var codeWord2 = "tubas";
var codeWord3 = "unsafe";
var codeWord4 = "?!";
codeWord1[1] + codeWord2[1] + codeWord3[1] +codeWord4[1];
// "run!"

"a string".slice(0, 3); // "a s"
"a string".slice(4); // "ring" 

var message = "Hello there, how are you doing?";
message.toUpperCase();  // "HELLO THERE, HOW ARE YOU DOING?"
message.toLowerCase();  // "hello there, how are you doing?"

var newMessage = message[0].toUpperCase() + message.slice(1).toLowerCase();  // 让首字母大写


```

- Boolean
```javascript
& // ampersand
| // pipe
! // bang

A && B
// 当A为true, 则返回B; 当A为false, 则返回A

A || B
// 当A为true, 则返回A; 当A为false, 则返回B

>= //greater than or equal to
<= //less than or equal to
=== // triple equal, is equal to
== // double equal

"5" === 5 // false
"5" == 5 // true
0 == false // true
"false" == false // false
```

- undefined VS null
```javascript
// when you create a new variable,if you don’t set its value to anything using the = operator, its value will be set to undefined
var myVariable;  // undefined

// The null value is usually used when you want to deliberately say “This is empty.”
var myNullVariable = null;
```

- array
```javascript
var dinosaurs = [];
dinosaurs[0] = "T-Rex";
dinosaurs[1] = "Velociraptor";
dinosaurs[2] = "Stegosaurus";
dinosaurs[3] = "Triceratops";
dinosaurs[33]="Philosoraptor"; // length: 34


var dinosaursAndNumbers = [3, "dinosaurs", ["triceratops", "stegosaurus", 3627.5], 10];
dinosaursAndNumbers[2][1]
// "stegosaurus"

dinosaursAndNumbers.length
dinosaursAndNumbers[dinosaursAndNumbers.length -1]

var animals = [];
animals.push("cat");  // 开头插入
animals.push("dog");
animals.push("Llama"); 
animals.unshift("Monkey");  // 末尾插入
animals.unshift("Polar Bear");
// ["Polar Bear", "Monkey", "cat", "dog", "Llama"]

animals.pop();  // 弹出最后
animals.shift();  // 弹出最前

// concatenate
firstArray.concat(otherArray);

// concat可以拼接多个数组
fisrtArry.concat(one, two ,three);

// finding the index of an element
array.indexOf(element);
colors.indexOf("blue");

// turning an array into a string
var boringAnimals = ["Monkey", "Cat", "Fish", "Lizard"];
boringAnimals.join(); // "Monkey,Cat,Fish,Lizard" 默认用comma
boringAnimals.join(" "); // "Monkey Cat Fish Lizard"
["Your", "dress", "is", "beautiful" + "!!!"].join(" "); // "Your dress is beautiful!!!"
[3, 2, 1].join(" is bigger than ") // "3 is bigger than 2 is bigger than 1"

// decision maker
Math.random();  // (0,1)
Math.random() * 7 // (0, 7)
Math.floor(Math.random() * 7) // [0, 6]
Math.ceil() // 向上取整
Math.round()  // 四舍五入

```