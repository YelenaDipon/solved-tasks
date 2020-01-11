# solved-tasks
##### * Task# 1 - Breaking chocolate problem 7 KUY 
```javascript
function breakChocolate(n,m) {
  return (m && n) ? n * m -1 : 0;
}
```
##### * Task# 2 -  For Twins: 2. Math operations 8 KUY
```javascript
function iceBrickVolume(radius, bottleLength, rimLength) {
  const rimWidth = bottleLength - rimLength;
  return (rimWidth * (radius * 2)) * radius;
}
```
##### * Task# 3 - Sum of angles 7 KUY
```javascript
function angle(n) {
  return (n - 2) * 180;
}
```
##### * Task# 4 - Sum The Strings 8 KUY 
```javascript
function sumStr(a,b) {
  return (+a+ +b)+''  
}
```
##### * Task# 5 - Convert a Boolean to a String 8 KUY
```javascript
function booleanToString(b){
    return (b === true) ? "true" : "false";
}
```
##### * Task# 6 - Super Duper Easy 8 KUY 
```javascript
function problem(x){
  return typeof x == 'string' ? 'Error' : (x * 50 + 6);
}
```
##### * Task# 7 - Alan Partridge II - Apple Turnover 8 KUY
```javascript
function apple(x) {
  return x ** 2 > 1000 ? 'It\'s hotter than the sun!!' : 'Help yourself to a honeycomb Yorkie for the glovebox.';
}
```
##### * Task# 8 - Area of a Square 8 KUY
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
##### * Task# 9 - Calculate Two People's Individual Ages 7 KUY
```javascript
function getAges(sum,difference){
  let age = sum-difference;
  return (age < 0 || difference < 0) ? null : [age / 2 + difference,age / 2]
}   
```
##### * Task# 10 - Is n divisible by x and y?
```javascript
function isDivisible(n, x, y) {
  return !(n % x || n % y)
}
```
##### * Task# 11 - Chuck Norris VII - True or False? 8 KUY
```javascript
function ifChuckSaysSo(){
  return 0 > 1;
}
```
##### * Task# 12  - Can we divide it? 8 KUY
```javascript
function isDivideBy(number, a, b) {
  return !(number % a || number % b);
}
```
##### * Task# 13  - L1: Set Alarm
```javascript
function setAlarm(employed, vacation){
  return employed > vacation
}
```
##### * Task# 14 - Rock Paper Scissors! 8 KUY
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
##### * Task# 15 -  Is this a triangle? 7 KUY
```javascript
function isTriangle(a, b, c)
{  
   return (a < b + c) && (b < a + c) && (c < a + b);
}
```
##### * Task# 16 -  Training JS #7: if..else and ternary operator 8 KUY
```javascript
function saleHotdogs(n){
  return (n < 5) ? n * 100 :( n >= 5 && n < 10 ? n * 95 : n * 90);
}
```
##### * Task# 17 - Factorial 7 KUY
```javascript
function factorial(n){
let result =1;
  for (let i=1;i<=n;i++)
  result = result*i;
  return result
}
```
##### * Task# 18 - Get Planet Name By ID 8 KUY
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
##### * Task# 19 - Power of two 7 KUY
```javascript
function isPowerOfTwo(n){
  if(n == 1)
    return true;
  if(n < 1)
    return false;
 return isPowerOfTwo(n / 2)
}
```
##### * Task# 20 Difference Of Squares 7 KUY
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
##### * Task# 21 No zeros for heros 8 KUY 
```javascript
function noBoringZeros(n){
let str = n.toString();
  while(str[str.length-1] == 0)str = +str / 10 + '';
return +str;
}
```
##### * Task# 22 Beginner Series #3 Sum of Numbers 7 KUY
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
##### * Task# 23 Sum of the first nth term of Series 7 KUY
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
##### * Task# 24 Power 8 KUY
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
##### таблицы умножения
```javascript
for (let i = 1; i <= 10; i++) {     
  for (let j = 1; j <= 10; j++) {
    console.log(`${i} * ${j} = ${i * j}`);
  }
  console.log('--------------');  
}
```
##### * Task# 25 To square(root) or not to square(root) 8 KUY
```javascript
function squareOrSquareRoot(array) {
let result = [];
 array.forEach(el =>  Number.isInteger(Math.sqrt(el)) ?
 result.push(Math.sqrt(el)) : result.push(Math.pow(el,2)));
               return result;
}
```
##### * Task# 26 You're a square! 7 KUY
```javascript
var isSquare = function(n){
  return Number.isInteger(Math.sqrt(n));
}
```
##### * Task# 27 All Star Code Challenge #22 7 KUY
```javascript
function toTime(seconds) {
  let hours = Math.floor(seconds / 3600);
  let minutes = Math.floor((seconds - hours * 3600) / 60);
return `${hours} hour(s) and ${minutes} minute(s)`
}
```

##### *Task# 28 Expressions Matter 8 KUY
```javascript
function expressionMatter(a, b, c) {
let frst = a * (b + c); let secnd = a * b * c; let trd = a + b * c;  
 let frt = (a + b) * c; let ffth = a + b + c;
return Math.max(...[frst,secnd,trd,frt,ffth]);
}
```

##### *Task# 29 Tortoise racing 6 KUY
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
*Task# 30 Formatting decimal places #1 7 KUY
function twoDecimalPlaces(number) {
  return Math.trunc(number * 100) / 100;
}