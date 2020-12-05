[![General Assembly Logo](https://camo.githubusercontent.com/1a91b05b8f4d44b5bbfb83abac2b0996d8e26c92/687474703a2f2f692e696d6775722e636f6d2f6b6538555354712e706e67)](https://generalassemb.ly)

# Javascript Homework

1.  Variables
    - https://www.youtube.com/watch?v=cXUWYZXru6o (7 min video)

2.  Conditions
    - https://blog.codeanalogies.com/2018/06/18/javascript-booleans-explained-by-going-to-court/ (reading)


## Assignment Operator
Without running the following code, try to determine:

```js
let a = 1;
let b = 'bongos';
let c = true;

a = b;
b = c;
c = a;
```

### Your solution here:
1.  What is `a`?
```
a is bongos
```
2.  What is `b`?
```
b is true
```
3.  What is `c`?
```
c is bongos // because var of `a` override in line 20.
```

## Concatenation
Use the `+` operator to concatenate these strings together within a `console.log()`: "Please", "squeeze", "the", "cheese". Make sure there are spaces in-between each word.

```js
const firstWord = "Please";
const secondWord = "squeeze";
const thirdWord = "the";
const fourthWord = "cheese";
```
Result should be:
```js
"Please squeeze the cheese"
```

### Your solution here:
4.  Fill in the `console.log()`?
```js
console.log(firstWord+" "+secondWord+" "+thirdWord+" "+fourthWord);
```

Output a console log `The sum of 5 and 10 is 15` where the values for 5 and 10 are saved to variables, and where 15 comes from those variables being summed.
```js
const num1 = 5;
const num2 = 10;
```

### Your solution here:
5.  How can we make `num3` equal to the sum of `num1` and `num2`?
```js
const  num3 = num1 + num2;
```
6.  Use variables `num1`, `num2` and `num3` to fill in the `console.log()` to complete the sentence: 

>The sum of 5 and 10 is 15

```js
console.log("The sum of "+num1+" and "+num2+" is "+num3);
```

## Comparisons
By just looking at the following expressions, determine in your mind whether or not each will evaluate to true or false
```
a) 999 > 999  
b) 999 === 999 
c) 999 !== 999
d) -5 >= -4   
e) 100 <= -100 
f) 20 + 5 < 5 
g) 81 / 9 === 9 
h) 9 !== 8 + 1  
```
### Your solution here:
7.  Write `true` or `false` based on the list above
```
a) false
b) true
c) false
d) false
e) false
f) false
g) true
h) false
```

## Conditionals
Declare a variable equal to a number 0 to 100

Write a conditional statement that...
- If it is a multiple of 3, print “Fizz” instead of the number.
- If it is a multiple of 5, print “Buzz” instead of the number.
- If it is a multiple of both 3 and 5, print “FizzBuzz” instead of the number.
- Otherwise, print the number

### Your solution here:
8.  Write your javascript solution below
```js

let num = 50;

if(num % 3 == 0 && num % 5 == 0){

	num = "FizzBuzz";
	console.log(num);

}else if(num % 3 == 0){

    num = "Fizz";
	console.log(num);

}else if(num % 5 == 0){
    num = "Buzz";
	console.log(num);

}else{

	console.log("The number is "+num+" .");
}


```



## Array Practice

Using 

### What's in Your Closet?

Below, we've given you examples of Kristyn and Thom's closets modeled as data in JavaScript.

```javascript
const kristynsCloset = [
	'left shoe',
	'cowboy boots',
	'right sock',
	'GA hoodie',
	'green pants',
	'yellow knit hat',
	'marshmallow peeps',
];

// Thom's closet is more complicated. Check out this nested data structure!!
const thomsCloset = [
	[
		// These are Thom's shirts
		'grey button-up',
		'dark grey button-up',
		'light blue button-up',
		'blue button-up',
	],
	[
		// These are Thom's pants
		'grey jeans',
		'jeans',
		'PJs',
	],
	[
		// Thom's accessories
		'wool mittens',
		'wool scarf',
		'raybans',
	],
];
```

1. What's Kristyn wearing today? Using bracket notation to access items in `kristynsCloset`, log the sentence "Kristyn is rocking that " + _the third item in Kristyn's closet_ + " today!" to the console.


2. Kristyn can't find her left shoe. Remove this item from her closet and save it to a variable named `kristynShoe`.


3. Kristyn just bought some sweet shades! Add `"raybans"` to her closet **after `"yellow knit hat"`.**


4. Kristyn spilled coffee on her hat... modify this item to read `"stained knit hat"` instead of yellow.


5. Put together an outfit for Thom! Using **bracket notation**, access the first element in Thom's `shirts` array.


6. In the same way, access one item from Thom's pants array.


7. Access one item from Thom's accessories array.


8. Log a sentence about what Thom's wearing. Example: `"Thom is looking fierce in a grey button-up, jeans and wool scarf!"`


9. Get more specific about what kind of PJs Thom's wearing this winter. Modify the name of his PJ pants to `Footie Pajamas`.


### After finishing all the steps place your solution here:

Write your javascript solution below
```js
// 1
console.log("Kristyn is rocking that "
+kristynsCloset[2]+" today!");

// 2
let kristynShoe = kristynsCloset.shift(); //Note: all upcoming answers are same waterflow of the requirements. execute in order of req.
console.log(kristynsCloset);

// 3
kristynsCloset.splice(5 , 0 , "raybans"); 
console.log(kristynsCloset);

// 4
kristynsCloset[4] = "stained knit hat"; 
console.log(kristynsCloset);

// 5
console.log(thomsCloset[0]);

// 6
console.log(thomsCloset[1][1]); //Thom's pants >> jeans.

// 7
console.log(thomsCloset[2][0]); //Thom's accessories >> wool mittens.

// 8
console.log("Thom is looking fierce in a "+thomsCloset[0][0]+", "+thomsCloset[1][1]+" and "+thomsCloset[2][1]+"!");

// 9
thomsCloset[1][2] = "Footie Pajamas";
console.log(thomsCloset[1]);
```

## Homework Submission
https://git.generalassemb.ly/seir-alahsa/w01d01/blob/master/notes/note_w01d01.03_hw_submission/note_w01d01-homework-submission.md

# Additional Resources
- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures
- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array#
- https://javascript.info/array
- https://javascript.info/array-methods
- https://javascript.info/variables
- https://javascript.info/types
- https://javascript.info/operators
- https://javascript.info/comparison
- https://javascript.info/ifelse
- https://javascript.info/logical-operators

---

_Copyright 2020, General Assembly Space. Licensed under [CC-BY-NC-SA, 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)_