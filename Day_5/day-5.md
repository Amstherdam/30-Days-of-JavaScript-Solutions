# 5. Gün Alıştrımaları
## Exercises: Level 1
1. Declare an empty array.
```javascript
const arr = [];
```
---
2. declare an array with more than 5 number of elements.
```javascript
const arrMarvel = ['Black panther', 'Thor', 'Iron Man', 'Captain America','Hulk', 'Doctor Strange']
```
---
3. Find the length of your array.
```javascript
const arrMarvel = ['Black panther', 'Thor', 'Iron Man', 'Captain America','Hulk', 'Doctor Strange']

console.log('Number of arrMarvel ',arrMarvel.length);
```
---
4. Get the first item, the middle item and the last item of the array.
```javascript
const arrMarvel = ['Black panther', 'Thor', 'Iron Man', 'Captain America','Hulk', 'Doctor Strange']

console.log(arrMarvel[0]);
console.log(arrMarvel[2],'-', arrMarvel[3]);
console.log(arrMarvel[arrMarvel.length - 1]); //Son item
```
---
5. Declare an array called mixedDataTypes, put different data types in the array and find the length of the array. The array size should be greater than 5.
```javascript
const mixedDataTypes = [
    'Thor',
     true,
     200,
     {country: 'Asgard', city: '-'},
     {skills: ['strength', 'speed', 'agility', 'durability', 'immunity']}
     ]
```
---
6. Declare an array variable name itCompanies and assign initial values Facebook, Google, Microsoft, Apple, IBM, Oracle and Amazon
```javascript
const itCompanies = ['Facebook', 'Google', 'Microsoft', 'Apple', 'IBM', 'Orcale', 'Amazon']
```
---
7. Print the array using console.log().
```javascript
const itCompanies = ['Facebook', 'Google', 'Microsoft', 'Apple', 'IBM', 'Orcale', 'Amazon']

console.log(itCompanies);
```
---
8. Print the number of companies in the array.
```javascript
const itCompanies = ['Facebook', 'Google', 'Microsoft', 'Apple', 'IBM', 'Orcale', 'Amazon']

console.log('itCompanies:' ,itCompanies.length);
```
9.Print the first company, middle and last company.
```javascript
const itCompanies = ['Facebook', 'Google', 'Microsoft', 'Apple', 'IBM', 'Orcale', 'Amazon']

console.log(itCompanies[0]);
console.log(itCompanies[3]);
console.log(itCompanies[itCompanies.length - 1]);
```
---
10. Print out each company. 
```javascript
const itCompanies = ['Facebook', 'Google', 'Microsoft', 'Apple', 'IBM', 'Orcale', 'Amazon']

itCompanies.forEach(element => console.log(element));
```
```javascript
const itCompanies = ['Facebook', 'Google', 'Microsoft', 'Apple', 'IBM', 'Orcale', 'Amazon']

for(let i = 0; i < itCompanies.length; i++){
    console.log(itCompanies[i]);
}
```
* Bu bölümde ilk örnek forEach() fonksiyonu kullanılarak yapılmıştır. İkinci örnek ise for döngüsü ile yapılmıştır. Gözünüz korkmasın bunların daha anlatılmadığının farkındayım ama sadece göz aşinalığı kazanmak için inceleyebilirsiniz. İsterseniz daha önceki örneklerde olduğu gibi console.log() ile yazdırabilirsiniz.
```javascript
const itCompanies = ['Facebook', 'Google', 'Microsoft', 'Apple', 'IBM', 'Orcale', 'Amazon']

console.log(itCompanies[0], itCompanies[1], itCompanies[2], itCompanies[3], itCompanies[4], itCompanies[5], itCompanies[6]);
```
---
11. Change each company name to uppercase one by one and print them out
```javascript

const itCompanies = ['Facebook', 'Google', 'Microsoft', 'Apple', 'IBM', 'Orcale', 'Amazon']

console.log(itCompanies[0].toUpperCase());
console.log(itCompanies[1].toUpperCase());
console.log(itCompanies[2].toUpperCase());
console.log(itCompanies[3].toUpperCase());
console.log(itCompanies[4].toUpperCase());
console.log(itCompanies[5].toUpperCase());
console.log(itCompanies[6].toUpperCase());
```
---
12. Print the array like as a sentence: Facebook, Google, Microsoft, Apple, IBM,Oracle and Amazon are big IT companies.
```javascript
const itCompanies = ['Facebook', 'Google', 'Microsoft', 'Apple', 'IBM', 'Orcale', 'Amazon']

const lastItem = itCompanies.pop();

const newString = itCompanies.join(', ');

console.log(`${newString} and ${lastItem} are big IT companies.`)
```
---
13. Check if a certain company exists in the itCompanies array. If it exist return the company else return a company is not found
```javascript
const itCompanies = ['Facebook', 'Google', 'Microsoft', 'Apple', 'IBM', 'Orcale', 'Amazon']

console.log(itCompanies.indexOf('Apple')); // 3

console.log(itCompanies.indexOf('Blizzard')); // -1
```
```javascript
const itCompanies = ['Facebook', 'Google', 'Microsoft', 'Apple', 'IBM', 'Orcale', 'Amazon'];

let searchITComp = prompt('Enter company to search','');
if (itCompanies.includes(searchITComp)) {
    console.log(searchITComp);
}
else{
    console.log('company not found.');
}
```
* Hangisini sormak istediğini anlamadıpım için iki farklı yöntemle yaptım.
---
14.Filter out companies which have more than one 'o' without the filter method.
```javascript

```
---
15. Sort the array using sort() method.
```javascript
const itCompanies = ['Facebook', 'Google', 'Microsoft', 'Apple', 'IBM', 'Orcale', 'Amazon']

console.log(itCompanies.sort());
```
---
16. Reverse the array using reverse() method.
```javascript
const itCompanies = ['Facebook', 'Google', 'Microsoft', 'Apple', 'IBM', 'Orcale', 'Amazon']

console.log(itCompanies.reverse());
```
---
17. Slice out the first 3 companies from the array.

```javascript
const itCompanies = ['Facebook', 'Google', 'Microsoft', 'Apple', 'IBM', 'Orcale', 'Amazon']

console.log(itCompanies.slice(0,3));
```
---
18. Slice out the last 3 companies from the array.
```javascript
const itCompanies = ['Facebook', 'Google', 'Microsoft', 'Apple', 'IBM', 'Orcale', 'Amazon']

console.log(itCompanies.slice(4,7));
```
---
19. Slice out the middle IT company or companies from the array.
```javascript
const itCompanies = ['Facebook', 'Google', 'Microsoft', 'Apple', 'IBM', 'Orcale', 'Amazon']

console.log(itCompanies.slice(3,4));
```
---
20. Remove the first IT company from the array.
```javascript
const itCompanies = ['Facebook', 'Google', 'Microsoft', 'Apple', 'IBM', 'Orcale', 'Amazon']

itCompanies.shift();
console.log(itCompanies);
```
---
21. Remove the middle IT company or companies from the array.
```javascript
const itCompanies = ['Facebook', 'Google', 'Microsoft', 'Apple', 'IBM', 'Orcale', 'Amazon']

itCompanies.splice(3,1);
console.log(itCompanies);
```
---
22. Remove the last IT company from the array.
```javascript
const itCompanies = ['Facebook', 'Google', 'Microsoft', 'Apple', 'IBM', 'Orcale', 'Amazon']

itCompanies.pop();
console.log(itCompanies);
```
---
23. Remove all IT companies.
```javascript
const itCompanies = ['Facebook', 'Google', 'Microsoft', 'Apple', 'IBM', 'Orcale', 'Amazon']

let denem = itCompanies.splice(0, 7);
console.log(itCompanies);
```

```javascript
const itCompanies = ['Facebook', 'Google', 'Microsoft', 'Apple', 'IBM', 'Orcale', 'Amazon']

itCompanies.length = 0;
console.log(itCompanies);
```
---
## Exercises: Level 2
1.Create a separate countries.js file and store the countries array in to this file, create a separate file web_techs.js and store the webTechs array in to this file. Access both file in main.js file.
```javascript
export const countries = [   // countries.js 
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
```
```javascript
export const webTechs = [    // web_techs.js
    'HTML',
    'CSS',
    'JavaScript',
    'React',
    'Redux',
    'Node',
    'MongoDB'
  ]
```
```javascript
import {countries} from './countries.js'  // main.js
import {webTechs} from './web_techs.js'

console.log(countries);
console.log(webTechs);
```
---
2. First remove all the punctuations and change the string to array and count the number of words in the array.
```javascript 
let text = 'I love teaching and empowering people. I teach HTML, CSS, JS, React, Python.';
console.log(text, typeof text);

text = text.replace(/[^a-zA-Z ]/g, ''); // noktalama işaretleri çıkartıldı.
console.log(text, typeof text);

text = text.split(' ');                 // array a dönüştürüldü.
console.log(text, typeof text, text.length);
```
---
3. In the following shopping cart add, remove, edit items.
* add 'Meat' in the beginning of your shopping cart if it has not been already added.
* add Sugar at the end of you shopping cart if it has not been already added.
* remove 'Honey' if you are allergic to honey.
* modify Tea to 'Green Tea'.
```javascript
const shoppingCart = ['Milk', 'Coffee', 'Tea', 'Honey'];

shoppingCart.unshift('Meat');
shoppingCart.push('Sugar');
shoppingCart.splice(4,1);
shoppingCart[3] = 'Green Tea'

console.log(shoppingCart);
```
---
4. In countries array check if 'Ethiopia' exists in the array if it exists print 'ETHIOPIA'. If it does not exist add to the countries list.
```javascript
import {countries} from './countries.js'

if(countries.includes('Ethiopia')) { 
    console.log('ETHIOPIA');
} else (
    countries.push('Ethiopia');
)
```
---
5. In the webTechs array check if Sass exists in the array and if it exists print 'Sass is a CSS preprocess'. If it does not exist add Sass to the array and print the array.

```javascript
import {webTechs} from './web_techs.js'

if(webTechs.includes('Sass')) {
    console.log('Sass is a CSS preprocess.')
} else { 
    webTechs.push('Sass');
    console.log(webTechs);
}
```
---
6. Concatenate the following two variables and store it in a fullStack variable.
```javascript
const frontEnd = ['HTML', 'CSS', 'JS', 'React', 'Redux']
const backEnd = ['Node','Express', 'MongoDB']

const fullStack = frontEnd.concat(backEnd);

console.log(fullStack);
```
## Exercises: Level 3
1. The following is an array of 10 students ages:
* Sort the array and find the min and max age.
* Find the median age(one middle item or two middle items divided by two).
Find the average age(all items divided by number of items).
* Find the range of the ages(max minus min).
*Compare the value of (min - average) and (max - average), use abs() method 1.Slice the first ten countries from the countries array
.
```javascript
const ages = [19, 22, 19, 24, 20, 25, 26, 24, 25, 24]

ages.sort();
console.log(ages[0]);               // min age
console.log(ages[ages.length - 1]); // max age

--------------------------------------------------------
let totalAge = 0;      // find the average age
let avgAge;
for(let i = 0; i < ages.length; i++) { 
    totalAge += ages[i];
    avgAge = totalAge / ages.length;
}

console.log(avgAge);  // 22.8
---------------------------------------------------------
ages.sort();
console.log(ages[ages.length- 1] - ages[0]);
---------------------------------------------------------
let minAge = ages.sort()[0];
let maxAge = ages.sort()[ages.length - 1];

console.log(Math.abs(minAge - avgAge));
console.log(Math.abs(maxAge - avgAge));
```
---
2. Find the middle country(ies) in the countries array.
```javascript
import {countries} from './countries.js'

console.log(countries.slice(0, 10));
console.log(countries[(countries.length - 1 ) / 2 ]);
```
---
3. Divide the countries array into two equal arrays if it is even. If countries array is not even , one more country for the first half.

```javascript
import {countries} from './countries.js'

console.log(countries.slice(0,((countries.length - 1) / 2)));
```














