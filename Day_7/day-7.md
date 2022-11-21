# 7. Gün Alıştrımaları

## Exercises: Level 1
1. Declare a function fullName and it print out your full name.
```javascript
function fullName () { 
  return console.log('Necati ÇETİNGÜL');
}

fullName();
```
---
2.Declare a function fullName and now it takes firstName, lastName as a parameter and it returns your full - name.
```javascript
function fullName (firstName, lastName) { 
  return console.log(`${firstName} ${lastName}`);
}

fullName('Necati', 'ÇETİNGÜL');
```
---
3. Declare a function addNumbers and it takes two two parameters and it returns sum.
```javascript
function addNumbers (num1, num2) { 
  return num1 + num2 
}

console.log(addNumbers(2,3));
```
---
4. An area of a rectangle is calculated as follows: area = length x width. Write a function which calculates areaOfRectangle.
```javascript
function rectangleArea (length, width) { 
  const area = length * width
  return area;
}

console.log(rectangleArea(5, 3));
```
5. A perimeter of a rectangle is calculated as follows: perimeter= 2x(length + width). Write a function which calculates perimeterOfRectangle.
```javascript
function perimeterOfRectangle (length, width) {
  const perimeter = (length + width) * 2
  return perimeter
}

console.log(perimeterOfRectangle(5, 3));
```
---
6. A volume of a rectangular prism is calculated as follows: volume = length x width x height. Write a function which calculates volumeOfRectPrism.
```javascript
function volumeOfRectPrism (length, width, height) { 
  const volume = length * width * height
  return volume;
}

console.log(volumeOfRectPrism(5, 3, 7));
```
---
7. Area of a circle is calculated as follows: area = π x r x r. Write a function which calculates areaOfCircle
```javascript
const PI = Math.PI;

function circleArea (radius) { 
  const area = PI * radius * radius
  return area;
}

console.log(circleArea(3));
console.log(Math.round(circleArea(3))); // en yakina yuvarlamak için kullanılır.
console.log(circleArea(3).toFixed(2)); // virgülden sonra istenilen kadar sayı lamak için kullanılır.
```
8. Circumference of a circle is calculated as follows: circumference = 2πr. Write a function which calculates circumOfCircle.
```javascript
const PI = Math.PI;

function circumferenceCircle (radius) { 
  const circumference =  2 * PI * radius
  return circumference
}

console.log(circumferenceCircle(3));;
console.log(Math.round(circumferenceCircle(3)));
console.log(circumferenceCircle(3).toFixed(2));
```
---
9. Density of a substance is calculated as follows:density= mass/volume. Write a function which calculates density.
```javascript
const densitySubstance = (mass, volume) =>  mass / volume;

console.log(densitySubstance(20, 3.2));
```
---
10. Speed is calculated by dividing the total distance covered by a moving object divided by the total amount of time taken. Write a function which calculates a speed of a moving object, speed.
```javascript
function calculateSpeed (totalDistance, totaltime) { 
  const speed = totalDistance / totaltime 
  return speed
}

console.log(calculateSpeed(720, 6));
```
---
11. Weight of a substance is calculated as follows: weight = mass x gravity. Write a function which calculates weight.
```javascript
const weight = (mass, gravity) => mass * gravity;

console.log(weight(5, 9.8))
```
---
12. Temperature in oC can be converted to oF using this formula: oF = (oC x 9/5) + 32. Write a function which convert oC to oF convertCelsiusToFahrenheit.
```javascript
function convertCelsiusToFahrenheit (celcius) { 
  const fahrenheit =  (celcius * (9 / 5)) +32
  return fahrenheit;
}

console.log(convertCelsiusToFahrenheit(30));
```
13. Body mass index(BMI) is calculated as follows: bmi = weight in Kg / (height x height) in m2. Write a function which calculates bmi. BMI is used to broadly define different weight groups in adults 20 years old or older.Check if a person is underweight, normal, overweight or obese based the information given below.
* The same groups apply to both men and women.
* Underweight: BMI is less than 18.5
* Normal weight: BMI is 18.5 to 24.9
* Overweight: BMI is 25 to 29.9
* Obese: BMI is 30 or more
```javascript
let mass = Number(prompt('Enter the mass (kg)', ''));
let height = Number(prompt('Enter the height (m)', ''));


function calculateBMI () { 
  const calBMI = mass / (height * height);
  return calBMI;
}

if( calculateBMI().toFixed(2) < 18.5) { 
  console.log(`Underweight BMI = 18.5 --- Your BMI ${calculateBMI().toFixed(2)}`);
} 
else if (calculateBMI().toFixed(2) < 24.9) {
  console.log(
    `Underweight BMI = 18.5 --- Normal weight BMI = 24.9 --- Your BMI ${calculateBMI().toFixed(2)}`
    );
}
else if( calculateBMI().toFixed(2) < 29.9) {
  console.log(
    `Normal weight BMI = 24.9 --- Overweight BMI = 29.9 --- Your BMI ${calculateBMI().toFixed(2)}`
  );
} 
else {
  console.log(
    `Obese BMI is 30 or more --- Your BMI  ${calculateBMI().toFixed(2)}`
  );
}
```
---
14. Write a function called checkSeason, it takes a month parameter and returns the season:Autumn, Winter, Spring or Summer.
```javascript
let month = prompt('Enter the month', '');

month = month.toLowerCase();

function checkSeason () {
  if ( month == 'march' || month == 'april' || month == 'may' ) {
    console.log('Spring');
  }
  else if ( month == 'june' || month == 'july' || month == 'august' ) { 
    console.log('Summer');
  }
  else if ( month == 'september' || month == 'october' || month == 'november') { 
    console.log('Autumn');
  }
  else if ( month == 'december' || month == 'january' || month == 'february') {
    console.log('Winter');
  }
  else {
    console.log('Not a month');
  }
}

checkSeason();
```
---
15. Math.max returns its largest argument. Write a function findMax that takes three arguments and returns their maximum with out using Math.max method.
```javascript
function findMax () { 
    return Math.max.apply(null, arguments);
}

console.log(findMax(-99,24,-13,9,2))

```
---
## Exercises: Level 2
1. Linear equation is calculated as follows: ax + by + c = 0. Write a function which calculates value of a linear equation, solveLinEquation.
```javascript 

```
---
2. Quadratic equation is calculated as follows: ax2 + bx + c = 0. Write a function which calculates value or values of a quadratic equation, solveQuadEquation.
```javascript

```
---
3. Declare a function name printArray. It takes array as a parameter and it prints out each value of the array.
```javscript

```
---
4. Write a function name showDateTime which shows time in this format: 08/01/2020 04:08 using the Date object.
```javascript
const showDateTime = () => {
  const today = new Date();
  let day = today.getDate(),
      month = today.getMonth(),
      year = today.getFullYear(),
      hour = today.getHours(),
      minute = today.getMinutes();
  
      return  `${day}/${month + 1}/${year} ${hour}:${minute}`;
}

console.log(showDateTime());
```
5. Declare a function name swapValues. This function swaps value of x to y.
```javascript

```
---
6. Declare a function name reverseArray. It takes array as a parameter and it returns the reverse of the array (don't use method).
```javascript
const reverseArray = (arr) => { 
  let newArr = [];
  for (let i = 0; i < arr.length; i++) { 
    newArr.unshift(arr[i]) // unshift ya da push kullanımı fark yaratmaz.
  }
  console.log(newArr);
}

reverseArray([1,2,3])
```
---
7. Declare a function name capitalizeArray. It takes array as a parameter and it returns the - capitalizedarray.
```javascript
const capitalizedArray = (arr) => {
  let newArr = [];
  for ( let i = 0 ; i < arr.length; i++) {  
    newArr.push(arr[i].toUpperCase());
  }
  console.log(newArr);
}

capitalizedArray(['de', 'ne', 'me'])
```
---
8. Declare a function name addItem. It takes an item parameter and it returns an array after adding the item.
```javascript

```
---
9. Declare a function name removeItem. It takes an index parameter and it returns an array after removing an item.
```javascript

```
---
10. Declare a function name sumOfNumbers. It takes a number parameter and it adds all the numbers in that range.
```javascript
function sumOfNumber (...item) { 
  let sum = 0;
  for ( let i = 0 ; i < item.length; i++) { 
    sum = sum + item[i];
  }
  return sum;
}

console.log(sumOfNumber(1, 2, 3, 5))
```
11. Declare a function name sumOfOdds. It takes a number parameter and it adds all the odd numbers in that - range.
```javascript
function sumOfOdds (...item) { 
  let sumOdds = 0;
  for (let i = 0; i < item.length; i++) {
    if( item[i] % 2 == 1) { 
      sumOdds = sumOdds + item[i];
    }
  }
  return sumOdds;
}

console.log(sumOfOdds(1,2,3,4,5,7,9));
```
---
12. Declare a function name sumOfEven. It takes a number parameter and it adds all the even numbers in that - range.
```javascript
function sumOfEven (...item) { 
  let sumEven = 0;
  for (let i = 0; i < item.length; i++) { 
    if( item[i] % 2 == 0) { 
      sumEven += item[i];
    }
  }
  return sumEven;
}

console.log(sumOfEven(1,2,3,4,5,6,7,8,9));
```
---
13. Declare a function name evensAndOdds . It takes a positive integer as parameter and it counts number of evens and odds in the number.
```javascript
let allNumber = [];

function evensAndOdds (num) {
  let odd = 0;
  let even = 0;

    for ( let i = 0; i < num+1; i++) {
    allNumber.push(i);
  }

  console.log(allNumber);

  for ( let j = 0; j <= allNumber.length; j++) { 
    if (allNumber[j] % 2 === 0) { 
      even++
    }
    else if (allNumber[j] % 2 === 1) { 
      odd++
    }
  }
  return `the number of odds are ${odd} \nthe number of evens are ${even}`
}

console.log(evensAndOdds(100));
```
---
14. Write a function which takes any number of arguments and return the sum of the arguments
```javascript
function sum (...arg) { 
  let sumAll = 0;
  for( let i = 0; i < arg.length; i++) { 
    sumAll += arg[i]
  }
  return sumAll
}

console.log(sum(1,2,3,4));
```
---
15. Writ a function which generates a randomUserIp.
```javascript
function randomUserIp () { 
  let one = Math.floor(Math.random() * 255);
  let two = Math.floor(Math.random() * 255);
  let three = Math.floor(Math.random() * 255);
  let four = Math.floor(Math.random() * 255);
  return `Ip: ${one}.${two}.${three}.${four}`
}

console.log(randomUserIp());
```
---
16. Write a function which generates a randomMacAddress.
```javascript
const macCharacter = '0123456789ABCDEF';

let partA = new Array(1);
let partB = new Array(1);
let partC = new Array(1);
let partD = new Array(1);
let partE = new Array(1);
let partF = new Array(1);

let mac = ``;

function randomMacAddress () { 
  
  for ( let i = 0; i < 2; i++ ) { 
    partA[i] = macCharacter[Math.round(Math.random() * macCharacter.length)]
  }
  for ( let i = 0; i < 2; i++ ) { 
    partB[i] = macCharacter[Math.round(Math.random() * macCharacter.length)]
  }
  for ( let i = 0; i < 2; i++ ) { 
    partC[i] = macCharacter[Math.round(Math.random() * macCharacter.length)]
  }
  for ( let i = 0; i < 2; i++ ) { 
    partD[i] = macCharacter[Math.round(Math.random() * macCharacter.length)]
  } 
  for ( let i = 0; i < 2; i++ ) { 
    partE[i] = macCharacter[Math.round(Math.random() * macCharacter.length)]
  }
  for ( let i = 0; i < 2; i++ ) { 
    partF[i] = macCharacter[Math.round(Math.random() * macCharacter.length)]
  }
  mac = `${partA[0]}${partA[1]}:${partB[0]}${partB[1]}:${partC[0]}${partC[1]}:${partD[0]}${partD[1]}:${partE[0]}${partE[1]}:${partF[0]}${partF[1]}`;
  return mac
}

console.log(randomMacAddress());
```
---
17. Declare a function name randomHexaNumberGenerator. When this function is called it generates a random hexadecimal number. The function return the hexadecimal number.
```javascript
const hexaNumber = '0123456789ABCDEF';

function randomHexaNumberGenerator () {
let result = '#';

  for(let i = 0; i < 6; i++) {
    result += hexaNumber.charAt(Math.floor(Math.random() * hexaNumber.length));
}
  return result;
}

console.log(randomHexaNumberGenerator());
```
---
18. Declare a function name userIdGenerator. When this function is called it generates seven character id. The function return the id.
```javascript
const idCharacter = 'ABCDEFGHIJKLMNOPRSTUVYZabcdefghijklmnoprstuvyz0123456789';

function userIdGenerator () { 
  let result = '';

  for( let i = 0; i < 7; i++) {
    result += idCharacter.charAt(Math.floor(Math.random() * idCharacter.length))
  }
  return result;
}

console.log(userIdGenerator());
```
---
## Exercises: Level 3
1. Modify the userIdGenerator function. Declare a function name userIdGeneratedByUser. It doesn’t take any parameter but it takes two inputs using prompt(). One of the input is the number of characters and the second input is the number of ids which are supposed to be generated.
```javascript
let ids = [];

function userIdGeneratedByUser () {
  let chars = "0123456789ABCDEFGHIJKLMNOPQRSTUVWXTZabcdefghiklmnopqrstuvwxyz";
  let getID = Number(prompt('how mamy id doyou want to generate', ''));
  let getChars = Number(prompt('how many chars', ''));

      for ( let i = 0; i < getID ; i++ ) { 
        ids[i] = '';
          for ( let j = 0; j < getChars; j++ ) {
            ids[i] += chars[Math.floor(Math.random() * chars.length)];
          }
      }
      console.log(ids);
      for ( let k = 0; k < ids.length ; k++) { 
        console.log(ids[k])
      }
}

console.log(userIdGeneratedByUser ());
```
---
2. Write a function name rgbColorGenerator and it generates rgb colors.
```javascript
function rgbColorGenerator () { 
  let randomA = Math.floor(Math.random() * 255);
  let randomB = Math.floor(Math.random() * 255);
  let randomC = Math.floor(Math.random() * 255);

  return `rgb(${randomA},${randomB},${randomC})`
}

console.log(rgbColorGenerator());
```
3. Write a function arrayOfHexaColors which return any number of hexadecimal colors in an array.
```javascript
const hexaNumber = '0123456789ABCDEF';

function arrayOfHexaColors () { 
  let random = Math.floor(Math.random() * 30);
  let hex = [];

  for ( let i = 0; i < random; i++) { 
      hex[i] = '#'
    for ( let j = 0; j < random; j++) { 
      hex[j] += hexaNumber[Math.floor(Math.random() * hexaNumber.length)];
    }
  }
  return hex;
}

console.log(arrayOfHexaColors());
```
---
4. Write a function arrayOfRgbColors which return any number of RGB colors in an array.
```javascript
function arrayOfRgbColors () { 
  let random = Math.floor(Math.random() * 30);
  let color = [];

  for( let i = 0; i < random; i++) { 
    let randomA = Math.floor(Math.random() * 255);
    let randomB = Math.floor(Math.random() * 255);
    let randomC = Math.floor(Math.random() * 255);
    color[i] = `rgb(${randomA},${randomB},${randomC})`
  }
  return color
}

console.log(arrayOfRgbColors());
```
---
5. Write a function convertHexaToRgb which converts hexa color to rgb and it returns an rgb color.
```javascript

```
---
6. Write a function convertRgbToHexa which converts rgb to hexa color and it returns an hexa color.
```javascript

```
---
7. Write a function generateColors which can generate any number of hexa or rgb colors.
```javascript
function generateColors (type, num) { 
  let chars = "0123456789ABCDEF";
  let color = [];

  if(type === 'rgb') { 
    for(let i = 0; i < num; i++) { 
      color[i] = 'rgb';
      color[i] +=`(${Math.floor(Math.random() * 255)},`
      color[i] += `${Math.floor(Math.random() * 255)},`
      color[i] += `${Math.floor(Math.random() * 255)})`
    }
    }
    else if ( type === 'hex') {
      for (let i = 0; i <num; i++) { 
        color[i] = '#'
        for( let j = 0; j < 6; j++) { 
          color[i] += chars[Math.floor(Math.random() * chars.length)];
        }
      }
  }
  return color
}

console.log(generateColors('rgb', 6));
```
---
8. Call your function shuffleArray, it takes an array as a parameter and it returns a shuffled array.
```javascript
function shuffleArray (arr) { 
  let newArr = [];
    for ( let i = 0; i < arr.length; i++) { 
      let rand = Math.floor(Math.random() * arr.length - 1);
      if (arr.indexOf(rand) !== -1 && !newArr.includes(arr[rand])) {
        newArr.push(arr[rand]);
      }
  }
  return newArr
}

console.log(shuffleArray([1,2,3,4,5,6,7,8,9]));
```
---
9. Call your function factorial, it takes a whole number as a parameter and it return a factorial of the number.
```javascript
let result = 1;
function factorial (num) {
  
  if( Number.isInteger(num) == true) { 
    for( let i = 1; i <= num; i++ ) { 
      result *= i ;    
    }
  }
  return result
}

console.log(factorial(7));
```
---
10. Call your function isEmpty, it takes a parameter and it checks if it is empty or not.
```javascript
function isEmpty (arr) { 
  if (arr === undefined) {
    return 'it is empty'
  }
  else {
    return 'it is not empty'
  }
}

console.log(isEmpty());
```
---
11. Call your function sum, it takes any number of arguments and it returns the sum.
```javascript
function sum  (...arg) { 
  let plus = 0;

    for ( let i = 0; i < arg.length; i++) { 
      plus += arg[i]
    }
      return plus
}

console.log(sum(8,9,10))
```
---
12. Write a function called sumOfArrayItems, it takes an array parameter and return the sum of all the items. Check if all the array items are number types. If not give return reasonable feedback.
```javascript

```
---
13. Write a function called average, it takes an array parameter and returns the average of the items. Check if all the array items are number types. If not give return reasonable feedback.
```javascript

```
---
14. Write a function called modifyArray takes array as parameter and modifies the fifth item of the array and return the array. If the array length is less than five it return 'item not found'.
```javascript

```
---
15. Write a function called isPrime, which checks if a number is prime number.
```javascript.

```
---
16. Write a functions which checks if all items are unique in the array.
```javascript.

```
---
17. Write a function which checks if all the items of the array are the same data type.
```javascript

```
---
18. JavaScript variable name does not support special characters or symbols except $ or _. Write a function isValidVariable which check if a variable is valid or invalid variable.
```javascript

```
---
19. Write a function which returns array of seven random numbers in a range of 0-9. All the numbers must be unique.
```javascript

```
---
20. Write a function called reverseCountries, it takes countries array and first it copy the array and returns the reverse of the original array
```javascript

```






































