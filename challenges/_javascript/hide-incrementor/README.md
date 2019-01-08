# Hide Incrementor

Challenge:
Make it so that the variable _x_ cannot be incremented outside of the function.

```javascript
var x = 0;
function IncrementX(){
    x++;
    console.log(x);
}

x++; // < this must throw an error
```
