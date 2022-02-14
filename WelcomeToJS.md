#### DataTypes
<pre><code>console.log("hello");
console.log("hello "+"gb39");
console.log(12+4);
---
hello
hello gb39
16
</code></pre>

#### Variables(const and let)
<code>const</code> doesn't change the value<br/>
<code>let</code> can change the value<br/>
and when you what to upadate value you can just write <code>[variable] = [value]</code><br/>
we don't use <code>var</code> any more<br/>
always <code>const</code> sometimes <code>let</code> never <code>var</code>
<pre><code>
const a = 5;
let MyName = jim;

MyName = "gb39";
a=7;

console.log (a);
console.log(MyName);
---
Uncaught TypeError: Assignment to constant variable.
</code></pre>

#### Boolean
<pre><code>const amIFat = true;
const amITall = false;
const areYouSure = null;
const strong;

console.log("amIFat");
console.log("amITall");
console.log("areYouSure");
console.log("strong");
---
true
false
null
undefined
</code></pre>
<code>null</code> means nothing, but it is defined.<br/>
<code>undefined</code> is variable but undefined.<br />

#### Array
<pre><code>const dayOfWeek = ["mon", "tue", "wed", "thu", "fri", "sat"];
const nonsense = [1, 2, "hello", false, null, true, undefined, "gb39"];

console.log(dayOfWeek, nonsense, dayOfWeek[3]);

//Add one more day to the array
dayOfWeek.push("sun");

console.log(dayOfWeek);
---
['mon', 'tue', 'wed', 'thu', 'fri', 'sat'] [1, 2, 'hello', false, null, true, undefined, 'gb39'] 'thu'
['mon', 'tue', 'wed', 'thu', 'fri', 'sat', 'sun']</code></pre>
use <code>[variable].push("[value]")</code> to add array value

#### Object
<pre><code>//entity
const player = {
  //property
  name: "gb39",
  HP: 30,
  point: 3,
 };
 
console.log(player, player.name);
player.HP = 100;
player.fat = true;
console.log(palyer)
---
{name: 'gb39', HP: 30, point: 3} 'gb39'
{name: 'gb39', HP: 100, point: 3, fat: true}
</code></pre>

you can use value by typing <code>[entity].[property]</code> <br/>
and just write <code>[entity].[property] = [value]</code> to add or change property 

#### Function 
you can use function in object just like line:3,4,5 in script just down here
<pre><code>const npc = {
    name: "gb39",
    sayHello: function (otherPersonsName){
        console.log("hello " + otherPersonsName + " how's the day");
    },
};

function add(a,b){
    console.log(a+b);
}

npc.sayHello("jim");
add(3,4);
---
hello jim how's the day
7</code></pre>

#### Others
with th function <code>typeof</code> we can know the type of the value.<br/>
and with <code>parseInt</code> we can change other datatype to int.<br/>
if the value is text, the result would be NaN.
<pre><code>const age = prompt("How old are you");

console.log(typeof age, age, parseInt(age));
---
string 15(string) 15(int)</code></pre>

<pre><code>const age = parseInt( prompt("How old are you"));

console.log(typeof age, age);
---
int 15(int)</code></pre>

#### conditional
<pre><code>const age = parseInt( prompt("How old are you"));

if (isNaN(age)){
    console.log("please write a number"); // use isNaN() to check is age int.
} else if (age < 18){
    console.log("you are too young");
} else if (age >=18 && age <=50){
    console.log("You can drink");
}else if (age >50 && age <80){
    console.log("you should exercise");
}else {
    console.log("you can do whatever you want");
}</code></pre>
