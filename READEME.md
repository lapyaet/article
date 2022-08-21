
## What is Reference Type?

JavaScript languae ၏ primitive data types မှ ဆင်းသက်လာသော data types ကို non-primitive data types ဟုခေါ်သည်။ non-primitive data types ကို reference data types ဟုလည်း ခေါ်သည်။ Reference data types တွင် array , function, objects တို့ပါဝင်ပါသည်။
##

## What is Object? 
JavaScript object သည် properties နှင့် method ပါရှိသော အရာဖြစ်သည်။ JavaScript သည် object-based language တစ်ခုဖြစ်သည်။ 
အရာအားလုံးသည် javaScript ရှိ object ဖြစ်သည်။
JavaScript သည်  class based မဟုတ်ဘဲ template based  ဖြစ်သည်။ ကျွန်တော်တို့သည် object ပြုလုပ်ရန် class ကို ဖန်းတီးစရာမလို ဘဲ object ကို တိုက်ရိုက် ဖန်တီးနိုင်ပါသည်။
#

## How to create Object? 

Object တစ်ခု ပြုလုပ်ရန် နည်း 3နည်းရှိပါသည်။ 
၎င်းတို့မှာ

1. By object literal
2. By creating instance of Object directly (using new keyword)
3. By using an object constructor (using new keyword)

## 1. By object literal

```javascript
let object = {
    propretie1 : value 1,
    propretie2 : value 2,
    propretie3 : value 3
}
```
## 2. By creating instance of Object directly (using new keyword)

```javascript
let emp=new Object();  
emp.id=101;  
emp.name="Ravi Malik";  
emp.salary=50000;  

```

## 3. By using an object constructor (using new keyword)

```javascript
function emp(id,name,salary){  
this.id=id;  
this.name=name;  
this.salary=salary;  
}  
e=new emp(103,"Vimal Jaiswal",30000);   

```


## Object Properties 

Property Accessories များသည် dot notation သို့မဟုတ် bracket notation ကိုအသုံးပြု၍ object properties များကို ဝင်ရောက်ကြည့်ရှုခွင့်ပေးသည်။


## Examples

```javascript
const person1 = {};
person1['firstname'] = 'Mario';
person1['lastname'] = 'Rossi';

console.log(person1.firstname);
// expected output: "Mario"

const person2 = {
  firstname: 'John',
  lastname: 'Doe'
};

console.log(person2['lastname']);
// expected output: "Doe"
```


## Dot notation 

Object.property syntax တွင် ပိုင်ဆိုင်မှုသည် မှန်ကန်သော JavaScript identifier ဖြစ်ရပါမည်။
(ECMAScript စံနှုန်းတွင် properties name များသည် နည်းပညာအရ "ldentifierName" မဟုတ်ဘဲ "ldentifiers" ဖြစ်သောကြောင့် သီးသန့်စကားလုံးများကို သုံးနိုင်သော်လည်း အကြုံပြုထားခြင်းမရှိပါ။)


## Examples

```javascript
const object = {};
object.$1 = 'foo';
console.log(object.$1);  // 'foo'

```

```javascript
const object = {};
object.1 = 'bar';        // SyntaxError
console.log(object.1);   // SyntaxError

```


## Bracket notation 

object[propertyName] syntax တွင်၊ propertyName သည် string သို့မဟုတ် Symbol တစ်ခုမျှသာဖြစ်သည်။ ထို့ကြောင့် '1foo'၊ '!bar!' သို့မဟုတ် ' ' (space) အပါအဝင် မည်သည့်စာကြောင်းမဆို ဖြစ်နိုင်သည်။


## Examples

```javascript
const variable = object[propertyName];
object[propertyName] = value;
```


## Object.value()

Object.values() method သည် for...in loop မှ ပံ့ပိုးပေးထားသည့် တူညီသော အစီအစဥ်အတိုင်း ပေးထားသော အရာဝတ္ထုတစ်ခု၏ ကိုယ်ပိုင် ကိန်းဂဏန်းပိုင်ဆိုင်မှုတန်ဖိုးများ array တစ်ခုကို ပြန်ပေးသည်။ (တစ်ခုတည်းသော ခြားနားချက်မှာ for...in loop သည် ရှေ့ပြေးပုံစံကွင်းဆက်ရှိ properties ကို ရေတွက်ခြင်းပင်ဖြစ်သည်။)

## Examples

```javascript
const object1 = {
  a: 'somestring',
  b: 42,
  c: false
};

console.log(Object.values(object1));
// expected output: Array ["somestring", 42, false]

```


