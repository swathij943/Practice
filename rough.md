# JavaScript -- Javascript is a programing language for the development of interactive webapplications. its a versatile & high level programming language.

## JavaScript is object based -- Objects are created using object literals/constructors. objects have properties and mentods.

## JavaScript is event driven -- JS allows you to write codes that are event driven, that responds to events like buttons, forms etc.

## JavaScript is prototype based -- objects can inherits properties & behaviours of other objects.

## Its a functional programming language - we can write code using functions.

# There are 6 types of primitive data types in JS as listed beliw
1. undefined 
2. null
3. string
4. number
5. boolean
6. symbol

# Objects -- Objects are entities that allows you to store & organize data using Key:Vale pairs in {}

1. Creating Objects using Object Literals & Constructor

eg: 

const person = {
  name: "Alex",
  age: 25,
  gender: "male"
};

Constructor function - uses regular functions used with 'new' keyword to create instances of object.

eg:

function Person(name, age, gender) {
  this.name = name;
  this.age = age;
  this.gender = gender;
}

const Alex = new Person ('Alex', 26, 'Male');

2. Accessing Object Properties

>> Using Dot notation --- console.log(person.name);

>> Using Bracket notation --- console.log(person['name']);

3. Modifying Objects --- Can modify objects using assignment operators

eg: 
person.age = 26;

or

person['name'] = 'Peter';

4. Adding & Deleting Object Properties

eg:

*add

person.city = 'london';

*delete

delete person.city;

5. Iterating over object properties -- using loop (for in)

eg:

for (let key in Person) {
  console.log(key + ':' + person[key]);
}

>> built in method is using Object.keys()

eg:

Object.keys(person),forEach(
  key => {
    console.log(key + ':' person[key]);
  }
);

6. Object Methods -- Objects can also have methods, which are function assigned as properties. These methods can perform actions or computations.

eg:

const calculator = {
  add : function (a, b) {
    return a+b;
  },
  multiply : function (a, b) {
    return a*b;
  },
  subract : function (a,b) {
    return a-b;
  },
  console.log(calculator.add(5,3));
}

# Arrays -- Arrays are used to store collection of dats

1. Creating an Array
>> Using Array literals -- uses [] separated by ,

eg:

const numbers = [1, 2, 3, 4, 5];
const fruits = ["apple", "orange", "lemon"];

>> Array Constructors -- uses new keyword

eg:

const numbers = new Array(1, 2, 3, 4, 5);

const fruits = new Array('apple', 'orange', 'pineapple');

2. Accessing Array Elements -- they are accessed using the Index.

eg:

console.log(numbers[0]);

o/p -- 1

console.log(fruits[2]);

o/p -- lemon

3. Modifying Array Elements -- Arrays can be modified by assisgning a new value in index.

eg:

numbers[2] = 10;
console.log(numbers);

o/p -- 1, 2, 10, 4, 5

4. Array Length - no: of elements in the array

console.log(numbers.length);

o/p -- 5

console.log(fruits.length);

o/p -- 3

5. Adding & Removing Array Elements

add -- Push()

eg: 

numbers.push(6);
console.log(numbers);

o/p -- 1, 2, 3, 4, 5, 6

remove -- Pop()

eg:

numbers.pop()
console.log(numbers);

o/p -- 1, 2, 3, 4, 5


6. Iterating over array elements - using loops 

>> For 

for (let i = 0; i < numbers.length; i++) {
  console.log(numbers[i]);
}


>> For of

for (let number of numbers) {
  console.log(number);
}

>> forEach

numbers.forEach(function(number) {
  console.log(number);
});

7. Array Methods

>> concat() -- combines 2 or more arrays & returns a new array.

eg:

const fruits = ['apple'];
const vegetables = ['carrot'];

const combined = fruits.concat(vegetables);
console.log(combined);

o/p - ['apple', 'carrot'];

>> slice() -- Extracts a section of array & returns a new array

eg:

const numbers = [1, 2, 3, 4, 5];
const sliced = numbers.slice(2,4);
console.log(sliced);

o/p -- [1, 3, 5];

>> splice() -- adds or remove elements from an array at a specific index.

eg:

add element


const numbers = [1, 2, 3, 4, 5];
numbers.splice(2, 0, 6, 7);
console.log(numbers);

o/p -- [1, 2, 6, 7, 3, 4, 5]

remove

numbers.splice(4,2);
console.log(numbers);

o/p -- [1, 2, 6, 7, 5];

>> indexOf() -- returns -- intex of 1st occurence of a specified element

const numbers = [1, 2, 3, 4, 5];
const index = numbers.index(3);

o/p -- 2

>> join() -- joins all elements of an array into a string

const fruits = ['apple', 'orange'];
const joined = fruits.join('-');

o/p --['apple - orange'];

>> sort() -- sorts elements of an array.

const numbers = [5, 4, 1, 3, 2];
numbers.sort();
console.log(numbers);

o/p -- [1, 2, 3, 4, 5];

>> reverse() -- reverse order of elements in array.

const numbers = [1, 2, 3, 4, 5];
numbers.revers();
console.log(numbers);

o/p -- [5, 4, 3, 2, 1];

