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

# Arrays 