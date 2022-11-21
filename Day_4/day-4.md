# 4. Gün Alıştrımaları

## Exercises: Level 1

1. Get user input using prompt(“Enter your age:”). If user is 18 or older , give feedback:'You are old enough to drive' but if not 18 give another feedback stating to wait for the number of years he needs to turn 18.

```javascript
let getAge = Number(prompt('Yaşınızı giriniz.', ''));

if(getAge >= 18 )  {
    console.log('Araç kullanmak için uygun yaştasın.');
}
else { 
    console.log(`Araç kullanmak için 18 yaşında olmalısın. ${18 - getAge} yıl sonra görüşelim.`);
};

```
---
2. Compare the values of myAge and yourAge using if … else. Based on the comparison and log the result to console stating who is older (me or you). Use prompt(“Enter your age:”) to get the age as input.

```javascript
let getAge = Number(prompt('Yaşınızı giriniz')); 

let myAge = 27;

if (getAge > myAge) { 
    console.log(`Benden ${getAge - myAge} yaş büyüksün.`);
}
else if (myAge > getAge) { 
    console.log(`Senden ${myAge - getAge} yaş büyüğüm.`);
}
else{
    console.log('Aynı yaştayız.');
}
```
---
3. If a is greater than b return 'a is greater than b' else 'a is less than b'. Try to implement it in to ways

* using if else
* ternary operator.


```javascript
    let a = 4
    let b = 3

if(a > b) {                                 // if else
    console.log('a, b den büyüktür.');
}
else if (a < b) { 
    console.log('b, a dan büyüktür.');
}
else { 
    console.log('a ve b eşittir.');
}

console.log(
    ((a > b) ? 'a, b den büyüktür.' : 'b, a dan büyüktür.')  //ternary operator
)

```
---

4. Even numbers are divisible by 2 and the remainder is zero. How do you check, if a number is even or not using JavaScript?

```javascript
let getNumber = Number(prompt('Bir sayı giriniz', ''));

if(getNumber % 2 == 0 ) { 
    console.log(`${getNumber} çift sayıdır`)
}
else {
    console.log(`${getNumber} tek sayidir.`)
}
```
---
## Exercises: Level 2

1. Write a code which can give grades to students according to theirs scores:
* 90-100, A
* 70-89, B
* 60-69, C
* 50-59, D
* 0-49, F

```javascript
let getScore = Number(prompt('Lütfen notunuzu giriniz', ''));  // switch ile 

switch(100 >= getScore) { 
    case getScore >= 90:
        console.log('Notunuz A');
    break
    case getScore >= 70 :
        console.log('Notunuz B');
    break
    case getScore >= 60 : 
        console.log('Notunuz C');
    break
    case getScore >= 50 :
        console.log ('Notunuz D');
    break
    default:
        console.log('Notunuz F');
}
```
```javascript
let getScore = Number(prompt('Lütfen notunuzu giriniz', ''));   // if else ile

if(getScore >= 90) { 
    console.log('Notunuz A');
}
else if (getScore >= 70) { 
    console.log('Notunuz B');
}
else if (getScore >= 60) { 
    console.log("Notunuz C"); 
}
else if (getScore >= 50) { 
    console.log('Notunuz D');
}
else {
    console.log('Notunuz F');
}
```
---
2. Check if the season is Autumn, Winter, Spring or Summer. If the user input is :
* September, October or November, the season is Autumn.
* December, January or February, the season is Winter.
* March, April or May, the season is Spring
* June, July or August, the season is Summer

```javascript
let season = prompt('Bir ay giriniz', '');  // if else 

season = season.toLowerCase();

if(season == 'september,' || season == 'october' || season == 'november'){
    console.log('Mevsim sonbahar.');
}
else if (season == 'december' || season == 'january' || season == 'february') {
    console.log('Mevsim kış.');
}
else if ( season == 'march' || season == 'april' || season == 'may') {
    console.log('Mevsim bahar.');
}
else if (season == 'june' || season == 'july' || season == 'august') {
    console.log('Mevsim yaz.');
}
else {
    console.log('Bir mevsim girilmemistir.');
}
```
```javascript
let season = prompt('Bir ay giriniz');  // switch ile

season = season.toLowerCase(); 

switch(season) {
    case 'september':
    case 'october' :
    case 'november':
        console.log('Mevsim sonbahar.');
    break;
    case 'december':
    case 'january' :
    case 'february':
        console.log('mevsim kış.');
    break;
    case 'march' :
    case 'april' : 
    case 'may' :
        console.log('Mevsim bahar.');
    break;
    case 'june' :
    case 'july' :
    case 'august' : 
        console.log('Mevsim yaz.');
    default:
        console.log('Lütfen bir mevsim giriniz.');
}
```
---

3. Check if a day is weekend day or a working day. Your script will take day as an input.
```javascript
let getDay = prompt('What is the day today?', '');

getDay = getDay.toLowerCase();

if (getDay == 'monday' || getDay == 'tuesday' || getDay == 'wednesday' || getDay == 'thursday' || getDay == 'friday') { 
    console.log(`${getDay} is  a working day.`);
}
else if (getDay == 'saturday' || getDay == 'sunday') { 
    console.log(`${getDay} is a weekend.`);
}
else {
    console.log('Please enter a day name.');
}
```
---
 ## Exercises: Level 3

 1. Write a program which tells the number of days in a month.
```javascript
let getMonth = prompt('Enter a month', '');

getMonth = getMonth.toLowerCase();

if(
    getMonth == 'january' ||
    getMonth == 'march' || 
    getMonth == 'may' ||
    getMonth == 'july' ||
    getMonth == 'august' ||
    getMonth == 'october' ||
    getMonth == 'december'
) { 
    console.log(`${getMonth} has 31 days.`);
}
else if (
    getMonth == 'november' || 
    getMonth == 'april' ||
    getMonth == 'june' ||
    getMonth == 'september'
) { 
    console.log(`${getMonth} has 30 days.`);
}
else if ( getMonth == 'february') {
    console.log(`${getMonth} has 28 days.`);
}
else {
    console.log('You must enter a month.');
}
```
---
<br> <br>

***Alıştırmaların yapımı sırasında yazım hataları bulunabilir, elimden geldiğince dikkat etmeye çalıştım hatam varsa affola!***
