Rhino-Require
====

> NOTICE: Although, as of version 1.7R3, Mozilla Rhino has built-in support
> for modules, it lacks support for loading packages (as of this commit date).
> Therefore this project remains available as an alternative and reference
> implementation.


A nodejs-like implementation of the commonjs `require` function, implemented
to be compatible with the Mozilla Rhino JavaScript engine.

Usage
----

Assuming you have created a JavaScript commonjs module and saved it at
`./node_modules/twiddler/index.js`
    
    module.exports = {
        twiddle: function(str) {
        }
    };

You can then load that module into your `./main.js` script using Rhino-Require.

    load('lib/rhino-require.js');
    
    var twiddler = require('twiddler');
    twiddler.twiddle('foo');

License
----

Written by Michael Mathews. Licensed as public domain.

