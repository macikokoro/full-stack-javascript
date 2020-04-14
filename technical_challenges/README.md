# Technical Challenges

The Square of a number

```text
var square = function(x, y) {
  y = x;
  return x * y;
};

console.log(square(8));
```

Exponential

```text
//Write a function that calculates x to the power of z

function power(num, exp) {
  var value = num;

  for (var i = 1; i < exp; i = i + 1) {
    value = value * num;
    //Keeps a running total
  }
  return value;
}

var value = power(2, 3);
console.log(value);

// A loop is exactly like an exponent or multipliying a
// number by itself for a certain amount of times.
// a loop executes one of more statements for a certain amount
// of times.
```

Reverse a string

```text
var string = "Batman";

var reverse = function (string) {
  var newString = "";
  for (var i = string.length; i >= 0; i--) {
  newString += string.charAt(i);
  }
  return newString;
};

console.log(reverse(string));
```

Multiply Array

```text
var numArray = [2, 3];

function multiply(numArray) {
  var sum = 1;
  for(var i = 0; i < numArray.length; i++){
    sum = sum * numArray[i];
  }
  return sum;
}

console.log(multiply(numArray));
```

Date

```text
/*Write a function that converts user entered date formatted as M/D/YYYY to a
format required by an API (YYYYMMDD). The parameter "userDate" and the return value are strings.*/

var userDate = "12/31/2014";

function formatDate(userDate) {
  var year = userDate.slice(6, 10);
  var theRest = userDate.slice(0, 5);
  return year + theRest.split('/').join('');
   // format from M/D/YYYY to YYYYMMDD
}

formatDate(userDate);

console.log(formatDate(userDate));
```

Eliminate Duplicates

```text
var numArray = [2, 3, 6, 4, 8, 10, 11, 13, 1, 2, 2, 3,3,3,3];
//sort numbers in order
numArray.sort(function(a, b) {return a-b;});
//empty array to store results
var result = [];
//loop through array
for (var i = 0; i < numArray.length; i++) {
    //compare results
    if (numArray[i + 1] === numArray[i]) {
       //push duplicates
        result.push(numArray[i]);
    }
}
//log the contents of the array
console.log(numArray);
//log the repeating numbers in array
console.log("these numbers repeat: " + result);

//made possible by http://dreaminginjavascript.wordpress.com/
//Eliminating duplicates
function eliminateDuplicates(arr) {
  var i,
      len=arr.length,
      out=[],
      obj={};

  for (i=0;i<len;i++) {
    obj[arr[i]]=0;
  }
  for (i in obj) {
    out.push(i);
  }
  return out;
}


var b=[];


b=eliminateDuplicates(result);
console.log(result);
console.log("array without duplicates " + b);
```

Find the remainder of a number

x - \(z \* y \) x - zy = remainder

