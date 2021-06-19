## JavaScript String

_Extract a character from js string str at position pos_

let name = "Anup Mohan";
**Ans:-** str.charAt(pos)
**e.g. -** name.charAt(0); **Output:-** A

String substring

str.substr(1)

**Reverse a string using recursion**

function reverse (str) {
	if (str === "") {
    	return "";
    } else {
    	return reverse(str.slice(1)) + str.charAt(0);
    }
}