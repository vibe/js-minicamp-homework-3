#### Objects
* Objects are a way to encapsulate data and functions (properties & methods) into a single data type. Think of objects just as you would any other object in the real world. For example take a Cook for example, they can be viewed as an object with data and functions. For example, a cook can have a name and functions so they can do their job like "starting the stove", "measuring ingridents. 

```javascript
var cook = {
    name: 'Cook Awesome Joe',
    startStove() {
        console.log("starting stove");
    }
}

```

#### Properties

* Properties are regular data types but instead of being standalone they are attached to an object. These properties can hold values and state related to an object. 

```javascript
var obj = {
    propertyOne: 'Awesome prop',
    propertyTwo: 2,
}

console.log(obj.propertyOne);
```

#### Methods

* Methods are functions that attached to objects, these functions inside the object in turn become the `methods`.

```javascript
var obj = {
    methodOne() {
        console.log("Calling a method")
    }
}

obj.methodOne();
```

#### For in
* `for in` are loops that can be utilized to loop over every property of an object.

```javascript
var obj = {
    propertyOne: "prop 1",
    propertyTwo: "prop 2"
}
for(key in obj) {
    console.log(key, " : ", obj[key])
}

//propertyOne  :  prop 1
//propertyTwo  :  prop 2

``` 


#### Dot notation vs bracket notation
* Dot notation and bracket notation are two ways to access properties and methods from an object. Using bracket notation you can use it to access variables that use forbidding keys

```javascript

var obj = {
    propertyOne: "Awesome prop",
    methodName() {
        console.log("Awesome method calling")
    }
}

obj.propertyOne;
obj[propertyOne]

obj.methodName()
obj[methodName]()

```