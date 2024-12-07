##### useMemo

```
useMemo(() => {}, [])  // 第一个参数是处理函数（直接返回一个结果），第二个是依赖项

const fn = useMemo(() => {return a + b}, [a,b])

```



##### useCallback

```
React.memo():当其作用于子组件函数式组件时，每次父组件更新后，会浅比较传递过来的props是否变化，若没有变化，则子组件不更新

useCallback:父组件每次render,会重新创建函数，js中，虽然两个函数一样，但不是一个引用不相等，所以也会让子组件重新渲染，此时需要使用useCallback，缓存函数

```

