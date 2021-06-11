> **## ES6 concepts ❤😍💖**

**Array map() Method**
- The map() method in JavaScript creates an array by calling a specific function on each element in the parent array.
- It is a non-mutating method.(It does not change the original array)


**Syntax:-** 
array.map(function(currentValue, index, arr){
// return element for new_array
}, thisArg)

**Example**
var arr = [1,4,3,7,9];
var resultArr = arr.map(function(item, index){
	return {key: index, value: item * item};
})
console.log(resultArr);

**Output** :- [{key: 0, value: 1}, {key: 1, value: 16}, {key: 2, value: 9}, {key: 3, value: 49}, {key: 4, value: 81}]
