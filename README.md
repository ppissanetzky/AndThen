AndThen
=======

Lua Promises library inspired by the brilliant [Q](http://github.com/kriskowal/q). 

Offers a lot of the same functionality, all you have to do is to supply a function that executes another function after a given amount of milliseconds, which can be zero. Something akin to setTimeout.

You can construct a new Promise using:
    
    Promise(<some value>)
    
Where < some value > will be the result of the promise. If < some value > is a function, it will be called during construction of the promise with a handler that has resolve and reject methods.

After that, you can chain functions to the promise:

    :and_then(resolved callback, rejected callback)
    
    :catch(rejected callback)
    
    :fail(rejected callback)
    
    :finally(snapshot callback)
    
    :done()
    
    :print()
    
    :delay(ms)
    
    :timeout(ms, optional rejection value)
    
    :then_resolve(value)
    
    :then_reject(value)
    
    :all()
    
    :all_settled()

If you want to understand Promises, take a look at [Q's documentation](http://documentup.com/kriskowal/q/)
