# Disemvowel-Trolls

##

## Problem

Description:
Trolls are attacking your comment section!

A common way to deal with this situation is to remove all of the vowels from the trolls' comments, neutralizing the threat.

Your task is to write a function that takes a string and return a new string with all vowels removed.

For example, the string "This website is for losers LOL!" would become "Ths wbst s fr lsrs LL!".

Note: for this kata y isn't considered a vowel.

## Solution 1

```javascript
const disemvowel = (str) => {
// assign a variable that holds an array of vowels
var vowels = ['a', 'e', 'i', 'o', 'u', 'A', 'E', 'I', 'O', 'U'];
// create empty string
var newStr = '';
// loop thru string
for(let i = 0; i < str.length; i++) {
   // check to see for any vowels a,e,i,o,u
let char = str.charAt(i);
if(vowels.indexOf(str[i]) == -1) {
  newStr += char;
}
  
}

return newStr;

}

```

## Solution 2
```javascript
const disemvowel = (str) => {
  return str.replace(/[aeiou]/gi, '');
}
```
