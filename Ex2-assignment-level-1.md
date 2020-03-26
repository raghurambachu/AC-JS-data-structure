# Data Structure Assignments

## writeCode

Follow the instruction and write code just below the instruction.

- Create a variable named `character` using `let` and assign a value of blank object to it.
- Go to this [link](https://awoiaf.westeros.org/index.php/List_of_characters) and choose any charactor you like and click on the link. For example [Arya Stark](https://awoiaf.westeros.org/index.php/Arya_Stark)
- Re-assign the value of `charator` variable to and object with the key `charatorName` and value of the first name of your charactor. example "Arya"
- Add a new key named `surName` with the vlaue of the surname of the cahractor i.e "Stark"
- Add a new key named `title` with the value title of the charactor (you will find in the right side bar) i.e "Lady of Winterfell"
- Add another property named `greet` and value should be a function when called should alert `I am [NAME HERE] and my title is [TITLE HERE]`.

- Add a new property named `isFemale` and value will be either `true` or `false` according to the charactor.
- Change the method `greet` to now alert `He is [NAME HERE] and his title is [TITLE HERE]` if the character is male or else `She is [NAME HERE] and her title is [TITLE HERE]`. You should use `if/else`.
- Add a new method (function inside objects are called methods) named change gender. When called should be able to flip the value of `isFemale`.
- Check by calling `greet` and see if the message changed or not.
- `let keyName = "playedBy";`- Add a new key with the value stored in `keyName` variable the value of the Played by in right side bar. (use the variable name to do this)
- `alert` the value of key stored in `keyName` variable.
- Write a `for..in` loop to `console.log()` all the key of the object character.
- Write a `for..in` loop to log the all the key value pair seperated by `-` like `charactorName - Arya`.

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
- Why are they different.
- Can I use `.` dot notation to access the value (using variable name). Write reason.
- What is the difference between `.` dot notation and `[]` bracket notation. Example
- What are situation where we use dot notation and bracket notation.

## writeQuiz

Whic statement is true?

- [ ] You can replace all dot notation with bracket notation.
- [ ] You can replace all bracket notation with dot notaiton.
