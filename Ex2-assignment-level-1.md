# Data Structure Assignments

## writeCode

Follow the instruction and write code just below the instruction.

- Create a variable named `character` using `let` and assign a value of blank object to it.
```js
// your code goes here
let character = {};
```

- Go to this [link](https://awoiaf.westeros.org/index.php/List_of_characters) and choose any charactor you like and click on the link. For example [Arya Stark](https://awoiaf.westeros.org/index.php/Arya_Stark)

```js
// your code goes here
```

- Re-assign the value of `charator` variable to and object with the key `charatorName` and value of the first name of your charactor. example "Arya"
//FEEDBACK: `charator` should be `character`

```js
// your code goes here
character.characterName = "Arya";
```

- A variable named `age` is predeined to 20. Add a new key named `character-age` with the value of age variable.

```js
let age = 20;
// your code goes here
character["character-age"] = age;
```

- Add a new key named `sur name` with the vlaue of the surname of the cahractor i.e "Stark"

```js
// your code goes here
character["sur name"] = "Stark";
```

- Add a new key named `title` with the value title of the charactor (you will find in the right side bar) i.e "Lady of Winterfell"

```js
// your code goes here
character['title'] = "Lady of Winterfell";
```

- Add another property named `greet` and value should be a function when called should alert `I am [NAME HERE] and my title is [TITLE HERE]`.

```js
// your code goes here
character.greet = function(){
  alert(`I am ${this.characterName} and my title is ${this.title}`)
}
```

- Add a new property named `isFemale` and value will be either `true` or `false` according to the charactor.

```js
// your code goes here
character.isFemale = true;
```

- Change the method `greet` to now alert `He is [NAME HERE] and his title is [TITLE HERE]` if the character is male or else `She is [NAME HERE] and her title is [TITLE HERE]`. You should use `if/else`.

```js
// your code goes here
character.greet = function(){
  let designation = this.isFemale ? "She" : "He";
  let hisHer = this.isFemale ? "her" : "his"; 
  alert(`${designation} is ${this.characterName} and ${this.hisHer} title is ${this.title}`);
}
```

- Add a new method (function inside objects are called methods) named change gender. When called should be able to flip the value of `isFemale`.

```js
// your code goes here
character.changeGender = function(){
  character.isFemale = !character.isFemale;
}
```

- Check by calling `greet` and see if the message changed or not.

```js
// your code goes here
character.greet();
```

- `let keyName = "playedBy";`- Add a new key with the value stored in `keyName` variable the value of the Played by in right side bar. (use the variable name to do this)

```js
// your code goes here
character[keyName] = "Maisie Williams";

```

- `alert` the value of key stored in `keyName` variable.

```js
// your code goes here
alert(character[keyName]);
```

- Write a `for..in` loop to `console.log()` all the key of the object character.

```js
// your code goes here
for(let key in character){
  console.log(key);
}

```

- Write a `for..in` loop to log the all the key value pair seperated by `-` like `charactorName - Arya`.

```js
// your code goes here
for(let key in character) {
  console.log(`${key} - ${character[key]}`);
}
```

- Using the function `console.log log` the value of the key `42`.

```js
// your code goes here
console.log(character[42]);
```

- Add a key in your object with the value of the variable `city`. The value of the key should be `true`.

```js
// your code goes here
let city = "Dharamshala";
character[city] = true;
```

```js
var city = prompt("Enter the city name you visited last time.");

// your code goes here
character[city] = true;

```

- Uisng console.log log the value of the key defined above.

```js
// your code goes here
console.log(character[city]);
```

-. Can you define a key of `let or var` in any object? Reason.

```js
// your code goes here
// Yes keys can be any of the reserved words so let or var can be used.
```

## writeTextAnswer

```js
let keyValue = "username";
let charactor = {
  username: "arya"
};
// 1.
console.log(charactor["keyValue"]);
// 2.
console.log(charactor[keyValue]);
```

- What will be the output of 1 and 2.
// Output of 1 : undefined and Output of 2 : "arya" ;

- Why are they different.
// In the first case we are trying to search keyname as "keyValue" which is not existing in the object so we get undefined and in the second case we are trying to get key with value as "username" which is "arya"

- Can I use `.` dot notation to access the value (using variable name). Write reason.
//No internally if we try to access variable with . notation it will try to search "variablename" in string form in the object.

- What is the difference between `.` dot notation and `[]` bracket notation. Example
//"." notation is used to access value whereas '[]' notation is used to both compute the expression and even access the value.

- What are situation where we use dot notation and bracket notation.
//If we have a spaced string as key or number as key, there we tend to use bracket notation, rest elsewhere we can use "." notation for accessing the value.

## writeQuiz

Whic statement is true?

- [true] You can replace all dot notation with bracket notation.
- [ ] You can replace all bracket notation with dot notaiton.

## Array-writeCode

- Create an array named colors that contains five different names of colors as strings.

```js
// your code goes here
let colors = ["green","yellow","red","black","orange"];
```

- Access the first color in the array and print it to the console using `console.log()`

```js
// your code goes here
console.log(colors[0]);
```

- Now do the same with the third color in the list.

```js
// your code goes here
console.log(colors[2]);
```

- Re-assign the value of the last color in array to "ultraviolet".

```js
// your code goes here
colors[4] = "ultraviolet"
```

- Re-assign the value of the last color in array to "ultraviolet". This time use `arr.length` property to know the length of the array.

```js
// your code goes here
colors[colors.length - 1] = "ultraviolet"
```

- Create a new variable called fourthColor and set it equal to the fourth color in the list.

```js
// your code goes here
let fourthColor = colors[3];
```

- Add another color to the end of the list. (use array method called push)

```js
// your code goes here
colors.push("white");
```

- Add another color to the beginning of the list. (use unshift)

```js
// your code goes here
colors.unshift("tomatored");
```

- Print the length of the array to the console with `console.log()`

```js
// your code goes here
console.log(colors.length);
```

- Remove the last color from the end of list, and then print the length of the array to the console one more time.

```js
// your code goes here
colors.pop();
console.log(colors.length);
```

- Write a for loop to iterate through every color in the array and print each color's value to the console.(use for loop)

```js
// your code goes here
for(let i = 0; i < colors.length; i++) {
  console.log(colors[i]);
}
```

- Write a for loop to iterate through every color in the array and print each color's value to the console.(use for..in)

```js
// your code goes here
for(let color in colors) {
  console.log(colors[color])
}
```

- Write another loop to display the value and key of array in this format. `The value for index 0 is Red` for each value.

```js
// your code goes here
for(let i = 0; i < colors.length; i++) {
  console.log(`The value for index ${i} is ${colors[i]}`);
}
```

- Create a variable named `lastColor` that will always point to the last element of the colors array, no matter how many colors are in the list.

```js
// your code goes here
let lastColor = colors[colors.length - 1];
```

- Add a new color `tomato` to the index 45. And check the length of the array. Use `console.log` to print.

```js
// your code goes here
colors[45] = "tomato";
console.log(colors.length);
```

## writeTextAnswer

What will be the output if you access index greater than the length of the array. Like array length is 10 and `arr[11]`. Same with object if you access the key that doesnot exist.
//We will get undefined.
