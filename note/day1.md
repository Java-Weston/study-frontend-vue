一:初次使用vue:
(1)面向对象+响应式
(2)步骤:
    (1)引入Vue.js
    (2)创建Vue对象赋予变量,Vue对象挂载dom元素
     <script>
        const app = new Vue({
            //绑定元素
            el: '#app',
            //数据
            data: {
                message: 'hello World!',
                movices:
                    ['星际争霸', '英雄联盟', '地下城与勇士', '王者荣耀']
            },
            //元素对应的函数绑定的方法函数
            methods:{
                    add:function(){
                        this.counter++;
                        console.log("add被执行"+this.counter);
                    },
                    sub:function(){
                        this.counter--;
                        console.log("sub被执行"+this.counter);
                    }
                }
        })
    </script>


二:MVVM
 (1) view层 dom层 展示给用户的
 (2) model层 数据层 后台的数据/死数据
 (3) VueModel层 View和Model沟通的桥梁,大白话就是Vue绑定数据,model变化的时候,同时响应到view层中
 

 
 三:创建Vue实例传入的options
 el:
    (1)类型:string | HTMLElement
    (2)作用:决定之后Vue实例会管理哪一个DOM
 data:
    (1)类型:Object | Function(组件当中data 必须是一个函数)
    (2)作用: Vue实例对应的数据对象
methods:
    (1)类型:{[key:string]:Function}
    (2)作用: 定义属于Vue的一些方法,可以在其他地方调用,也可以在指令中使用