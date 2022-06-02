## Project Purpose and Components
The purpose of this second project was mainly to get students thinking about editing their code, so the main task was refactoring given code.

## What I Learned
This project was really good for getting me to think about the most efficiant, clean, organized, and modern way to write my code. It also gave me the tools to work on revamping older code, or to work with a team who might have different styles.

## Code
### p2-expressions.js
/*
    CIT 281 Project 2
    Name: Sophia Lynsky
*/

// Returns a random number between min (inclusive) and max (exclusive)

const getRandomInteger = function(min, max) {
    return Math.floor(Math.random() * (max - min) + min);
}

const alphabet = "abcdefghijklmnopqrstuvwxyz".split("");

//let result = "";

//let lengthOfOutputString = getRandomInteger(5, 26);

//Returns a random letter from the alphabet constant

const getRandomLetter = function() {
    let letter = getRandomInteger(0,alphabet.length);
    return alphabet[letter];
}


const getRandomString = function(minLength, maxLength) {
    let stringLength = Math.floor(Math.random() * (maxLength - minLength) + minLength);
    let text = ""
    for (i=0; i<stringLength; i++) {
        text += getRandomLetter();
    }
    return text;
}

/*
for (let i = 0; i < lengthOfOutputString; i++) {
    result += getRandomLetter();
}
*/
console.log(getRandomString(10,20));

const getSortedString = function(string) {
    return string.split("").sort().join("")
}

### p2-random.js
/*
    CIT 281 Project 2
    Name: Sophia Lynsky
*/

// Returns a random number between min (inclusive) and max (exclusive)
function getRandomInteger(min, max) {
    return Math.floor(Math.random() * (max - min) + min);
}

const alphabet = "abcdefghijklmnopqrstuvwxyz".split("");

//let result = "";

let lengthOfOutputString = getRandomInteger(5, 26);

//Returns a random letter from the alphabet constant
function getRandomLetter() {
    let letter = getRandomInteger(0,alphabet.length);
    return alphabet[letter];
}

function getRandomString(minLength, maxLength) {
    let stringLength = Math.floor(Math.random() * (maxLength - minLength) + minLength);
    let text = ""
    for (i=0; i<stringLength; i++) {
        text += getRandomLetter();
    }
    return text;
}

/*
for (let i = 0; i < lengthOfOutputString; i++) {
    result += getRandomLetter();
}
*/
console.log(getRandomString(10,20));

function getSortedString(string) {
    return string.split("").sort().join("")
}

### [Home Page](https://slynsky.github.io)

