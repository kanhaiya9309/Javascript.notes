# Javascript.notes

### Example 1 - Basic Functionality
```javascript
// Basic Functionality of alert, console.log, and prompt

// Multiple alerts
alert("Hello");
alert("World");

// Logging multiple values
console.log("Happy", "New", "Year", "2023");

// Using prompt to get user input
var yourName = prompt("What is your name?");
prompt("What is your qualification");
prompt("What is your current profession");

// Concatenating and displaying a message
var myName = "Kanhaiya";
alert("My name is " + myName + ", welcome to my Website " + yourName + "!");
```

### Example 2 - Twitter-like Functionality
```javascript
// Example 2 - Twitter-like functionality

// Using prompt to get user input
var yourIntro = prompt("Write something about you?");

// Slicing and alerting the first 140 characters
alert(yourIntro.slice(0, 140));

// Optional: Displaying the remaining word count
// var introLength = yourIntro.length;
// alert("Your word count is " + introLength + " and your remaining word count is " + (140 - introLength));
```

### Example 3 - Variable Assignment Replacement
```javascript
// Example 3 - Variable assignment replacement

// Using prompt to get user input
var a = prompt("Hello How Are you ? ");
var b = prompt("What is Your name ? ");

// Swapping the values of variables
var c = a;
a = b;
b = c;

console.log(a);
console.log(b);
```

### Example 4 - First Character to Uppercase
```javascript
// Example 4 - First character to uppercase

// Using prompt to get user input
var name = prompt("What is your name?");
var firstChar = name.slice(0, 1);
var upperCaseName = firstChar.toUpperCase();
var restOfName = name.slice(1, name.length);
var lowerCaseName = restOfName.toLowerCase();
var capitalise = upperCaseName + lowerCaseName;
alert("Hello, " + capitalise);
```

### Example 5 - Age of Dog Calculation
```javascript
// Example 5 - Age of Dog calculation

// Using prompt to get user input
var dogAge = prompt("What is your dog age?");
var humanAge = ((dogAge - 2) * 4) + 21;
console.log("Your dog is " + humanAge + " years old in human years.");
```

### Example 6 - Operator Precedence
```javascript
// Example 6 - Operator precedence

var x = 3;
x = x + 1;
var y = x++;
var z = y += 1;
console.log("The value of Y is " + z);
```


### Example 7 - BMI Calculator
```javascript
// BMI Calculator

var weight = prompt("Enter your Weight in Kg to calculate BMI");
var height = prompt("Enter your Height in Cm to calculate BMI");

function bmiCalculator(weight, height) {
    var heightInMeters = height / 100;
    var bmi = weight / (heightInMeters * heightInMeters);
    return bmi;
}

var bmi = bmiCalculator(weight, height);
bmi = Math.floor(bmi);

if (bmi >= 18.5 && bmi <= 24.9) {
    alert("Your BMI is " + bmi + ", so you have a normal weight.");
} else if (bmi > 24.9) {
    alert("Your BMI is " + bmi + ", so you are overweight.");
} else {
    alert("Your BMI is " + bmi + ", so you are underweight.");
}
```

### Example 8 - Love Calculator
```javascript
// Love Calculator

var maleOne = prompt("Enter your name of loveOne");
var femaleOne = prompt("Enter your name of loveOne");
var lovePercentage = Math.random() * 100;
lovePercentage = Math.floor(lovePercentage) + 1;
alert(maleOne + " and " + femaleOne + " your love percentage is " + lovePercentage + "% ");

if (lovePercentage >= 80) {
    alert("Your love with each other is true");
} else if (lovePercentage >= 50) {
    alert("Your love with each other is in a compromise way");
} else {
    alert("Your love with each other is in a complicated way");
}
```

### Example 9 - Leap Year
```javascript
// Leap Year

var year = prompt("Enter the year to check if it's a leap year or not");

function isLeapYear(year) {
    return (year % 4 === 0 && year % 100 !== 0) || (year % 400 === 0);
}

var leapYear = isLeapYear(year);

if (leapYear) {
    alert(year + " This year is a leap year");
} else {
    alert(year + " This year is not a leap year");
}
```



### Example 10 - Birthday Invitation
```javascript
// Birthday Invitation

var guestInput = prompt("Enter your name");
var guestList = ["Kanhaiya", "Kunal", "Harshal", "Tushar", "Gaurav"];
var invitationList = guestList.includes(guestInput);

if (invitationList === true) {
    alert(guestInput + " Welcome!");
} else {
    alert(guestInput + " Sorry, maybe next time.");
}
```

### Example 11 - FizzBuzz By User
```javascript
// FizzBuzz By User

var userInput = prompt("Enter the number to check Fizz or Buzz");
var array = [];

function FizzBuzz() {
    if (userInput % 3 === 0 && userInput % 5 === 0) {
        array.push("FizzBuzz");
    } else if (userInput % 3 === 0) {
        array.push("Fizz");
    } else if (userInput % 5 === 0) {
        array.push("Buzz");
    }
    alert(userInput + " Number is a " + array);
}

FizzBuzz();
```

### Example 12 - FizzBuzz By Console.log
```javascript
// FizzBuzz By Console.log

var array = [];
var count = 1;

function FizzBuzz() {
    if (count % 3 === 0 && count % 5 === 0) {
        array.push("FizzBuzz");
    } else if (count % 3 === 0) {
        array.push("Fizz");
    } else if (count % 5 === 0) {
        array.push("Buzz");
    } else {
        array.push(count);
    }

    count++;
    console.log(array);
}

FizzBuzz();
```



### Example 13 - Who is Bill Pay
```javascript
// Who is Bill Pay

var names = ["kanhaiya", "kunal", "Gaurav", "Harshal", "Tushar"];

function whoPaying(names) {
    var random = Math.floor(Math.random() * names.length);
    var billPay = names[random];
    alert(billPay + " you bill pay");
}

whoPaying(names);
```

### Example 14 - Song by For Loop
```javascript
// Song by For Loop

// var mine =[];
var beer = 99;

function MineBeer() {
    while (beer >= 1) {
        // mine.push(beer);
        alert(beer + " bottles of beer on the wall,  " + beer + " bottles of beer. Take one down and pass it around, " + (beer - 1) + " bottles of beer on the wall.");
        beer--;
        // console.log(mine);
    }
}
```

### Example 15 - FizzBuzz by For Loop
```javascript
// FizzBuzz by For Loop

var array = [];
// var count = 1;

function FizzBuzz() {
    for (var count = 1; count <= 100; count++) {
        if (count % 3 === 0 && count % 5 === 0) {
            array.push("FizzBuzz");
        } else if (count % 3 === 0) {
            array.push("Fizz");
        } else if (count % 5 === 0) {
            array.push("Buzz");
        } else {
            array.push(count);
        }
        // count++;
        console.log(array);
    }
    // alert(userInput+" Number is a "+array);
}
```


### Example 16 - Fibonacci Series
```javascript
// Fibonacci Series

var input = prompt("Enter the number to make Fibonacci series");
var i = 0;
var j = 1;
var k = [i, j];
var array = [];

function FibonacciSeries(input) {
    if (input == 0) {
        alert(i + " is part of the Fibonacci series");
    } else if (input == 1) {
        alert(k + " is part of the Fibonacci series");
    } else if (input > 1) {
        array.push(i);
        array.push(j);

        for (var f = 2; f <= input; f++) {
            var nextValue = array[f - 1] + array[f - 2];
            array.push(nextValue);
        }

        alert(array + " is the Fibonacci series");
    }
}

FibonacciSeries(input);
```

### Example 17 - Practice Section: BMI Calculation Function
```javascript
// Birthday Invitation Using Function

var numPeople = parseInt(prompt("Enter the number of people you want to calculate BMI for"));

for (var i = 0; i < numPeople; i++) {
    var height = parseFloat(prompt("Enter height in meters for person " + (i + 1)));
    var weight = parseFloat(prompt("Enter weight in kilograms for person " + (i + 1)));

    function calculateBMI(height, weight) {
        var heightInMeters = height / 100;
        var bmiCal = weight / (heightInMeters * heightInMeters);
        return bmiCal;
    }

    var bmi = calculateBMI(height, weight);

    alert("Person " + (i + 1) + ": Your BMI is " + Math.floor(bmi));

    if (bmi >= 18.5 && bmi <= 24.9) {
        alert("You are fit and fine.");
    } else if (bmi > 24.9) {
        alert("You are unhealthy and overweight.");
    } else {
        alert("You are underweight.");
    }
}
```

### Example 18 - Practice Section: Money Calculation
```javascript
// Practice Section: Money Calculation

var moneyByUser = prompt("Enter Money to buy a milk");
var milkPrice = 40;
var numberOfBottles = Math.floor(moneyByUser / milkPrice);
var remainingMoney = Math.floor(moneyByUser % milkPrice);
alert("Buy " + numberOfBottles + " milk bottles" + " and " + remainingMoney + " rs money is remaining");
```

### Example 19 - Practice Section: Robot Movement
```javascript
// Practice Section: Robot Movement

function main() {
    firstLine();
    secondLine();
    thirdLine();
    forthLine();
    fifthLine();
}

function firstLine() {
    putBeeper();
    moveBeeper();
    moveBeeper();
}

function secondLine() {
    turnLeft();
    move();
    turnLeft();
    move();
    putBeeper();
    moveBeeper();
    move();
    turnRight();
}

function thirdLine() {
    move();
    putBeeper();
    turnRight();
    moveBeeper();
    moveBeeper();
}

function forthLine() {
    turnLeft();
    move();
    turnLeft();
    move();
    putBeeper();
    moveBeeper();
    move();
}

function fifthLine() {
    turnRight();
    move();
    turnRight();
    putBeeper();
    moveBeeper();
    moveBeeper();
}

function moveBeeper() {
    move();
    move();
    putBeeper();
}
```

### Example 20 - Practice Section: BMI Calculation Function
```javascript
// Practice Section: BMI Calculation Function

var numPeople = parseInt(prompt("Enter the number of people you want to calculate BMI for"));

for (var i = 0; i < numPeople; i++) {
    var height = parseFloat(prompt("Enter height in meters for person " + (i + 1)));
    var weight = parseFloat(prompt("Enter weight in kilograms for person " + (i + 1)));

    function calculateBMI(height, weight) {
        var heightInMeters = height / 100;
        var bmiCal = weight / (heightInMeters * heightInMeters);
        return bmiCal;
    }

    var bmi = calculateBMI(height, weight);

    alert("Person " + (i + 1) + ": Your BMI is " + Math.floor(bmi));

    if (bmi >= 18.5 && bmi <= 24.9) {
        alert("You are fit and fine.");
    } else if (bmi > 24.9) {
        alert("You are unhealthy and overweight.");
    } else {
        alert("You are underweight.");
    }
}
```









