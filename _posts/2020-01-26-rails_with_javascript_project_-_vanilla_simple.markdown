---
layout: post
title:      "Rails with JavaScript Project - Vanilla Simple"
date:       2020-01-26 23:29:41 +0000
permalink:  rails_with_javascript_project_-_vanilla_simple
---


  This is my fourth project and by far the easiest. What can I say? I like vanilla JavaScript and vanilla ice cream too.
	
	Everyone raves about the "magic" of Rails, but in my humble yet professional (former engineer) opinion JavaScript is the MAGIC! 
	
	
	
	
	
	Here are few examples:
	
	/*******************************************
 *
 *   Javascript Magic Page
 *
 *   Author: Sergey Ivanov <xufocoder@gmail.com>
 *
 *          (\_/)
 *         (=':'=)
 *      ▀▀▀███████▀▀▀
 *         ███████
 *         ███████
 *
 *   Gist for javascript beginners
 *   programmers to show implicit behavior
 *
 ******************************************/


/***************
 * Type of Magic
 ****************/

console.log(typeof null);
// output: object

console.log(null instanceof Object);
// output: false

console.log(typeof NaN);
// output: number

console.log(typeof function () {
});
// output: function
// but there's no function type http://ecma-international.org/ecma-262/5.1/#sec-8


/****************
 * Compare magic
 ****************/

console.log('' == '0');
// output: false

console.log(0 == '');
// output: true

console.log(0 == '0');
// output: true

console.log(false == 'false');
// output: false

console.log(false == '0');
// output: true

console.log(false == undefined);
// output: false

console.log(false == null);
// output: false

console.log(null == undefined);
// output: true

console.log(' \t\r\n ' == 0);
// output: true

console.log("abc" == new String("abc"));
// output: true

console.log("abc" === new String("abc"));
// output: false

console.log(0.1 + 0.2 == 0.3);
// output: false
// sum of float values is not equeals obvious float value

console.log(NaN != NaN);
// output: true

console.log(NaN == NaN);
// output: false

console.log(NaN === NaN);
// output: false

console.log(!!undefined);
// output: false

console.log(!!NaN);
// output: false

console.log(!!null);
// output: false

console.log([1, 2, 3] == [1, 2, 3]);
// output: false
// How to detect array equality in JavaScript?

console.log(new Array(3) == ",,");
// output: true

console.log(new Array(3) === ",,");
// output: false

console.log("a" > "b");
// output: true

console.log("abcd" < "abcd");
// output: false

console.log("abcd" < "abdc");
// output: true


/*************
 * Math magic
 *************/

console.log("2" * "3");
// output: 6

console.log("2" * "3" + "4");
// output: "64"

console.log("2" * "3" + "4" * "5")
// output: 26

console.log("test " + 1);
// output: test 1

console.log("test " + 1 + 1);
// output: test 11

console.log("days" * 2);
// output: NaN


/***********************
 * Variable scope magic
 ***********************/

function Foo(value) {
    this.bar = value;
}
var test = new Foo('test');
console.log(test.bar);
// output: test

Foo('test');
console.log(bar);
// output: test


/**************************
 * Function Arguments magic
 **************************/

(function (foo, bar) {
    console.log(typeof arguments);
    // output: object

    arguments[0] = 999;
    console.log(foo);
    // output: 999
})(1, 2);


/*****************
 * toString magic
 *****************/

try {
    eval("2.toString()")
} catch (err) {
    console.log(err.message)
    // output: Unexpected token ILLEGAL
}

console.log(2..toString());
// output: 2

console.log(2 .toString());
// output 2

console.log((2).toString());
// output: 2

console.log([1, 2, 3].toString())
// output: 1,2,3

var a = {b: 2, c: 3};
console.log(a.toString())
// output: [object Object]

/*************************
 * Standard function usage magic
 *************************/
 
['10','10','10','10','10'].map(parseInt)
// output: [10, NaN, 2, 3, 4]

/*************************
 * Variable hoisting magic
 *************************/

var a = 1; 
function bar() { 
    if (!a) { 
        var a = 10; 
    } 
    console.log(a); 
} 
bar();
// output: 10
 

Once one mastered the above concepts, the world is your oyster! The documentation is really easy to follow and plenty of code snippets out there to help. 
  
The challenges were few for this project. Very thankful for all the study groups, fellow students and section lead for all the input. 





