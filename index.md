## Project 2

``` markdown
Goals and Outcomes

  - Gain experience using git via your CLI and Visual Studio Code (VSCode) Source Control
  - Gain experience writing and executing non-web server Node.js JavaScript code
  - Practice refactoring JavaScript code

```

p2-random.js

```rouge
  `/*
    CIT 281 Project 2
    Name: Emily Deng
*/

// will return a single, random, lowercase letter
function getRandomLetter() {

    const alphabet = "abcdefghijklmnopqrstuvwxyz".split("");

    return alphabet[Math.floor(Math.random() * alphabet.length)];
}

// Returns a random number between min (inclusive) and max (exclusive)
function getRandomInteger(min, max) {
    return Math.floor(Math.random() * (max - min) + min);
}

// will return a random length string between 10 and 20 characters
function getRandomString(minLength, maxLength) {
    let length = Math.floor(Math.random() * (maxLength - minLength) + minLength);
    let string = "";
    for (let i = 0; i < length; i++) {
        string += getRandomLetter();
    }
    return string;
}

// return a string in ascending order
function getSortedString(string) {
    return string.split("").sort().join("");
}

console.log(getSortedString(getRandomString(10, 20)));`

```

p2-expressions.js

```rouge
  `/*
    CIT 281 Project 2
    Name: Emily Deng
*/

// will return a single, random, lowercase letter
const getRandomLetter = function() {

    const alphabet = "abcdefghijklmnopqrstuvwxyz".split("");

    return alphabet[Math.floor(Math.random() * alphabet.length)];
}

// Returns a random number between min (inclusive) and max (exclusive)
const getRandomInteger = function(min, max) {
    return Math.floor(Math.random() * (max - min) + min);
}

// will return a random length string between 10 and 20 characters
const getRandomString = function(minLength, maxLength) {
    let length = Math.floor(Math.random() * (maxLength - minLength) + minLength);
    let string = "";
    for (let i = 0; i < length; i++) {
        string += getRandomLetter();
    }
    return string;
}

// return a string in ascending order
const getSortedString = function(string) {
    return string.split("").sort().join("");
}

console.log(getSortedString(getRandomString(10, 20)));`

```

<img src="p2-vscode-diff.png![image](https://user-images.githubusercontent.com/84113983/120712980-2de37b00-c476-11eb-98e2-e5cc9667777a.png" width="715" height="665" />


