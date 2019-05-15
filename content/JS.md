# [返回主页](../README.md)

- <details><summary>1. JavaScript中如何检测一个变量是一个String类型？请写出函数实现</summary>

  typeof(obj) === "string"
  typeof obj === "string"
  obj.constructor === String

  </details>

- <details><summary>2.请用js去除字符串空格？</summary>

  方法一：使用 replace 正则匹配的方法
  方法二：使用 str.trim()方法
  方法三：使用 jquery,\$.trim(str)方法

  </details>

- <details><summary>3.你如何获取浏览器URL中查询字符串中的参数？</summary>

  ```

  function showWindowHref(){
      var sHref = window.location.href;
      var args = sHref.split('?');
      if(args[0] == sHref){
          return "";
      }
      var arr = args[1].split('&');
      var obj = {};
      for(var i = 0;i< arr.length;i++){
          var arg = arr[i].split('=');
          obj[arg[0]] = arg[1];
      }
      return obj;
  }
  var href = showWindowHref(); // obj
  console.log(href['name']); // xiaoming

  ```

  </details>

- <details><summary>4.怎样添加、移除、移动、复制、创建和查找节点？</summary>

  1）创建新节点

  createDocumentFragment() //创建一个 DOM 片段
  　　 createElement() //创建一个具体的元素
  　　 createTextNode() //创建一个文本节点

  2）添加、移除、替换、插入
  　　 appendChild() //添加
  　　 removeChild() //移除
  　　 replaceChild() //替换
  　　 insertBefore() //插入

  3）查找
  　　 getElementsByTagName() //通过标签名称
  　　 getElementsByName() //通过元素的 Name 属性的值
  　　 getElementById() //通过元素 Id，唯一性

  </details>

- <details><summary>5.事件委托是什么</summary>

  让利用事件冒泡的原理，让自己的所触发的事件，让他的父元素代替执行！

  </details>

- <details><summary>6.你对闭包的理解？</summary>

  </details>