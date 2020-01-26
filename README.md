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






