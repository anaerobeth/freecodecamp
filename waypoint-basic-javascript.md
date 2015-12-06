Waypoint: Basic JavaScript

Get the last letter of a string
````
var lastLetterOfLastName = lastName[lastName.length -1];
````

Get the value of the third-to-last letter
````
var thirdToLastLetterOfFirstName = firstName[firstName.length - 3];
````

Add new properties to existing JavaScript objects
````
var myDog = {}
myDog.bark = 'woof';
````

Use a for loop to work to push the values 1 through 5 onto myArray
````
for (var i = 1; i < 6; i++) {
  myArray.push(i);
  }
````

Delete the "tails" property from myDog.
````
delete myDog.tails;
````

Selecting all the occurrences of the word 'and'
````
var expression = /and/gi;
````

Select the number of numbers in the string
````
var expression = /\d+/g;
````

Count the number of non-whitespace characters
````
var expression = /\S/g;
````
