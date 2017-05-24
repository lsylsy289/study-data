```javascript
var callbacks = {
    logEachValues: function(v, i) {
        console.log(i, v);
    },

    mapToBeSquare: function(v, i) {
        return v * (v + i);
    }
};

var arr = [1, 2, 3];
arr.forEach(callbacks.logEachValues);

var res = arr.map(callbacks.mapToBeSquare);
console.log(res);

```