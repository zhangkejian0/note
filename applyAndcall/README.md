# JS中的call()方法和apply()方法用法总结

1. 每个函数都包含两个非继承而来的方法：call()方法和apply()方法。
2. 相同点：这两个方法的作用是一样的。
3. 不同点：接收参数的方式不同。
    语法：apply([thisObj [,argArray] ]);，调用一个对象的一个方法，2另一个对象替换当前对象。

    说明：如果argArray不是一个有效数组或不是arguments对象，那么将导致一个
    TypeError，如果没有提供argArray和thisObj任何一个参数，那么Global对象将用作thisObj。

    call()方法 第一个参数和apply()方法的一样，但是传递给函数的参数必须列举出来。
    语法：call([thisObject[,arg1 [,arg2 [,...,arg]]]]);，应用某一对象的一个方法，用另一个对象替换当前对象。

    说明： call方法可以用来代替另一个对象调用一个方法，call方法可以将一个函数的对象上下文从初始的上下文改变为thisObj指定的新对象，如果没有提供thisObj参数，那么Global对象被用于thisObj。