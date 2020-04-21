## writeTextAnswer

```js
const user = {
  name: "Arya"
};
user.name = "Sansa";
console.log(user.name);
```

- Is the code above is valid or invalid.
- Can we change the variable defined with const. Explain with reason.
- What will be the output and why?
// Code is valid.
// We cannot reassign the variable defined with const, but if an object is defined with const, we can reassign it's properties that is key : value
//Output : "Sansa" , the value has been reassigned.

## writeTextAnswer

1. What will be the value of a, b, x and y.

```js
let x = 10;
let y = "abc";
let a = x;
let b = y;
```

Answer:
//a : 10
//b : "abc"
//x : 10
//y : "abc"

---

2. What will be the value of a, b, x and y.

```js
var x = 10;
var y = "abc";
var a = x;
var b = y;
a = 5;
b = "def";
```

Answer:
// a : 5
// b : "def"
// x : 10
// y : "abc"

---

3. What will be the value of `arr` and `arrCopy`.

```js
var arr = [1];
var arrCopy = arr;
arr.push(2);
```

Answer:
// arr = [1, 2]
// arrCopy = [1, 2]

4. What will be the output and explain the reason.

```js
let obj = { name: "Arya" };
obj = { surname: "Stark" };
let newObj = { name: "Arya" };
let user = obj;
let arr = ["Hi"];
let arr2 = arr;
//FEEDBACK : I think arr2 should have been arr1
```

- `[10] === [10]` //False
- What is the value of obj? // answer : obj is { surname: "Stark" };
- `obj == newObj` //false
- `obj === newObj`//false
- `user === newObj`//false
- `user == newObj` //faslse
- `user == obj` //true
- `arr == arr1` //false
- `arr === arr1`//false

5. What's will be the value of `person1` and `person2` ? Explain with reason.

```js
function personDetails(person) {
  person.age = 25;
  person = { name: "John", age: 50 };
  return person;
}
var person1 = { name: "Alex", age: 30 };
var person2 = personDetails(person1);
console.log(person1);
// person1 {name:"Alex",age:25}
console.log(person2);
//person2 { name: "John", age: 50 };
```

```js
var brothers = ["Bran", "John"];
var user = {
  name: "Sansa"
};
user.brothers = brothers;
brothers.push("Robb");
console.log(user.brothers === brothers); //1. output true
console.log(brothers.length === brothers.length); //2. true output
```

## writeCode

What are the different ways of cloning an object? Clone below object.

```js
let charactor = {
  charactorName: "Sansa",
  sisters: 1,
  brothers: 4
};
let cloneCharactorWay1 = {...charactor};
let cloneCharactorWay2 = Object.assign(charactor);
```

## writeTextAnswer

```js
let brothers = ["John", "Bran", "Robb"];
let house = "Stark";
let user = {
  name: "Arya",
  house: house,
  brothers: brothers
};

let user2 = {
  name: "Arya",
  house: house,
  brothers: brothers
};

let user3 = {
  name: "Arya",
  house: "Stark",
  brothers: ["John", "Bran", "Robb"]
};
user.house === user2.house; // output: true
user.house == user2.house; // output: true
user.brothers === user2.brothers; // output:  true
user.brothers == user2.brothers; // output: true
user.name == user2.name; // output: true
user.name === user2.name; // output:  true
user.brothers == user3.brothers; // output: false
user.brothers === user3.brothers; // output:  false
user.house === user2.house; // output true
user.house === user3.house; // output true
user.brothers[0] === user2.brothers[0]; // output  true
user.brothers[0] === user3.brothers[0]; // output true
```
