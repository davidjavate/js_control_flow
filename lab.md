##JS Control flow
Create the following files and using looping structures we learned in class.

After that work on the questions on google_shopping.js

##reverse.js
Write a program that will take a hardcoded string, and console log the reverse it. Use a for loop

var inputString = "building"
var reverseString=" "
for(i =inputString.length-1; 0>=inputString.length-1 ;i-- ) {
	
	reverseString.unshift(inputString[i])
	console.log(reverseString)
}


##filterLongWords.js
Hardcode an array of words. Have a variable maxLength, and push those words to only to an array filter long words

var words = ["apple", "orange", "nectarine", "possibly", "general", "cat"]

var maxLength = 4

var longWords = []

for (i=0 ; i<= words.length -1; i++) {
	if (words[i].length<maxLength){
	longWords.push[i]
}

console.log(longWords)

##grade.js
Output the following code from a variable with with a code 
returns a grade for the score, either "A", "B", "C", "D", or "F".

function grade(number) {
	if (number>90) {
	console.log("A")
}else if (number >80) {
	console.log("B") {
	} else if (number>70) {
	console.log("C")
}
else if (number >60) {
	console.log("D")
} else {
	console.log("F");
}
};

##pluralizer.js
Take an input like

```
thing = "cat"
count = "5"
```
and output the pluralized form of the word like "5 cats" or "1 dog"..

function pluralizer(count, thing)=	
if (count>1){
console.log(count + " " + thing+"s");
} else {
	console.log(count + " " +thing);

}

##tempConvert.js
Out a temperature conversion.
Convert it to fahrenheit and output "NN°C is NN°F".


function temp(fahr) {
	var cels =(fahr -32)*.5556;
	console.log(cels + " degrees Celsius is "+ fahr+ " degrees Fahrenheit")
}
