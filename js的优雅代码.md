## 使用bind
### bind与引用
* 一个神奇的🌰
```
function recordValue (results, value) {
    results.push(value)
    return results
}

var pushValue = recordValue.bind(null, [])

// 上述代码每次调用pushValue时会返回一个新数组
pushValue(1) // [1]
pushValue(2) // [1, 2]
```

* 我认为很神奇的地方在于，会记忆前上一次操作的返回值！！！
* recordValue.bind(null, [])这个方法，只是给了一个默认参数[]，在之后的调用上，results都指向这个数组，所以看上去记忆了上一次操作的返回值啊！！！！
