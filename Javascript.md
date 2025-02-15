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

#### 1] var :
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
- variable have -> `Global scope`
- variables are not binded with any scope. 
- E.g. - var have global scope i.e. its also accessed out of scope also.
```JS
if (true) {
	var age = 23; // variable age in local scope
}

console.log(age); // 23 
// using "var" anyplace we create variable & anytime we accessed it.
```
<br>

- var is `Global Scope`
- Variables are not binded with any scope.
- We create any variable using var, through out program they access anywhere.
- No matter that var created in local function or local if else..
- Using `var` any position we create variable & anytime we access variable.
<br>


#### Special thing of var
E.g. - Give error without defined 
```JS
console.log(age); // give Error age not defined
```
<br>

E.g. - var defined after print, but not give error 
```JS
console.log(age); // undefined // but not give error
// age come first in memory but they not idea about age value i.e. shows `undefined`
var age = 10;   
console.log(age); // 10 
```
<br>

[!NOTE]
> - var -> is global scope but, not same for 'let' & 'const' cases i.e. are Local Scope.
<br>


E.g. - `var` in global scope
```JS
{
	var a = 10;
}
console.log(a); // 10 // a that also access out of scope
```
<br>

[!IMPORTANT]
> - `var` also accessed in console & also change that value in console bcz of global scope.
> - let & const scope always in local.
> - Datatype in JS are assigned Dynamically.
<br>


#### 2] let :
- `Let` always in local scope.
E.g. Wrong but, valid operation in JS
```JS
let age = 22;
age = "Piyush";  // valid operation in JS
console.log(age);
```
<br>

E.g. `let` is in local scope
```JS
if (true) {
	let a = 20;
	console.log(a);  // 20 // a is in local scope
}
console.log(a); // a is not defined // becz, let not global scope 
```
<br>

> [!NOTE]
> - Perfer to choose always `let` as compared with var.
<br>


#### 3] const :
- `const` always local scope.
E.g. - const is in local scope can't access out of scope
```JS
if(true) {
	const a = 10;
}
console.log(a); // a is not defined // becz, let not global scope 
```
<br>

E.g. - const value doesn't re-aasign after defined
```JS
const age = 22; // 22 that value is fixed that not changed after it
age = 30;  // Type Error : Assignment to constant variable
age = "Piyush";  // Type Error : Assignment to constant variable
```
<br>

- `const` always local scope & const value doesn't re-assign after defined.
- In case of const compulsory defined any value (not undefined value of const whenever const is used).
 ```JS
const age; // Error : that not undefined
age = 20; // Is not possible
```
- Access `const` value, operation on it, but `doesn't change age value or its datatype`.
<br>

> [!NOTE]
> - In let & var also work without assign value of variable but const do not work without assign value.
> ```JS
>  let age;
>  console.log(age); // undefined
>  age = 30;
>  console.log(age); // 30
> ```
> - In const case variable doesn't work without initialize becz, const case not undefined at initialize.
> ```JS
>  const age;
>  age = 20;  // not possible
> ```
> - Access, modify const value but, not change that datatype & value.
> ```JS
>  const age = 30;  // that value is fixed
>  console.log(age + 10); // 40 // but not change age value
> ```
<br>

> [!IMPORTANT]
> - Variable -> 3 types of declaration :-
> - var, let, const
> - const - in production 90% used const
<br>

### Difference in between var VS let VS Const

var : Global Scope
- also re-assign var 
- var as global scope (not recommand gets unwanted bug through) 
- access anywhere 

let : Local Scope
- also re-assign let 
-  let as local scope (highly recommended choose 'let' always)
- access it only in self of block 
- let avialable in newer versions of JS

const : Local Scope
- not re-assign const 
- const as local scope (in production 90% used 'const')
- access only in self of block 
<br>

-------------------
<br>

## 3] 




