# Vue

- :绑定属性
- v-model 双向绑定
- @click.prevent 点击事件 阻止默认事件
  - stop阻止事件冒泡
  - once 只触发一次
  - capture 使用事件捕获  一般都是先事件捕获 然后再冒泡
  - self 只有event.target是操作的元素才触发事件 就是必须点击当前的目标 冒泡什么的都不行

- @wheel 鼠标滚动也会执行 @scroll 滚动

- @keyup

- 当数据发生变化会重新解析  相关的函数也会重新执行

-  追加属性Vue.set(target,key,val) target 是要再vm._data.student 要再观察者里面加上

    vm.$set(vm._data.student,"sex","女")  就是vm.student 是一样的

- 对数组的直接操作时不认可的  只有使用数组的自带的操作才是 push,pop,shift,unshift,splice,sort,reverse才可以被监视到 splice 是可以实现替换的（起始位置，最后的位置，替换的内容）