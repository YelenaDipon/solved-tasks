# solved-tasks
* Task 1 - Breaking chocolate problem 7 KUY 
```javascript
function breakChocolate(n,m) {
  return (m && n) ? n * m -1 : 0;
}
```
* Task# 2 -  For Twins: 2. Math operations 8 KUY
```javascript
function iceBrickVolume(radius, bottleLength, rimLength) {
  const rimWidth = bottleLength - rimLength;
  return (rimWidth * (radius * 2)) * radius;
}
```
* Task# 3 - Sum of angles 7 KUY
```javascript
function angle(n) {
  return (n - 2) * 180;
}
```
* Task# 4 - Sum The Strings 8 KUY 
```javascript
function sumStr(a,b) {
  return (+a+ +b)+''  
}
```
* Task# 5 - Convert a Boolean to a String 8 KUY
```javascript
function booleanToString(b){
    return (b === true) ? "true" : "false";
}
```
* Task# 6 - Super Duper Easy 8 KUY 
```javascript
function problem(x){
  return typeof x == 'string' ? 'Error' : (x * 50 + 6);
}
```
* Task# 7 - Alan Partridge II - Apple Turnover 8 KUY
```javascript
function apple(x) {
  return x ** 2 > 1000 ? 'It\'s hotter than the sun!!' : 'Help yourself to a honeycomb Yorkie for the glovebox.';
}
```
* Task# 8 - Area of a Square 8 KUY
```javascript
function squareArea(A){
  return +((A * 2 / Math.PI)**2).toFixed(2);
}
```
or
```javascript
function squareArea(A){
  var circum = 4 * A;
  var radius = circum / (2 * Math.PI);
  var area = Math.pow(radius, 2);
  return Math.round(area*100)/100
}
```
* Task# 9 - Calculate Two People's Individual Ages 7 KUY
```javascript
function getAges(sum,difference){
  let age = sum-difference;
  return (age < 0 || difference < 0) ? null : [age / 2 + difference,age / 2]
}   
```
* Task# 10 - Is n divisible by x and y?
```javascript
function isDivisible(n, x, y) {
  return !(n % x || n % y)
}
```
* Task# 11 - Chuck Norris VII - True or False? 8 KUY
```javascript
function ifChuckSaysSo(){
  return 0 > 1;
}
```
* Task# 12  - Can we divide it? 8 KUY
```javascript
function isDivideBy(number, a, b) {
  return !(number % a || number % b);
}
```
* Task# 13  - L1: Set Alarm
```javascript
function setAlarm(employed, vacation){
  return employed > vacation
}
```
* Task# 14 - Rock Paper Scissors! 8 KUY
```javascript
const rps = (p1, p2) => {
let message1 = "Player 1 won!"; let message2 = "Player 2 won!";
if(p1 == "scissors" && p2 == "paper"){
return message1;}
else if(p1 == "rock" && p2 == "scissors"){
return message1;}
else if(p1 == "paper" && p2 =="rock"){
return message1;}
else if(p1 == p2){return "Draw!"}
else {return message2}
};
```
* Task# 15 -  Is this a triangle? 7 KUY
```javascript
function isTriangle(a, b, c)
{  
   return (a < b + c) && (b < a + c) && (c < a + b);
}
```
* Task# 16 -  Training JS #7: if..else and ternary operator 8 KUY
```javascript
function saleHotdogs(n){
  return (n < 5) ? n * 100 :( n >= 5 && n < 10 ? n * 95 : n * 90);
}
```
* Task# 17 - Factorial 7 KUY
```javascript
function factorial(n){
let result =1;
  for (let i=1;i<=n;i++)
  result = result*i;
  return result
}
```
* Task# 18 - Get Planet Name By ID 8 KUY
```javascript
function getPlanetName(id){
  var name;
  switch(id){
    case 1:
      name = 'Mercury';
      break;
    case 2:
      name = 'Venus';
      break;
    case 3:
      name = 'Earth';
      break;
    case 4:
      name = 'Mars';
      break;
    case 5:
      name = 'Jupiter';
      break;
    case 6:
      name = 'Saturn';
      break;
    case 7:
      name = 'Uranus';
      break;
    case 8:
      name = 'Neptune';
      break;
  }
  return name;
}
```
* Task# 19 - Power of two 7 KUY
```javascript
function isPowerOfTwo(n){
  if(n == 1)
    return true;
  if(n < 1)
    return false;
 return isPowerOfTwo(n / 2)
}
```
* Task# 20 Difference Of Squares 7 KUY
```javascript
function differenceOfSquares(n){
  let i = 1;
  let sumSqr = 0;
  let sumNum = 0; 
    while(i <= n){
    sumSqr+=Math.pow(i,2);
      sumNum+=i;
    i++;
    }
  return Math.pow(sumNum,2) - sumSqr;
}
```
* Task# 21 No zeros for heros 8 KUY 
```javascript
function noBoringZeros(n){
let str = n.toString();
  while(str[str.length-1] == 0)str = +str / 10 + '';
return +str;
}
```
* Task# 22 Beginner Series #3 Sum of Numbers 7 KUY
```javascript
function getSum( a,b )
{
  let result = 0;
  let num1 = Math.min(a,b);
  let num2 = Math.max(a,b);
  for(let i = num1; i <= num2; i++){
    result += i;
  }
    return result;
}
```
* Task# 23 Sum of the first nth term of Series 7 KUY
```javascript
function SeriesSum(n)
{
  let result = 0;
  for(let i = 1; i <= (n * 3) ; i = i + 3){
   result += (1 / i);
  }
  return result.toFixed(2);
}
```
* Task# 24 Power 8 KUY
```javascript
function numberToPower(number, power){
let i = 1; 
let count = 0;
 do{
   i *= number;
    count++;
 } while(count < power);
   return (power === 0) ? 1 : i;
}
```
* таблицы умножения
```javascript
for (let i = 1; i <= 10; i++) {     
  for (let j = 1; j <= 10; j++) {
    console.log(`${i} * ${j} = ${i * j}`);
  }
  console.log('--------------');  
}
```
* Task# 25 To square(root) or not to square(root) 8 KUY
```javascript
function squareOrSquareRoot(array) {
let result = [];
 array.forEach(el =>  Number.isInteger(Math.sqrt(el)) ?
 result.push(Math.sqrt(el)) : result.push(Math.pow(el,2)));
               return result;
}
```
* Task# 26 You're a square! 7 KUY
```javascript
var isSquare = function(n){
  return Number.isInteger(Math.sqrt(n));
}
```
* Task# 27 All Star Code Challenge #22 7 KUY
```javascript
function toTime(seconds) {
  let hours = Math.floor(seconds / 3600);
  let minutes = Math.floor((seconds - hours * 3600) / 60);
return `${hours} hour(s) and ${minutes} minute(s)`
}
```

*Task# 28 Expressions Matter 8 KUY
```javascript
function expressionMatter(a, b, c) {
let frst = a * (b + c); let secnd = a * b * c; let trd = a + b * c;  
 let frt = (a + b) * c; let ffth = a + b + c;
return Math.max(...[frst,secnd,trd,frt,ffth]);
}
```

*Task# 29 Tortoise racing 6 KUY
```javascript
function race(v1, v2, g) {
  if (v1 >= v2) return null;
    let t = g / (v2 - v1); 
    let time = t * 3600;
    let hour = Math.trunc(time / 3600);
    let minute = Math.trunc((time - hour * 3600) / 60); // minutes
    let seconds = Math.trunc(time - hour * 3600 - minute * 60);
    return [hour, minute, seconds]
}
```

* Task# 30 Formatting decimal places #1 7 KUY
```javascript
function twoDecimalPlaces(number) {
  return Math.trunc(number * 100) / 100;
}
```

* Task# 31 Calculate Price Excluding VAT 8 KUY
```javascript
function excludingVatPrice(price){
  return (price === null) ? -1 : +(price / ((.115 * 10))).toFixed(2);
}
```
* Task# 32 Total amount of points 8 KUY
```javascript
function points(games) {
  let sum = 0;
  games.forEach((el) => (el[0] > el[2]) ? sum += 3 : (el[0] === el[2]) ? sum += 1 : 0);
return sum;
}
```
* Task# 33 How good are you really? 8 KUY
```javascript
function betterThanAverage(classPoints, yourPoints) {
  let classPointsTotal = 0;
  classPoints.reduce((a,b)=> classPointsTotal = a + b);
  return yourPoints > (classPointsTotal / classPoints.length);
}
```
* Task# 34 Odd or Even? 7 KUY
```javascript
function oddOrEven(array) {
   array.push(0);
  let sum = 0; 
  (array.length === 0) ? 0 : array.push(0),array.reduce((a,b)=> sum = (a + b));
  return (sum % 2 === 1 || sum % 2 === -1) ? 'odd': 'even'
  }
```
* Task# 35 Divide and Conquer 7 KUY
```javascript
function divCon(x){
let stringSum = 0; let numberSum = 0;
  x.map((el)=> (typeof el === 'string') ? stringSum += +el : numberSum += el);
  return numberSum - stringSum;
}
```
* Task# 36 Remove the minimum 7 KUY
```javascript
function removeSmallest(numbers) {
let sum = [];
  let min = numbers.indexOf(Math.min(...numbers))
for (let i = 0; i < numbers.length; i++){
       sum.push(numbers[i]);  
}
  sum.splice(min,1)
return sum;
}
```
* Task# 37 Find Maximum and Minimum Values of a List 8 KUY
```javascript
let min = function(list){
    return Math.min(...list)
};
let max = function(list){
    
    return Math.max(...list)
}
```
* Task# 38 Find the divisors! 7 KUY
```javascript
function divisors(integer) {
  let array = [];
  for (let i = 2; i < integer; i++) {
    if (integer%i === 0) array.push(i)
  }
  return array.length === 0 ? `${integer} is prime` : array
};
```
* Task# 39 Pre-FizzBuzz Workout #1 8 KUY
```javascript
function preFizz(n) {
let result = [];
for(let i = 1; i <= Number(n); i++){
result.push(i);
}
return result;
}
```
* Task# 40 Unfinished Loop - Bug Fixing #1 8 KUY
```javascript
function createArray(number){
  let newArray = [];
  for(let i = 1; i <= Number(number); i++){
    newArray.push(i);
  }
  return newArray;
}
```
* Task# 41 Count by X 8 KUY
```javascript
function countBy(x, n) {
  let result = [];
for(let i = x; i <= n * x; i = i + x){
result.push(i);
}
  return result;
}
```
* Task# 42 Training JS #4: Basic data types--Array 8 KUY
```javascript
function getLength(arr){
  return arr.length;
}
function getFirst(arr){
  return arr[0];
}
function getLast(arr){
  return arr[arr.length-1];
}
function pushElement(arr){
  arr.push(1);
  return arr;
}
function popElement(arr){
  arr.pop();
  return arr;
}
```
* Task# 43 No Loops 2 - You only need one 8 KUY
```javascript
function check(a, x) {
  return a.includes(x);
}
```
* Task# 44 Be Concise IV - Index of an element in an array 8 KUY
```javascript
function find(a, e) {
    let i = a.indexOf(e);  
    return i < 0 ? "Not found" : i;
}
```
* Task# 45 JavaScript Array Filter 7 KUY
```javascript
function getEvenNumbers(numbersArray){
  return numbersArray.filter(el => el % 2 === 0);
}
```
* Task# 46 Find numbers which are divisible by given number 8 KUY
```javascript
function divisibleBy(numbers, divisor){
  return numbers.filter(el => el % divisor === 0);
}
```
* Task# 47 Removing Elements 8 KUY
```javascript
function removeEveryOther(arr){
  return arr.filter((el, i) => i % 2 === 0);
}
```
* Task# 48 Well of Ideas - Easy Version 8 KUY
```javascript
function well(x){
let good = x.filter(el=> el === 'good');
return (good.length > 2) ? 'I smell a series!' : (good.length === 1 || good.length === 2) ? 'Publish!' : 'Fail!';
}
```
* Task# 49 Find how many times did a team from a given country win the Champions League? 7 KUY
```javascript
function countWins(winnerList1, country) {
 let count = 0;
  for(let i = 0; i < winnerList1.length; i++){
    if(winnerList1[i].country === country){
      count++
    }
  }
  return count;
}
```
* Task# 50 filterEvenLengthWords 7 KUY
```javascript
function filterEvenLengthWords(words) {
  return words.filter(el => el.length % 2 === 0);
}
```
* Task# 51 Array.diff 6 KUY
```javascript
function array_diff(a, b) {
   return a.filter( el => !b.includes(el));
}
```
* Task# 52 Find Duplicates 7 KUY
```javascript
function duplicates(arr) {
  return arr.filter((el,i) => i !== arr.indexOf(el) && i === arr.lastIndexOf(el))
}
```
* Task# 53 Train to remove duplicates from an array with filter() 7 KUY
```javascript
function unique(arr) {
  return arr.filter((el, i) => i === arr.indexOf(el));
}
```
* Task# 54 Santa's Naughty List 7 KUY
```javascript
const findChildren = (santasList, children) => [...new Set(children.filter(name => santasList.includes(name)).sort())]
```
* Task# 55 My head is at the wrong end! 8 KUY
```javascript
function fixTheMeerkat(arr) {
  return arr.reverse();
}
```
* Task# 56 Two Oldest Ages 7 KUY
```javascript
function twoOldestAges(ages){
   ages.sort((a,b) => b - a);
   return [ages[1],ages[0]] 
}
```
* Task# 57 Sum of two lowest positive integers 7 KUY
```javascript
function sumTwoSmallestNumbers(numbers) {  
  numbers.sort((a,b) => b - a ).reverse();
  return numbers[0] + numbers[1] 
}
```
* Task# 58 Sentence Smash 8 KUY
```javascript
function smash (words) {
    "use strict";
    return words.join(' ');
};
```
* Task# 59 String Templates - Bug Fixing #5 8 KUY
```javascript
function buildString(...template){
  return (`I like ${template.join(', ')}` + "!");
}
```
* Task# 60 CSV representation of array 8 KUY
```javascript
function toCsvText(array) {
   return array.join('\n');
}
```
* Task# 61 Printing Array elements with Comma delimiters 8 KUY
```javascript
function printArray(array){
  return array.join();
}
```
* Task# 62 Enumerable Magic #1 - True for All? 8 KUY
```javascript
function all( arr, fun ){
  return arr.every(el=>fun(el)) 
}
```
* Task# 63 Grasshopper - Array Mean 8 KUY
```javascript
var findAverage = function (nums) {
  return nums.reduce((a,b) => a + b) / nums.length
}
```
* Task# 64 Beginner - Reduce but Grow 8 KUY
```javascript
function grow(x){return x.reduce((a,b)=> a * b)};
```
* Task# 65 SpeedCode #2 - Array Madness 8 KUY
```javascript
function arrayMadness(a,b) {
  let firstArray = a.reduce((c,d)=> c + d ** 2,1)
  let secondArray = b.reduce((e,f)=> e + f ** 3,1)
return firstArray >= secondArray
}
```
* Task# 66 Enumerable Magic #25 - Take the First N Elements 8 KUY
```javascript
function take(arr, n) {
  return arr.splice(0,n);
}
```
* Task# 67 Remove First and Last Character Part Two 8 KUY
```javascript
function array(arr){
  arr = arr.split(',').slice(1,-1);
  let result = arr.toString().replace(/,/g, ' ');
  return (result === '') ? null : result;
}
```
* Task# 68 Jenny's secret message 8 KUY
```javascript
function greet(name){
  return name === "Johnny" ? "Hello, my love!" : "Hello, " + name + "!";
}
```
* Task# 69 Template Strings 8 KUY
```javascript
var TempleStrings = function(obj, feature) {
  return `${obj} are ${feature}`;
}
```
* Task# 70 Grasshopper - Combine strings 8 KUY
```javascript
function combineNames(a,b){
    return a +" "+ b;
}
```
* Task# 71 Numbers to Letters 7 KUY
```javascript
function switcher(x){
  const alp = "0zyxwvutsrqponmlkjihgfedcba!? ";
  return x.map((el, i) => el = alp[el]).join('');
}
```
* Task# 72 get character from ASCII Value 8 KUY
```javascript
function getChar(x) {
  return String.fromCharCode(x);
}
```
* Task# 73 Regex validate PIN code 7 KUY
```javascript
function validatePIN (pin) {
if(!pin) return false;
  let numbersLength = pin.match(/[0-9]/g).length;
return numbersLength === pin.length && (numbersLength === 4 || numbersLength === 6);
}
```
* Task# 74 Triple Trouble 8 KUY
```javascript
function tripleTrouble(one, two, three){
  let result = '';
  for (let i = 0; i < one.length; i++) {
    result += (one[i] + two[i] + three[i]);
  }
  return result;
 }
```
* Task# 75 Regex count lowercase letters 8 KUY
```javascript
function lowercaseCount(str){
  return !str.match(/[a-z]/g) ? 0 : str.match(/[a-z]/g).length;
}
```
* Task# 76 Spacify 7 KUY
```javascript
function spacify(str) {
let result = '';
let i = 0;
do{result += str[i] + ' ';
i++;
}
while(i < str.length);
return result.trim();
}
```
* Task# 77 Is it a palindrome? 8 KUY
```javascript
function isPalindrome(x) {
x = x.toLowerCase();
let reversed = '';
for(let i = x.length-1 ; i >= 0 ; i--){
reversed += x[i];
}
return reversed === x;
}
```
* Task# 78 Unique In Order 6 KUY
```javascript
var uniqueInOrder=function(iterable){
let array = [];
  for(let i = 0; i < iterable.length; i++){
    if(iterable[i]!==iterable[i + 1]){
      array.push(iterable[i])
    }
  }
return array;
}
```
* Task# 79 The Wide-Mouthed frog! 8 KUY
```javascript
function mouthSize(animal) {
  return animal.toLowerCase() === 'alligator' ? 'small' : 'wide';
}
```
* Task# 80 Find the capitals 7 KUY
```javascript
var capitals = function (word) {
  const result = [];
  for (let i = 0; i < word.length; i++){
    if (word[i] === word[i].toUpperCase()){
      result.push(i);
    }  
  }
  return result;
};
```
* Task# 81 MakeUpperCase 8 KUY
```javascript
function makeUpperCase(str) {return str.toUpperCase();}
```
* Task# 82 Thinking & Testing : Something capitalized 7 KUY
```javascript
function testit(s){
  if (!s){
    return s;
  }
  return  s.split(' ').map((el)=> el.slice(0,-1) + el[el.length -1].toUpperCase()).join(' ');
}
```
* Task# 83 repeatIt 8 KUY
```javascript
var repeatIt = function(str, n) {
  return typeof str === "string" ? str.repeat(n) : "Not a string";
}
```
* Task# 84 Don't give me five! 7 KUY
```javascript
function dontGiveMeFive(start, end) {
    let count = 0;
    for (let i = start; i <= end; i++) {
        if (!i.toString().includes('5')) {
            count++;
        }
    }
    return count;
}
```
* Task# 85 Do you speak "English"? 8 KUY
```javascript
function spEng(sentence){
return sentence.search(/english/i)>=0
}
```
* Task# 86 Find the position! 8 KUY
```javascript
function position(letter){
  let alphabet = ' abcdefghijklmnopqrstuvwxyz';
  return `Position of alphabet: ${alphabet.indexOf(letter)}`;
}
```
* Task# 87 validate code with simple regex 8 KUY
```javascript
function validateCode (code) {
  code = code.toString();
  return code.startsWith('1') || code.startsWith('2') || code.startsWith('3');
}
```
* Task# 88 String ends with? 7 KUY
```javascript
function solution(str, ending){
  return str.endsWith(ending);
}
```
* Task# 89 Tail Swap 7 KUY
```javascript
function tailSwap(arr) {
  let firstStr =  arr[0].slice(arr[0].indexOf(':'));
  let secondStr = arr[1].slice(arr[1].indexOf(':'));
  return [arr[0].slice(0,arr[0].indexOf(':')) + secondStr, arr[1].slice(0,arr[1].indexOf(':')) + firstStr];
}
```
* Task# 90 Credit Card Mask 7 KUY
```javascript
function maskify(cc) {
    let result = '#';
  if(cc.length < 5){
    return cc
  }
  result += result.repeat(cc.length-5)
return result + cc.slice(-4)
}
```
* Task# 91 Vowel remover 8 KUY
```javascript
function shortcut(string){
  return string.replace(/[aeiou]/gi, '');
}
```
* Task# 92 DNA to RNA Conversion 8 KUY
```javascript
function DNAtoRNA(dna) {
  return dna.replace(/[T]/gi, 'U');
}
```
* Task# 93 Get number from string 8 KUY
```javascript
function getNumberFromString(s) {
  return Number( s.match(/[0-9]/g).join(""))
}
```
* Task# 94 FIXME: Replace all dots 8 KUY
```javascript
var replaceDots = function(str) {
  return str.replace(/[.]/g, '-');
}
```
* Task# 95 Exclamation marks series #2: Remove all exclamation marks from the end of sentence 8 KUY
```javascript
function remove(s){
let letter = s.match(/[a-z]/gi);
let i = s.lastIndexOf(letter[letter.length - 1]);
return s.slice(0,i + 1);
}
```
* Task# 96 Reversed Words 8 KUY
```javascript
function reverseWords(str){
  return str.split(' ').reverse().join(' ');
}
```
* Task# 97 Descending Order 7 KUY
```javascript
function descendingOrder(n){
  return parseInt(String(n).split('').sort().reverse().join(''))
}
```
* Task# 98 Highest and Lowest 7 KUY
```javascript
function highAndLow(numbers){
  numbers = numbers.split(' ').sort( (a, b) => b - a);
  return numbers[0] + ' ' + numbers[numbers.length - 1];
}
```
* Task# 99 Name Shuffler 8 KUY
```javascript
function nameShuffler(str){
  return str.split(' ').reverse().join(" ");
}
```
* Task# 100 Squash the bugs 8 KUY
```javascript
function findLongest(str) {
  
  let spl = str.split(" ");
  let longest = 0;
  
  for (let i = 0; i < spl.length; i++){
    if (spl[i].length > longest){
      longest = spl[i].length;
    }
  }
  return longest;
};
```
* Task# 101 Reversing Words in a String 8 KUY
```javascript
function reverse(string){
  return string.split(' ').reverse().join(' ');
}
```
* Task# 102 Can Santa save Christmas? 7 KUY
```javascript
function determineTime(durations){
let hours = 0;
let minutes = 0;
let seconds = 0;
  for(let i = 0 ; i < durations.length ; i++){
    hours += +(durations[i].split(':')[0]);
    minutes += +(durations[i].split(':')[1]);
    seconds += +(durations[i].split(':')[2]);
  }
return hours * 3600 + minutes * 60 + seconds <= 24 * 3600;
}
```
* Task# 103 Every possible sum of two digits 7 KUY
```javascript
function digits(n){
    n = n.toString();
    let result = [];
    for(let i = 0; i < n.length; i++){
        for(let j = i + 1; j < n.length; j++){
            result.push(Number(n[i]) + Number(n[j]));
        }
    }
    return result;
}
```
* Task# 104 Welcome! 8 KUY
```javascript
function greet(language) {
let dataBase = {
english: 'Welcome',
czech: 'Vitejte',
danish: 'Velkomst',
dutch: 'Welkom',
estonian: 'Tere tulemast',
finnish: 'Tervetuloa',
flemish: 'Welgekomen',
french: 'Bienvenue',
german: 'Willkommen',
irish: 'Failte',
italian: 'Benvenuto',
latvian: 'Gaidits',
lithuanian: 'Laukiamas',
polish: 'Witamy',
spanish: 'Bienvenido',
swedish: 'Valkommen',
welsh: 'Croeso',
default : 'Welcome',
};
return (!dataBase[language]) ? dataBase.default : dataBase[language] ;
}
```
* Task# 105 Duck Duck Goose 8 KUY
```javascript
function duckDuckGoose(players, goose) {
  return goose ? players[(goose - 1) % players.length].name : '';
}
```
* Task# 106 Make a function that does arithmetic! 7 KUY
```javascript
function arithmetic(a, b, operator){
  if (operator === "add") {
      return a + b;
      } else if (operator === "subtract") {
      return a - b;
      }  else if (operator === "multiply") {
      return a * b;
      }  else {
      return a / b};
}
```
* Task# 107 Beginner Series #2 Clock 8 KUY
```javascript
function past(h, m, s){
  return h * 3600000 + m * 60000  + s * 1000;
}
```
* Task# 108 makeBackronym 7 KUY
```javascript
var dict = {
'A': "awesome",
'B': 'beautiful',
'C': 'confident',
'D': 'disturbing',
'E': 'eager',
'F': 'fantastic',
'G': 'gregarious',
'H': 'hippy',
'I': 'ingestable',
'J': 'joke',
'K': 'klingon',
'L': 'literal',
'M': 'mustache',
'N': 'newtonian',
'O': 'oscillating',
'P': 'perfect',
'Q': 'queen',
'R': 'rant',
'S': 'stylish',
'T': 'turn',
'U': 'underlying',
'V': 'volcano',
'W': 'weird',
'X': 'xylophone',
'Y': 'yogic',
'Z': 'zero'
};
var makeBackronym = function(string){
let result = '';
for(let i = 0; i < string.length; i++){
result += dict[string[i].toUpperCase()] + ' ';
}
return result.trim();
};
```
* Task# 109 Check three and two 7 KUY
```javascript
function checkThreeAndTwo(array) {
  let a = 0;
  let b = 0;
  let c = 0;
  array.map((el)=> (el === 'a') ? a++ : (el === 'b') ? b++ : c++);
return (a === 3 && b === 2) || (a === 2 && b === 3) || (a === 3 && c === 2) || (c === 3 && a === 2) || (c === 3 && b === 2) || (c === 2 && b === 3)
}
```
* Task# 110 Add property to every object in array 7 KUY
```javascript
for(let i = 0; i < questions.length; i++) {
  questions[i].usersAnswer = null;
}
```
* Task# 111 Numbers to Objects 7 KUY
```javascript
function numObj(s){
  let result = []; 
  for(let i = 0; i < s.length; i++){
    result.push({[s[i]] : String.fromCharCode(s[i])})
  }
  return result;
};
```
* Task# 112 Coding Meetup #5 - Higher-Order Functions Series - Prepare the count of languages 7 KUY
```javascript
function countLanguages(list) {
  let result = {}; 
  for(let i = 0; i < list.length; i++){
    result[list[i].language] === undefined ? 
      result[list[i].language] = 1: result[list[i].language]++}
return result;
}
```
* Task# 113 What is my name score? #1 7 KUY
```javascript
function nameScore(name){
let count = 0 ;
for(let key in alpha){
  for(let i = 0; i < name.length; i++){
  (key.includes(name.toUpperCase()[i])) ? count+=alpha[key] : 0;
}
}
  return {[name] : count}
}
```
* Task# 114 The Office I - Outed 7 KUY
```javascript
function outed(meet, boss){
let count = 0; let array = []; let bos;
 for(let key in meet){
 (boss === key) ? bos = meet[key] : key;
    array.push(key)
   count += meet[key] ;
 }
  count = count + bos
  return (count / array.length <= 5) ? 'Get Out Now!' : 'Nice Work Champ!'
}
```
* Task# 115 Permute a Palindrome 6 KUY
```javascript
function permuteAPalindrome (input) { 
  let array = input.split('');
  let spec = [...new Set (input)];
  const countArr = []; 
  for(let i = 0; i < spec.length; i++){
  let count = 0; 
    for(let j = 0; j < array.length; j++){
            if(array[j] === spec[i]) count++;
      console.log(spec[i]);
    }
    if(count % 2 !== 0) countArr.push(1);
  }
  return countArr.length <= 1;
}
```
OR
```javascript
function permuteAPalindrome ([...input], odd = 0) { 
  new Set(input).forEach(a => input.filter(b => b == a).length % 2 ? odd++ : 0)
  return odd < 2;
}
```
* Task# 116 Most valuable character 7 KUY
```javascript
function solve(st) {
 let  str = st.split('');
    let b = [0,''];  
    let dif = 0;
  for(let i = 0; i < st.length; i++){
 dif = st.lastIndexOf(st[i]) - st.indexOf(st[i]);
    if(st.lastIndexOf(st[i]) === st.indexOf(st[i])) { dif = 1}
    if(dif > b[0]){
      b[0] = dif; 
      b[1] = st[i]; 
    } else if (dif === b[0] && str[i] < b[1]){ 
          b[1] = st[i]; 
        }
 
  }
    return b[1];
}

```
* Task# 117 How many days are we represented in a foreign country? 7 KUY
```javascript
function daysRepresented(trips){
let result = [];
  for (let i = 0; i < trips.length; i++){
    for (let j = trips[i][0]; j <= trips[i][1]; j++){
      if (result.indexOf(j) === -1){
        result.push(j);
      }
    }
  }
  return result.length;
}
```
* Task# 118 The Office II - Boredom Score 7 KUY
```javascript
let score ={
  'accounts' : 1,
'finance': 2,
'canteen' : 10,
'regulation' : 3,
'trading': 6,
'change' : 6,
'IS' : 8,
'retail' : 5,
'cleaning' : 4,
'pissing about' : 25,
};
function boredom(staff){
 let count = 0;
for(let key in staff){
  count += score[staff[key]]
}
return (count <=80) ? 'kill me now' :
count < 100 & count > 80 ? 'i can handle this' :
'party time!!';
}
```
* Task# 119 No oddities here 7 KUY
```javascript
function noOdds( values ){
let result = [];
values.filter((el)=> el % 2 === 0 ? result.push(el) : 0)
return result;
}
```
* Task# 120 Area or Perimeter 8 KUY
```javascript
const areaOrPerimeter = function(l , w) {
  return l === w ? l * w : (l * 2) + (w * 2);
}
```
* Task# 121 Find the Difference in Age between Oldest and Youngest Family Members 8 KUY 
```javascript
function differenceInAges(ages){
  let sortedAges = ages.sort((a,b)=>a-b);
  return [sortedAges[0],sortedAges[sortedAges.length-1],sortedAges[sortedAges.length-1]-sortedAges[0]];
}
```
* Task# 122 Maximum Multiple 7 KUY 
```javascript
function maxMultiple(divisor, bound) {
  return Math.floor(bound / divisor) * divisor;
}
```


























































