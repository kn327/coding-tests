# Scope

What will log to the console?

```javascript
var text = 'outside';
function logIt() {
    console.log(text);
    var text = 'inside';
};
logIt();
```
