Bonfire - Intermediate JavaScript Algorithm

Sum of two numbers and all numbers between them
````
function range(arr) {
  var a = [arr[0]]; 
  var b = arr[0];
  while (b<arr[1]) {
    b += 1;
    a.push(b);
  }
  return a;
}

function arrange(arr) {
  arr = arr[0] < arr[1] ? arr : [arr[1], arr[0]];
  return arr;
}

function sumAll(arr) {
  arr = arrange(arr);
  console.log('Arranged array is ' + arr);
  var r = range(arr);
  console.log('Range is ' + r);
  sum = r.reduce(function(prev, curr){ 
    return prev + curr;
  });
  console.log('Sum is ' + sum);
  return sum;
}

sumAll([1, 4]);
// 10
````

Compare two arrays and return a new array with any items 
only found in one of the original arrays

````
````
