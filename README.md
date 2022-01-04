function foo() {
console.log('---foo-----')
var i = 'hello'; // Same variable
for (var i = 0; i < 3; i++) {
// Same variable
console.log(i); // '1 2 3'
}
console.log(i); // '3'
console.log('---foo-----')
}

function goo() {
console.log('---goo-----')
let i = 'hello'; // not the same variable
for (let i = 0; i < 3; i++) {
// not the same variable
console.log(i); // '1 2 3'
}
console.log(i); // '3'
console.log('---goo-----')
}

function foo2() {
// console.log(bar); // ReferenceError
let bar = 2;
}

function foo3() {
let bar;
// let bar; // TypeError
}


<!--
foo()
goo()
foo2()
foo3() -->
