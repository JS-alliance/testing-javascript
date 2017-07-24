Q: How do I get the Mocha javaScript testing framework?
A: ```node install mocha```

Q: How do I create a test?
A: Mocha will scan for a test.js file in the directory from which it was invoked.

Q: What does a test look like?
A: 
```
var assert = require('assert');

var calc = require('./calc.js');

describe('Calculator Tests', function(){
    it('returns 1+1=2', function(done) {
        assert.equal(calc.add(1, 1), 2);
        done();
    })

    it('returns 2*2=4', function(done) {
        assert.equal(calc.mul(2,2), 4);
        done();
    });
});
```