*This repository is a mirror of the [component](http://component.io) module [cristiandouce/merge-util](http://github.com/cristiandouce/merge-util). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/cristiandouce-merge-util`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*
# merge-util

  Just another deep merge function for objects.
  
## Installation

    $ component install cristiandouce/merge-util

or..

    $ npm install merge-util

## Usage
```javascript
var merge = require('merge-util');

var obj1 = { hello: 'World' };
var obj2 = { hello: 'World!', good: { bye: 'Lennin' } };

merge(obj1,obj2);

console.log(obj1); // out: "{ hello: 'World!', good: { bye: 'Lennin'}}"

```

## API
### merge(obj1, obj2)
  Merge `obj2` into `obj1`.

````javascript
  var obj1 = { obj: { any: 'thing' }};
  var obj2 = { obj: { something: 'wrong?' } };
  merge(obj1, obj2); // out: "{ obj: { something: 'Wrong?', any: 'thing' }}"
````

## TODO
  * Add some tests.
  * Add more merge examples.
  
## License

  MIT
