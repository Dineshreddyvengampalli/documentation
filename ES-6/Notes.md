# What is ECMA262?

ECMA262 is a standards that need to be followed to build a scripting languages.javaScript one such scripting language that follows ECMA standards. By learning ECMA262 one can able to create a scripting language using the standards of ECMA262.It is commonly used for client-side scripting language in developing web based applications,websites etc.

## Versions of ECMAscript

### JavaScript ES6:

It is introduced in 2015.It is the second largest enhanced version after ES2015.

### New features in ES6 include :

--> let keyword : let keyword allows us to declare a variable within the blocked scope
example:
	var a = 2
	{
	let a = 5
	}
--> const keyword : const keyword allows us to create a variable that stores the constant value that cannot be changed
--> Arrow functions : This is the easy form of creating functions without using the ‘function’ keyword
example:
let a = (b,c) => b+c
-->  for/of : used to iterate over any iteratable data structure
example:
	let a = [1,2,3,4]
	let sum = 0
	for(let i of a)
	{
	sum = sum+i
	} 
--> Promises
--> rest arguments (...args)
--> map object
--> set object
--> default parameters to the function : function(a,b=19)
--> string.includes() function
--> string.startsWith() function
--> string.endsWith() function
--> Array.from() : Array.from(“dinesh”) forms an array : [‘d’,’i’,’n’,’e’,’s’,’h’]

## Browser compactibility of ES6