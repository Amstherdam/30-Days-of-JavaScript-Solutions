# 6. Gün Alıştrımaları
## Exercises: Level 1
1. Iterate 0 to 10 using for loop, do the same using while and do while loop.
```javascript
for(let i = 0; i <= 10; i++) {   // for
    console.log(i);
}
```
```javascript
let i = 0;                       // while
while( i <= 10 ) { 
    console.log(i);
    i++;
}
```
```javascript
let i = 0;                       // do while
do{
    console.log(i)
    i++;
} while (i <= 10);
```
---
2. Iterate 10 to 0 using for loop, do the same using while and do while loop.
```javascript
for( let i = 10; i >= 0; i--) {  // for 
    console.log(i);
}
```
```javascript
let i = 10;                      // while  
while( i >= 0) { 
    console.log(i);
    i--;
}
```
```javascript
let i = 10;                      // do while
do{ 
    console.log(i);
    i--;
} while ( i >= 0 );
```
---
3. Iterate 0 to n using for loop.
```javascript
let n = Number(prompt('Bir sayı giriniz',''));

for(let i = 0;  i <= n; i++){
    console.log(i);
}
```
---
4. Write a loop that makes the following pattern using console.log():
```javascript
let hashtag = '#'

for(let i = 0; i <=7; i++) { 
    console.log(hashtag);
    hashtag = hashtag + '#'
}
```
---
5. Use loop to print the following pattern:
```javascript
for(let i = 0 ; i <= 10; i++ ) { 
    console.log(`${i} * ${i} = ${i * i}`);
}
```
---
6. Using loop print the following pattern.
```javascript
console.log('i     i^2   i^3');
for(let i = 0 ; i <= 10; i++ ) { 
    console.log(`${i}     ${i ** 2}     ${i ** 3}`);
}
```
---
7. Use for loop to iterate from 0 to 100 and print only even numbers.
```javascript
for(let i = 0; i <= 100; i+= 2) { 
    console.log(i);
}
```
---
8. Use for loop to iterate from 0 to 100 and print only odd numbers.
```javascript
for(let i = 1; i <= 100; i+= 2) { 
    console.log(i);
}
```
---
9. Use for loop to iterate from 0 to 100 and print only prime numbers.
```javascript
let n = 100;
nextPrime: for ( let i = 2; i < n; i++) { 
                for (let j = 2; j < i; j++) { 
                    if (i % j == 0) continue nextPrime;
    }
    console.log(i);
}
```
---
10. Use for loop to iterate from 0 to 100 and print the sum of all numbers.
```javascript
let total = 0;

for(let i = 0; i <= 100; i++ ){ 
    total = total + i
    console.log(`${i}:   ${total}`);
}
```
---
11. Use for loop to iterate from 0 to 100 and print the sum of all evens and the sum of all odds.
```javascript
let evenTotal = 0;
let oddTotal = 0 ;

for(let i = 0; i <= 100; i++) { 
    if(i%2 == 0){
        evenTotal = evenTotal + i;
    }
    else{
        oddTotal = oddTotal + i;
    }
    console.log(`Even: ${evenTotal}      Odd: ${oddTotal}`)
}
console.log(`The sum of all evens from 0 to 100 is ${evenTotal}. And the sum of all odds from 0 to 100 is ${oddTotal}.`)
```
---
12. Use for loop to iterate from 0 to 100 and print the sum of all evens and the sum of all odds. Print sum of evens and sum of odds as array.
```javascript
let evenTotal = 0;
let oddTotal = 0 ;
const arr = [];

for(let i = 0; i <= 100; i++) { 
    if(i%2 == 0){
        evenTotal = evenTotal + i;
    }
    else{
        oddTotal = oddTotal + i;
    }
    arr[0] = evenTotal;
    arr[1] = oddTotal
    console.log(arr);
}
```
---
13. Develop a small script which generate array of 5 random numbers.
```javascript
let arr = []

for(let i = 10; i<15 ; i ++ ) { 
    arr.push(Math.floor(Math.random() * i ));
}

console.log(arr);
```
---
14. Develop a small script which generate array of 5 random numbers and the numbers must be unique.
```javascript
let randomUniqueArr = [];

while ( randomUniqueArr.length < 5 ) {
    let random = Math.floor(Math.random() * 10);
    if(randomUniqueArr.indexOf(random) === -1) {
        randomUniqueArr.push(random);
    }
}

console.log(randomUniqueArr);

// while döngüsü kullanımı  for döngüsüne göre daha okunabilir olduğu için tercih edildi. 
```
---
15. Develop a small script which generate a six characters random id:
```javascript
function makeId(length) {
    let result = '';
    let characters = `ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789`;

    for (let i = 0; i < length; i++) { 
        result += characters.charAt(Math.floor(Math.random() * characters.length));
    }
    return result;
}

console.log(makeId(6) );
```
---
## Exercises: Level 2
1. Develop a small script which generate any number of characters random id:
```javascript
let characters = `ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789`;
let random1 = Math.floor(Math.random() * 30);
let result = '';

for (let i = 0; i < random1; i++) { 
    result += characters.charAt(Math.floor(Math.random() * characters.length));
}
console.log(result); 
```
---
2. Write a script which generates a random hexadecimal number.
```javascript
let hexadecimalNumber = '0123456789ABCDEF'
let result = '#'

for(let i = 0; i < 6; i++) {
    result += hexadecimalNumber.charAt(Math.floor(Math.random() * hexadecimalNumber.length));
}

console.log(result);
```
---
3. Write a script which generates a random rgb color number.
```javscript

```
---
4. Using the above countries array, create the following new array.
```javascript 
const countries = [
    'Albania',
    'Bolivia',
    'Canada',
    'Denmark',
    'Ethiopia',
    'Finland',
    'Germany',
    'Hungary',
    'Ireland',
    'Japan',
    'Kenya'
  ]

let countriesUpper = []   

for(let i = 0; i < countries.length; i++) { 
    countriesUpper.push(countries[i].toUpperCase());
}

console.log(countriesUpper);
```
5. Using the above countries array, create an array for countries length'.
```javascript
const countries = [
    'Albania',
    'Bolivia',
    'Canada',
    'Denmark',
    'Ethiopia',
    'Finland',
    'Germany',
    'Hungary',
    'Ireland',
    'Japan',
    'Kenya'
  ]

let countriesLength = [];

for(let i = 0; i < countries.length; i++) { 
    countriesLength.push(countries[i].length);
}

console.log(countriesLength);
```
---
6. Use the countries array to create the following array of arrays:
```javascript
const countries = [
    'Albania',
    'Bolivia',
    'Canada',
    'Denmark',
    'Ethiopia',
    'Finland',
    'Germany',
    'Hungary',
    'Ireland',
    'Japan',
    'Kenya'
  ] 
  
let countriesK = [];
  
for (let i = 0; i < countries.length; i++) {
    countriesK.push((countries[i].substring(0,3)).toUpperCase());
}

console.log(countriesK); // 'ALB' şeklinde olan ikinci eleman bulundu

let countriesAll = [];

for (let i = 0; i < countries.length; i++) { 
    countriesAll[i] = [countries[i], countriesK[i], countriesLength[i]]
}

console.log(countriesAll); // 5. alıştırmada bulduğumuz length değeri ve default haldeki countries değeri kullanıldı.
```
---
7. In above countries array, check if there is a country or countries containing the word 'land'. If there are countries containing 'land', print it as array. If there is no country containing the word 'land', print 'All these countries are without land'.
```javascript
const countries = [ // Iceland verilen listede yok  unutulmuş sanirsam eklememiz lazım.
  'Albania',
  'Bolivia',
  'Canada',
  'Denmark',
  'Ethiopia',
  'Finland',
  'Germany',
  'Hungary',
  'Ireland',
  'Iceland'
  'Japan',
  'Kenya'
]

let countriesLand = [];

for ( let i = 0 ; i < countries.length ; i++){
    if(countries[i].includes('land')) {
        countriesLand.push(countries[i])
    }
}

console.log(countriesLand);
```
---
8. In above countries array, check if there is a country or countries end with a substring 'ia'. If there are countries end with, print it as array. If there is no country containing the word 'ia', print 'These are countries ends without ia'.
```javascript
const countries = [
    'Albania',
    'Bolivia',
    'Canada',
    'Denmark',
    'Ethiopia',
    'Finland',
    'Germany',
    'Hungary',
    'Ireland',
    'Iceland',
    'Japan',
    'Kenya',
    'Iceland'
  ] 

let countriesIA = [];

for (let i = 0; i < countries.length; i++)  {
    if(countries[i].endsWith('ia') == true) {
        countriesIA.push(countries[i]);
    }    
}

console.log(countriesIA);
```
--- 
9. Using the above countries array, find the country containing the biggest number of characters.
```javascript
const countries = [
    'Albania',
    'Bolivia',
    'Canada',
    'Denmark',
    'Ethiopia',
    'Finland',
    'Germany',
    'Hungary',
    'Ireland',
    'Iceland',
    'Japan',
    'Kenya',
    'Iceland'
  ] 

let countriesLength = [];

for (let i = 0; i < countries.length; i++) {
    countriesLength.push(countries[i].length);
}

let highest;
highest = Math.max.apply(null, countriesLength);
console.log(countries[countriesLength.indexOf(highest)]);
```
---
10. Using the above countries array, find the country containing only 5 characters.
```javascript
const countries = [
    'Albania',
    'Bolivia',
    'Canada',
    'Denmark',
    'Ethiopia',
    'Finland',
    'Germany',
    'Hungary',
    'Ireland',
    'Iceland',
    'Japan',
    'Kenya',
    'Iceland'
  ] 

for (let i = 0; i < countries.length; i++) { 
    if (countries[i].length === 5) {
        console.log(countries[i]);
    }
}

```
---
11. Find the longes word in the webTechs array.
```javascript
const webTechs = [
    'HTML',
    'CSS',
    'JavaScript',
    'React',
    'Redux',
    'Node',
    'MongoDB'
  ]

let webTechsLength = [];

for (let i = 0; i < webTechs.length; i++){
    webTechsLength.push(webTechs[i].length);
}

let highest;
highest = Math.max.apply(null, webTechsLength);
console.log(webTechs[webTechsLength.indexOf(highest)]);
```
---
12. Use the webTechs array to create the following array of arrays:
```javascript
const webTechs = [
    'HTML',
    'CSS',
    'JavaScript',
    'React',
    'Redux',
    'Node',
    'MongoDB'
  ]

let webTechsLength = [];
let webTechsAll = [];

for (let i = 0; i < webTechs.length; i++){
    webTechsLength.push(webTechs[i].length);
}

for (let i = 0; i < webTechs.length; i++) { 
    webTechsAll[i] = [webTechs[i], webTechsLength[i]]
}

console.log(webTechsAll);
```
---
13. An application created using MongoDB, Express, React and Node is called a MERN stack app. Create the acronym MERN by using the array mernStack.
```javascript
const mernStack = ['MongoDB', 'Express', 'React', 'Node']

let mern = '';
for ( let i = 0; i < mernStack.length; i++) { 
    mern += mernStack[i].slice(0, 1);
}

console.log(mern);
```
---
14. Iterate through the array, ["HTML", "CSS", "JS", "React", "Redux", "Node", "Express", "MongoDB"] using a for loop or for of loop and print out the items.
```javascript
let techs = ["HTML", "CSS", "JS", "React", "Redux", "Node", "Express", "MongoDB"]
for (let i = 0; i < techs.length; i++) {
    console.log(techs[i])
}
```
```javascript
for ( let tech of techs) { 
    console.log(tech)
}
```
---
15. This is a fruit array , ['banana', 'orange', 'mango', 'lemon'] reverse the order using loop without using a reverse method.
```javascript
let fruitArr = ['banana', 'orange', 'mango', 'lemon'];

let fruitArrReverse = [];

for (let i = fruitArr.length -1 ; i >= 0 ; i-- ) { 
    fruitArrReverse.push(fruitArr[i]);
}

console.log(fruitArrReverse);
```
16. Print all the elements of array as shown below.
```javascript
const webTechs = [
    'HTML',
    'CSS',
    'JavaScript',
    'React',
    'Redux',
    'Node',
    'MongoDB'
  ]

const fullStack = [];
const frontEnd = [];
const backEnd = [];

for (let i = 0; i < 4; i++) { 
    frontEnd.push(webTechs[i]);
}

for (let i = 4; i < webTechs.length; i++) { 
    backEnd.push(webTechs[i]);
} 

fullStack.push(frontEnd, backEnd);
console.log(fullStack);
```
---
## Exercises: Level 3
1. Copy countries array(Avoid mutation).  <br> // Mutasyonun ne olduğunu bilmiyorum umarım doğrudur.
```javascript
const countries2 = []

for (let i = 0; i < countries.length; i++) { 
    countries2.push(countries[i]);
}

console.log(countries2);
```
---
2. Arrays are mutable. Create a copy of array which does not modify the original. Sort the copied array and store in a variable sortedCountries.
```javascript
const sortedCountries = [];

for ( let i = 0; i < countries.length; i++) { 
    sortedCountries.push(countries[i]);
}

sortedCountries.sort();

console.log(sortedCountries)
```
---
3. Sort the webTechs array and mernStack array.
```javascript
const webTechs = [
    'HTML',
    'CSS',
    'JavaScript',
    'React',
    'Redux',
    'Node',
    'MongoDB'
  ]
  
  const mernStack = [
    'MongoDB', 
    'Express', 
    'React', 
    'Node'
]

webTechs.sort();
mernStack.sort();

console.log(webTechs);
console.log(mernStack);
```
4. Extract all the countries contain the word 'land' from the countries array and print it as array.
```javascript
let countriesWithLand = [];

for ( let i = 0; i < countries.length; i++) { 
    if( countries[i].includes('land')) { 
        countriesWithLand.push(countries[i]);
    }
}

console.log(countriesWithLand);
```
---
5. Find the country containing the hightest number of characters in the countries array.
```javascript
let countriesLength = [];

for ( let i = 0; i < countries.length; i++) { 
    countriesLength.push(countries[i].length);
}
let hightest;
hightest = Math.max.apply(null , countriesLength);

console.log(countries[countriesLength.indexOf(hightest)]);  // Central African Republic
```
---
6. Extract all the countries contain the word 'land' from the countries array and print it as array.
* 4. alıştırmanın aynısı !
---
7. Extract all the countries containing only four characters from the countries array and print it as array.
```javascript
for ( let i = 0; i < countries.length; i++) {
    if(countries[i].length === 4 ) {
        console.log(countries[i]);
    }
}
```
---
8. Extract all the countries containing two or more words from the countries array and print it as array.
```javascript
const countriesMoreWords = [];

for ( let i = 0; i < countries.length; i++) {
    if(countries[i].includes(' ')) {
        countriesMoreWords.push(countries[i]);
    }
}

console.log(countriesMoreWords);
```
---
9. Reverse the countries array and capitalize each country and stored it as an array.
```javascript
const countriesReverse = [];

for ( let i = countries.length -1; i >= 0; i--) { 
    countriesReverse.push(countries[i].toUpperCase());
}

console.log(countriesReverse);
```
---





