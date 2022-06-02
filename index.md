## Project Purpose and Components
The purpose of this second project was mainly to get students thinking about editing their code, so the main task was refactoring given code.

## What I Learned
This project was really good for getting me to think about the most efficiant, clean, organized, and modern way to write my code. It also gave me the tools to work on revamping older code, or to work with a team who might have different styles.

## Code
### p2-expressions.js
/*<br>
    CIT 281 Project 2<br>
    Name: Sophia Lynsky<br>
*/<br>

// Returns a random number between min (inclusive) and max (exclusive)<br>

const getRandomInteger = function(min, max) {<br>
    return Math.floor(Math.random() * (max - min) + min);<br>
}<br>

const alphabet = "abcdefghijklmnopqrstuvwxyz".split("");<br>

//let result = "";<br>

//let lengthOfOutputString = getRandomInteger(5, 26);<br>

//Returns a random letter from the alphabet constant<br>

const getRandomLetter = function() {<br>
    let letter = getRandomInteger(0,alphabet.length);<br>
    return alphabet[letter];<br>
}<br>


const getRandomString = function(minLength, maxLength) {<br>
    let stringLength = Math.floor(Math.random() * (maxLength - minLength) + minLength);<br>
    let text = ""<br>
    for (i=0; i<stringLength; i++) {<br>
        text += getRandomLetter();<br>
    }<br>
    return text;<br>
}<br>

/*
for (let i = 0; i < lengthOfOutputString; i++) {<br>
    result += getRandomLetter();<br>
}<br>
*/<br>
console.log(getRandomString(10,20));<br>

const getSortedString = function(string) {<br>
    return string.split("").sort().join("")<br>
}<br>

### p2-random.js
/*<br>
    CIT 281 Project 2<br>
    Name: Sophia Lynsky<br>
*/<br>

// Returns a random number between min (inclusive) and max (exclusive)<br>
function getRandomInteger(min, max) {<br>
    return Math.floor(Math.random() * (max - min) + min);<br>
}<br>

const alphabet = "abcdefghijklmnopqrstuvwxyz".split("");<br>

//let result = "";<br>

let lengthOfOutputString = getRandomInteger(5, 26);<br>

//Returns a random letter from the alphabet constant<br>
function getRandomLetter() {<br>
    let letter = getRandomInteger(0,alphabet.length);<br>
    return alphabet[letter];<br>
}<br>

function getRandomString(minLength, maxLength) {<br>
    let stringLength = Math.floor(Math.random() * (maxLength - minLength) + minLength);<br>
    let text = ""<br>
    for (i=0; i<stringLength; i++) {<br>
        text += getRandomLetter();<br>
    }<br>
    return text;<br>
}<br>

/*<br>
for (let i = 0; i < lengthOfOutputString; i++) {<br>
    result += getRandomLetter();<br>
}<br>
*/<br>
console.log(getRandomString(10,20));<br>

function getSortedString(string) {<br>
    return string.split("").sort().join("")<br>
}<br>

### [Home Page](https://slynsky.github.io)

