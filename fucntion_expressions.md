# Function Expressions

This function builds in memory immediately when the program loads.

```text
function diffOfSquares (a, b) {
    return a*a - b*b;
    }
```

Function expressions build only when the program reaches their line of code.

```text
var diff = function (a, b) {
 return a*a - b*b;
};

diff( 9, 5 ); // This is how we call the function
```

A variable that holds a function can be passed into other functions. Function expressions can give flexibility in choosing which functionality to build.

```text
var greeting;
var newCustomer =  false;

if (newCustomer) {
  greeting = function() {
    alert("Welcome first timer!) {
    };
  } else {
    alert("Welcome back beloved customer");
  };
}
closeTerminal (greeting);
function closeTerminal(message){
  message();
}
```

