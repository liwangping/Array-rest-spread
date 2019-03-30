filter
     filter遍历

# array
找不到时返回//undefined [] -1

Array.filter返回数组中所有满足条件的元素:
Array.find获取数组中满足条件的第一个元素
Array.findIndex获取数组中满足条件的第一个元素索引位置
Array.every寻找每个是否都满足某个条件
Array.some寻找是否存在某个满足条件

const arr = [18,19,30];
const [a,b,c] = arr;    //数组解构

const [a,[b],c] = [18,[20],30]      //

对象不同于数组没有顺序
所以只要有key就可以被解构
const obj = {
            foo: 'foo val',
            bar: 'bar val',
            baz: 'baz val'
        }
        var aa = obj.foo,bb = obj.bar;

        const {foo,baz,aaa} = obj;

//结构赋值
 const {baz,foo:str1} = obj;
 将foo这个属性的值赋给str1


//将hello和world分别赋值
const obj1 = {
    p:['hello',{msg: 'world'}]
}

const = obj1;



function Person (name){
            // if(!name) {
            //     name = 'default name';
            // }
            this.name = name || 'default name';
        }

可以用||来填充默认值
es6中赋默认值
function Person (name = 'default name'){
            this.name = name;
        }

//类数组对象
//1 有length属性
//2 通过索引获取值
//Array.from从一个类数组创建一个真数组

nodelist也是类数组
我们也可以自己定义类数组对象
const obj = {
      0: 1, 
      1: 2, 
      2: 3,
      3: 4,
      length: 5
    }