# Javascript - Piyush Garg

#### `07-02-25`

## Introduction to Javascript

- JS is just a programming language for web applications
- Internal Linking : Write the JS code inside the HTML file.
- External Linking : Write the JS code in seprate .js file.
- `;` not compulsory in JS.
<br>

-------------------
<br>

## 2] Variables in Javascript
<br>

> [!NOTE]
> - Variable is only memory name for storing data.

### Varaibles 
<br>

1] var :
- var is a keyword, which stand for variable
- old time in JS only `var` is present for creating variable.
<br>
  
> [!NOTE]
> - DataType varName = value; -> strongly Typed Languages in Java, C, C++
> - `if we give one datatype that datatype only can followed` in strongly Typed Languages.
<br>

> [!IMPORTANT]
> - JS is loosely typed language
> - In loosely typed no any datatype present i.e. `dynamically assign datatype`.
<br>

#### JS is loosely typed language
```JS
var age = 22; // loosely typed language -> auto or implicitly assign int
console.log(age);
```
<br>

- do not give data types in JS.
- JS interpreter that run JS, they automatically find which datatype is assigned.
- JS interpreter adjusts `Datatypes accordingly. 
  
```JS
var age = 22;
console.log(age);
age = "Piyush"; // datatype value change in during Run Time
console.log(age);
```

#### Drawback of loosely typed
- Technically lossely typed that is wrong & its `create bugs when we as experience developer`. - Lossely typed is  behaviour of JS & i.e. allowed in JS.
<br>

#### Naming Convention - 
- Variable name rule -
  - Variable name only start with alphabet.
  - Spaces are not allowed in varaible name.
  - also not put `-` on variable name.
  - Put `_` is valid for variable name for seprate.
- Follow Camel Casing - e.g.
  - firstName // most prefered way for `variable name`
  - FirstName // mostly used for `classes`
<br>

#### var property - 
- variables have -> `Global scope`
- variables are not binded with any scope. 
- E.g. - var have global scope 
```JS
if (true) {
	var age = 23; // variable age in local scope
}

console.log(age); // 23 
// using "var" anyplace we create variable & anytime we accessed it.
```

10 min 





E.g. 

console.log(age); // give Error age not defined
---

after-->

console.log(age);   // undefined 
var age = 10;   
console.log(age); // 10 

// var -> global scope but not same for 'let' & 'const' cases 

var global scope e.g. -

{
	var a = 10;
}

console.log(a); // 10 // --> that also access out of scope

// var also accessed in console & also change that value in console bcz of global scope.


// let & const scope always in local
// Datatype in JS are assigned Dynamically.

2] Let : 

let age = 22;

age = "Piyush";  // valid operation in JS

console.log(age);

// let scope always in local


let local scope e.g. -

if (true) {
	let a = 20;
}

console.log(a); // a is not defined // becz, let not global scope 

------------

if (true) {
	let a = 20;
	console.log(a);  // 20
}



3] const :

const local scope e.g. -

if(true) {
	const a = 10;
}

console.log(a); // a is not defined // becz, let not global scope 




e.g. const value doesnot re-aasign

const age = 22; 

age = "Piyush";  // Type Error : Assignment to constant variable
// const value doesnot re-assign


// In let & var also work without assign value of variable but cost do not work without assign value
e.g. 

let age;

console.log(age); // undefined

age = 30;

console.log(age); // 30


// In const case variable doesn't work without initialize becz, const case not undefined at initialize 

const age;

age = 20;  // not possible


// access, modify const value but not change that datatype & value e.g.

const age = 30;  // that value is fixed

console.log(age + 10); // 40 // but not change age value


-----
Difference between var vs let

var : Global Scope
// re-assign var 
// var as global scope ( not recommand gets unwanted bug through) 
// access anywhere 

let : Local Scope
// re-assign let 
// let as local scope (highly recommended choose 'let' always)
// access only in self of block 
// let avialable in newer versions of JS

const : Local Scope
// not re-assign const 
// const as local scope (in production 90% used 'const')
// access only in self of block 

---------


Variable -> 3 types of declaration
var, let, const


const - in production & 90% used const

