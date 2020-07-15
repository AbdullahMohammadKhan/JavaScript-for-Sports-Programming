# JavaScript-for-Sports-Programming
### Loop
https://www.hackerrank.com/challenges/js10-loops/topics/javascript-loops

### Strings
https://www.hackerrank.com/challenges/js10-try-catch-and-finally/topics/javascript-strings

### Try,Catch, Finally,Throw
https://www.hackerrank.com/challenges/js10-try-catch-and-finally/topics/javascript-strings

```javascript
function reverseString(s) {
  
  try{
    // Can be chained, but it damages readability
    console.log(s.split("").reverse().join("")) 
  }
  catch(e){
    console.log(e.message); // Use .message, or you'll get more than expected.
    console.log(s);
  }

}


//Another one:
if(a > 0){
        return 'YES';
    }
    else{
        throw (a === 0 ? new Error('Zero Error') : new Error('Negative Error'));
    }
    //or,
    function isPositive(a) {
    if (a > 0) { return "YES" };
    throw Error (a ? "Negative Error" : "Zero Error");
}
```

### RegEx
https://www.hackerrank.com/challenges/js10-regexp-1/topics/javascript-regex



### Classes
https://www.hackerrank.com/challenges/js10-inheritance/topics/javascript-classes
https://www.hackerrank.com/challenges/js10-class/topics/javascript-classes
```
class Polygon{
    constructor(sides){        
        this.sides = sides
    }
    perimeter() {
        return this.sides.reduce(function add(a,b){return a+b;})
    } 
}
```
```
/*
 *  Write code that adds an 'area' method to the Rectangle class' prototype
 */
    Rectangle.prototype.area = function() {
        return(this.w*this.h);
    };
/*
 * Create a Square class that inherits from Rectangle and implement its class constructor
 */
   
    class Square extends Rectangle {
        constructor(s) {
            super(s);
            this.h = s;
            this.w = s;
        }
    };
  ```
    
    
   ### JS Button Basics
   https://www.hackerrank.com/challenges/js10-create-a-button/topics/javascript-button-basics
   
   ### function
   https://www.hackerrank.com/challenges/js10-function/topics/javascript-function
   
   
   
   ### Recuersive function
   https://www.hackerrank.com/challenges/js10-function/topics/recursion
   ```
   function factorial(n){
    if(n === 0){
        return 1;
    } else{
        return n * factorial(n-1);
    }
}
//or
const factorial = n => (n === 0 ? 1 : n * factorial(n - 1));
```
### variable declaration
https://www.hackerrank.com/challenges/js10-let-and-const/topics/javascript-let-const-var


### if-else

https://www.hackerrank.com/challenges/js10-if-else/topics/javascript-conditional-if-else
```
function getGrade(score) {
    return 'FEDCBA'[parseInt((score > 0 ? score - 1 : 0) / 5)];
}
```

### switch
https://www.hackerrank.com/challenges/js10-switch/topics/javascript-conditional-switch
```
function getLetter(s) {
    let letter;
    // Write your code here
    switch (true) {
        case 'aeiou'.includes(s[0]):
            letter = 'A';
            break;
        case 'bcdfg'.includes(s[0]):
            letter = 'B';
            break;
        case 'hjklm'.includes(s[0]):
            letter = 'C';
            break;
        case 'npqrstvwxyz'.includes(s[0]):
            letter = 'D';
            break;
    }
    return letter;
}
```


### Arrays
https://www.hackerrank.com/challenges/js10-arrays/topics/javascript-arrays

```
//finding the second largets number
for (let i = 0; i < nums.length; i++) {


    if (nums[i] > first) {
        second = first;
        first = nums[i]
    }

    if (nums[i] > second && nums[i] < first) {
        second = nums[i];
    }
}


return second;
```

### objects
https://www.hackerrank.com/challenges/js10-objects/topics/javascript-objects

### iterating over arrays
https://www.hackerrank.com/challenges/js10-count-objects/topics/javascript-iterating-over-arrays
```
function getCount(objects) {
    return objects.filter(function(o){return o.x==o.y}).length
}
```
### template literals
https://www.hackerrank.com/challenges/js10-template-literals/topics/javascript-template-literals
```
function sides(literals, ...expressions) {
    // ES6 allows destructuring of arrays into multiple variables
    const [a, p] = expressions;
    // Perform this operation only once and assign to variable
    const root = Math.sqrt((p*p)-(16*a))
    const s1 = (p + root)/4;
    const s2 = (p - root)/4;
    // s2 will always be smaller because of the (-/+) above
    return ([s2, s1]);
}
```
### Arrow functions
https://www.hackerrank.com/challenges/js10-arrows/topics/javascript-arrow-functions

```
For better understanding .. every new method is a modification of previous method.. This is how it helped me understand the arrow function.

//method 1

function modifyArray(nums) {
    var something = function(n){
        if(n%2==0)
            return n*2;
        else
            return n*3;
    }
    var newArray = nums.map(something);
    return newArray;
    
}
// method 2

function modifyArray(nums) {
    var something = function(n){
        var a = (n%2==0) ? n*2: n*3;
        return a;
    }
    var newArray = nums.map(something);
    return newArray;
    
}
//method 3

function modifyArray(nums) {
    var something = n => n = (n%2==0) ? n*2: n*3;
    var newArray = nums.map(something);
    return newArray;
    
}
//method 4

function modifyArray(nums) {
    var newArray = nums.map(n => n = (n%2==0) ? n*2: n*3);
    return newArray;
    
}
//method 5

function modifyArray(nums) {
    return nums.map(n => n = (n%2==0) ? n*2: n*3);   
}
```
### bitwise operators
 https://www.hackerrank.com/challenges/js10-bitwise/topics/javascript-bitwise-operators
 
### 
