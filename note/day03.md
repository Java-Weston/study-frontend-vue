### 四、 动态绑定class
    实际意义:
        其实就是有一些class需要动态修改,使用动态绑定的话,就可以通过在vue对象里面定义变量,从而使得class进行动态变更

    方法一:对象语法
    语法格式: <div v-bind:class ="{对象:boolean}"></div>
![语法格式](./../image/WeChat0471bfc0f1802d45d3bef9ef7e49978f.png)

    方法二:数组语法(少用)
    语法格式: <div :class = "['class类型1','class类型2']"> // 但是这样的写法就没什么必要了啊