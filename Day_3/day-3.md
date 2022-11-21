# 3. Gün Alıştrımaları

## Exercises: Level 1


1. Declare firstName, lastName, country, city, age, isMarried, year variable and assign value to it and use the typeof operator to check different data types.

> 
```javascript
let firstName = 'Necati',
    lastName = 'ÇETİNGÜL',
    country =   'Türkiye', 
    city = 'İzmir',
    age = 27,
    isMarried = false ,
    year = 2022;

console.log(typeof firstName);      // string
console.log(typeof lastName);       // string  
console.log(typeof country);        // string
console.log(typeof city);           // string
console.log(typeof age);            // number
console.log(typeof isMarried);      // boolean
console.log(typeof year);           // number
```

---
2. Check if type of '10' is equal to 10.

```javascript
let a = 10;
let b = '10'

console.log(a == b);   // true
console.log(a === b); //  false
```

---

3. Check if parseInt('9.8') is equal to 10.

```javascript
console.log(parseInt('9.8') == 10);   
```
---

4. Boolean value is either true or false.

- Write three JavaScript statement which provide truthy value.
- Write three JavaScript statement which provide falsy value.

---
```javascript
let isLightOn = true;
let value = 4 > 3;
let nam = 1;

let namTwo = 0;
let isLightOff = false;
let valueTwo = 4 < 2;
```
---
5. Figure out the result of the following comparison expression first without using console.log(). After you decide the result confirm it using console.log().

```javascript
 4 > 3      //  true
 4 >= 3     //  true
 4 < 3      //  false
 4 <= 3     //  false
 4 == 4     //  true
 4 === 4    //  true
 4 != 4     //  false
 4 !== 4    //  false
 4 != '4'   //  false
 4 == '4'   //  true
 4 === '4'  //  false
```

---
6. Figure out the result of the following expressions first without using console.log(). After you decide the result confirm it by using console.log().

```javascript
4 > 3 && 10 < 12        //  true
4 > 3 && 10 > 12        //  false
4 > 3 || 10 < 12        //  true
4 > 3 || 10 > 12        //  true
!(4 > 3)                //  false
!(4 < 3)                //  true
!(false)                //  true
!(4 > 3 && 10 < 12)     //  false
!(4 > 3 && 10 > 12)     //  true 
!(4 === '4')            //  true
```
---

7. Use the Date object to do the following activities.

```javascript
const today = new Date();

let year = today.getFullYear(),

    month = today.getMonth(),

    day = today.getDate(),

    dayInWeek = today.getDay();

    hour = today.getHours(),

    minute = today.getMinutes(),

    allSeconds = today.getTime();

    console.log(year , month , day , dayInWeek , hour , minute , allSeconds );
```

---

## Exercises: Level 2

1. Write a script that prompt the user to enter base and height of the triangle and calculate an area of a triangle (area = 0.5 x b x h).

> ***Bu bölümde istenilenler fonksiyon oluşturularak yapılmıştır.*** 
```javascript

// Kullanılan Number() özelliği prompt() ile alınan verinin string veri türünden number veri türüne değişmesi için kullanılır. Bu işlem gereklidir.

let base = Number(prompt('Üçgenin tabanını giriniz'), '');  
let height = Number(prompt('Üçgenin yüksekliğini giriniz'), '');

function triangleArea() { 
    return base * height * 0.5
}

console.log(triangleArea());
```
---

2. Write a script that prompt the user to enter side a, side b, and side c of the triangle and and calculate the perimeter of triangle (perimeter = a + b + c).

```javascript

let sideA = Number(prompt('Üçgenin A kenarının uzunluğu', ''));
let sideB = Number(prompt('Üçgenin B kenarının uzunluğu', ''));
let sideC = Number(prompt('Üçgenin C kenarının uzunluğu', ''));

function  trianglePrimeter () { 
    return sideA + sideB + sideC
}

console.log(trianglePrimeter());
```
---
3. Get length and width using prompt and calculate an area of rectangle (area = length x width and the perimeter of rectangle (perimeter = 2 x (length + width)).

```javascript

let length = Number(prompt('Dikdortgenin kısa kenarı'));
let width = Number(prompt('Dikdortgenin geniş kenarı'));

function rectanglePerimeter () {
    return `Dikdörtgenin alanı = ${length * width} Dikdörtgenin genişliği = ${2 * (length + width)}`
}

console.log(rectanglePerimeter()); 
```
---
4. Get radius using prompt and calculate the area of a circle (area = pi x r x r) and circumference of a circle(c = 2 x pi x r) where pi = 3.14.

```javascript
let radius = Number(prompt('Yari cap giriniz', ''));
const PI = 3.14;

function circle () { 
    return `Dairenin alanı = ${PI * radius* radius} Dairenin genişliği = ${2 * PI * radius}`
}

console.log(circle ()); 
```
---

5. ***5-8 arasındaki sorular daha çok matamatik gerektirdiği için atlanmıştır.***
---
9. Writ a script that prompt a user to enter hours and rate per hour. Calculate pay of the person?

```javascript
let hourInAWeek = Number(prompt('Haftada kac saat çalisiyorsunuz?', ''));
let ratePerHour = Number(prompt('Saatlik ucretiniz ne kadar?', ''));

function weekly () {
    return (hourInAWeek * ratePerHour);
}

console.log(weekly());
```
---
10. If the length of your name is greater than 7 say, your name is long else say your name is short.

```javascript
let name  = prompt('Adınızı giriniz ', '');

function theName () {
    return (name.length > 7) ? 'adınız uzun' : 'adınız kısa' 
}

console.log(theName()); 
```
---
11. Compare your first name length and your family name length and you should get this output.

```javascript
let firstName = 'Necati';
let lastName = 'ÇETİNGÜL';

function theLonger() {
    return (firstName.length > lastName.length) ? 
    `Your first name, ${firstName} is longer than your family name, ${lastName}` : 
    `Your first name, ${firstName} is shorter than your family name, ${lastName}`
}

console.log(theLonger()); 
```
---
12. Declare two variables myAge and yourAge and assign them initial values and myAge and yourAge.

```javascript
let myAge = 250 ;
let yourAge = 25 ;

console.log((myAge > yourAge) ? 
    `I am ${myAge - yourAge} years older than you.` : 
    `You are ${yourAge - myAge} years older than me.`
);
```
---
13. Using prompt get the year the user was born and if the user is 18 or above allow the user to drive if not tell the user to wait a certain amount of years.
```javascript
let birthYear = Number(prompt('Enter your birth year', ''));

let today = new Date();
let year = today.getFullYear();

function driveCar () { 
    return ((year - birthYear) >= 18) ?
    `You are ${year-birthYear}. You are old enough to drive`:
    `You are ${year - birthYear}. You will be allowed to drive ${18 - (year - birthYear)}`
}

console.log(driveCar());
```
---
14. Write a script that prompt the user to enter number of years. Calculate the number of seconds a person can live. Assume some one lives just hundred years.

```javascript
let getAge = Number(prompt('Yaşınızı giriniz', ''));

function ageLong () { 
    return `You lived ${getAge * 365 * 24 * 60 * 60} seconds.`
}
    
console.log(ageLong());
```
---
15. Create a human readable time format using the Date time object.

```javascript
const today = new Date();

let year = today.getFullYear(),
    month = (today.getMonth()) + 1,
    day = today.getDate(),
    hour = today.getHours(), 
    minute = today.getMinutes();

console.log(`${year}-${month}-${day} ${hour}:${minute}`);
console.log(`${day}-${month}-${year} ${hour}:${minute}`)
console.log(`${day}/${month}/${year} ${hour}:${minute}`) 
```
---
## Exercises: Level 3

1. Create a human readable time format using the Date time object. The hour and the minute should be all the time two digits (7 hours should be 07 and 5 minutes should be 05 ).

```javascript
const today = new Date();

let year = today.getFullYear(),
    month = (today.getMonth()) + 1,
    day = today.getDate(),
    hour = today.getHours(), 
    minute = today.getMinutes();

    month = month < 10 ? '0' + month : month;  
    day = day < 10 ? '0' + day : day;
    hour = hour < 10 ? '0' + hour : hour;       // Saat 10'dan küçük ise başına sıfır ekle
    minute = minute < 10 ? '0' + minute : minute;

console.log(`${year}-${month}-${day} ${hour}:${minute}`);

```
---
<br><br>

***Alıştırmaların yapımı sırasında yazım hataları bulunabilir, elimden geldiğince dikkat etmeye çalıştım hatam varsa affola!***






