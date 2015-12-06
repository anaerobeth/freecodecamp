Waypoint - Object Oriented JavaScript


Make unique objects by passing parameters
````
var Car = function(wheels, seats, engines) {
  this.wheels = wheels;
  this.seats = seats;
  this.engines = engines;
};
var myCar = new Car(6, 2, 2);
````

Map
````
var newArray = oldArray.map(function(val){
  return val + 3;
});
````

Reduce
````
var singleVal = array.reduce(function(previousVal, currentVal) {
  return previousVal + currentVal;
}, 0);
````

Filter
````
var newArray = oldArray.filter(function(val){
  return val <= 5;
});
````

Sort
````
// ascending
array.sort(function(a, b){
  return a - b;
});

// descending
return b - a;
````



