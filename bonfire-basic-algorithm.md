Bonfire section


Reverse a string str:
````
str.split().reverse().join();
````


Factorialize a number:

Return the factorial of the integer n
````
var arr = Array.apply(null, Array(num)).map(function(a, b) {return b +1;});
factorial = arr.reduce(function(prod, n) {return prod * n}, 1);
````


Check for palindromes in string str:
````
var s = str.toLowerCase().replace(/ /g, '').replace(/[^a-z0-9]+/g, '');
var rev = s.split('').reverse().join('');
return rev === s;
````


Find the longest word in a string str:
````
var arr = str.split(' ');
var max = 0;
arr.map(function(a){if (a.length > max){max = a.length; str = a};});
return str.length;
````


Title case a sentence:
````
var s = str.toLowerCase().split(' ');
var cap = [];
s.map(function(word){cap = cap.concat(word.replace(word.charAt(0), word.charAt(0).toUpperCase()));});
str = cap.join(' ');
return str;
````


Return largest numbers in arrays:

Return an array consisting of the largest number from each provided sub-array
````
arr.map(function(a){return Math.max.apply(Math, a)});
````


Confirm the ending:

Check if a string str ends with the given target string
````
str = target === str.substr(- target.length);
````


Repeat a string:

Repeat a given string str n times. Return an empty string if n is a negative number
````
if(num > 1){
  str = str.repeat(num);
} else {
  str = '';
}
````


Truncate a string:

Truncate a string str if it is longer than maximum string length.
Return the truncated string with a "..." ending.

````
  if(num >= str.length){
    str;
  } else if(num <= 3){
    str = str.slice(0,num).concat('...');
  } else {
    str = str.slice(0,num-3).concat('...');
  }
````


Chunky monkey:

Split an array arr into groups the length of size and return them as a multidimensional array.

````
  var new_arr = [];
  var repeats = Math.ceil(arr.length / size);
  for (var i = 0; i < repeats; i++) {
    new_arr.push(arr.splice(0,size));    
  }
````


Slasher Flick:

Return the remaining elements of an array after chopping off n elements from the head.
````
arr.splice(0,n);
````


Mutations:

Return true if the string in the first element of the array contains all of the letters of the string in the second element of the array.
````
  var s = arr[0].toLowerCase();
  var wordArray = arr[1].toLowerCase().split('');

  for (i = 0; i < wordArray.length; i++) { 
    if (s.indexOf(wordArray[i]) === -1) { 
      arr = false;
      break;
    } else {
      arr = true;
    }
  };
````


Falsy Bouncer:

Remove all falsy values from an array.
Falsy values in javascript are false, null, 0, "", undefined, and NaN.

````
  arr = arr.filter(function(n){ 
    n = new Boolean(n); 
    return n.toString() === 'true';
  })
````


Seek and Destroy:

Given an initial array arr followed by one or more arguments, remove all elements from arr that are of the same value as these arguments.

````
  var args = Array.prototype.slice.call(arguments);
  arr = args.shift();
  for(i=0; i < args.length; i++) {
    arr = arr.filter(function(a){ return a !== args[i]});
  }
````

Where do I belong:

Return the lowest index at which a value (second argument) should be inserted into a sorted array (first argument).
````
  arr.push(num);
  console.log(arr);
  arr = arr.sort(function(a,b){ return a - b });
  console.log(arr);
  return arr.indexOf(num);
````
