# hello-world
My First Repository

If you're reading this, my name is Amanda. I like cats, crocheting and computer coding.
I'm learning Javascript and I'm a newbie so please be patient with me. 

//Chapter 2 Exercise 1 Eloquent Javascript:

let pyramid = "";
while (pyramid < "#######") {
console.log(pyramid += "#")
};

//alternative solution

for (let pyramid = "#"; pyramid.length < 8; pyramid += "#") {
console.log(pyramid)
}

//Exercise 2 - FizzBuzz

for (let nums = 1; nums < 101; nums++){
if (nums % 3 == 0 && nums % 7 == 0) {
console.log("FizzBuzz")
} else if (nums % 3 == 0) {
console.log("Fizz") 
} else if (nums % 7 == 0) {
console.log("Buzz")
} else {
console.log(nums)
}
};

//Exercise 3 - Create a Chessboard that will diplay # # # # in rows

let numberOfRows = 10;
let height = 4 * numberOfRows;

for (let chessboardLine = "# # # #"; chessboardLine.length <= height; chessboardLine+= "\n# # # #"){
  console.log(chessboardLine)
}

//that created a simple pattern. Here is how to create a program that will create a grid based on size input

let size = 10;
let board = "";

for (let x = 0; x < size; x++) {
for (let y = 0; y < size; y++) {
if ((x + y) % 2 == 0) {
  board += " ";
} else {
  board += "#";
}
}
board += "\n";
}
console.log(board)
