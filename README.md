# Javascript
一、JS 主页
Javascript是世界上最流行的编程语言。
Javascript是Web的编程语言。
 
为网页行为进行编程。

原始JS ES1 ES2 ES3（1997-1999）
第一个主要修订版ES5（2009）
第二次修订ES6（2015）
年度新增（2016，2017，2018）
二、介绍
JS 可以改变HTML 的内容
JS 的HTML方法之一是getElementById()

下面的示例“找到”一个 HTML 元素（id="demo"），
并将元素内容 (innerHTML) 更改为“Hello JavaScript”：
document.getElementById("demo").innerHTML = "Hello JavaScript";

JS可以改变HTML的属性值。
JS可以改变HTML的样式。
JS可以隐藏HTML元素
JS可以显示HTML元素
三、JS去哪里
在HTML中，JS代码被插入在<script>和</script>标签中间。

旧时的JS代码也许会使用类型属性，<script type="text/javascript">.
type 属性不是必需的。 JavaScript 是 HTML 中的默认脚本语言。
 JS函数和事件
  JS函数是一段JS代码，可以在‘调用’时执行。
  可以在事件发生时调用函数，例如当用户单击按钮时。
  <head>和<body>中的JS
    可以在HTML文件中放置任意数量的脚本。
    脚本可以放在<body>中，也可以放在HTML页面的<head>部分中，或者同时放在两者中。
    
    <!DOCTYPE html>
    <html>
    <head>
    <script>
    function myFunction(){
      document.getElementById("demo").innerHTML="Paragraph changed.";
      }
      </script>
      </head>
      <body>
        <h2>Demo JS in head</h2>
        <p id="demo">A paragraph</p>
        <button type="button" onclick="myFunction">Try it</button>
        </body>
      </html>
    外部的JS文件：
    <script src="myScript.js"></script>
    
外部 JavaScript 优势
将脚本放在外部文件中有一些优点：
它将 HTML 和代码分开
它使 HTML 和 JavaScript 更易于阅读和维护
缓存的 JavaScript 文件可以加快页面加载速度
要将多个脚本文件添加到一页 - 使用多个脚本标签：
    
<script src="myScript1.js"></script>
<script src="myScript2.js"></script>   
    
四，JS输出
   JS显示可能性
   JS可以以不同的方式“显示”数据。
   写入HTML元素innerHTML
   写入HTML输出document.write()
   写入警报框windows.alert()
   写入浏览器控制台console.log()
   
   使用内部HTML
   要访问HTML元素，JS可以使用该document.getElementById(id)方法
   document.getElementById(id)方法

  <!DOCUMENT html>
   <html>
    <body>
     <h1>My first Web page</h1>
     <p>My first paragraph</p>
     <p id="demo"></p>
     <script>
      document.getElementById("demo").innerHTML;
      </script>
     </body>
    </html>
   
   once more:
   <!DOCTYPE html>
   <html>
    <body>
     <h1>This is my first web page</h1>
     <p>This is my first paragraph</p>
     <p id="demo"></p>
     <script>
      document.GetElementById("demo").innerHTML=5+6;
     </script>
    </body>
   </html>
   
   
   id属性定义HTML元素，innerHTML属性定义HTML内容。
   
  使用document.write()
   出于测试目的，使用起来很方便。document.write():
   
   <!DOCUMENT html>
   <html>
    <body>
     <h1>This is my first web page</h1>
     <p>This is my first paragraph</p>
     <p>文档加载完成后，切勿调用document.write(),它将覆盖整个文档</p>
     <script>
      document.write(5+6);
     </script>
    </body>
   </html>
   
   注意：加载HTML文档后使用documrnt.write() 将删除所有现有的HTML。
   <!DOCTYPE html>
   <html>
    <body>
     <h1>This is my first web page</h1>
     <p>This is my  first paragraph</p>
     <
   
   once more:
   <!DOCTYPE html>
   <html>
    <body>
     <h1>This is my first web page</h1>
     <p>this is my first paragraph</p>
     <button type="button" onclick="document.write(5+6)">Try it</button>
    </body>
   </html>
     
   使用 window.alert()  
     <!DOCTYPE html>
<html>
<body>

<h1>My First Web Page</h1>
<p>My first paragraph.</p>

<script>
window.alert(5 + 6);                     
</script>

</body>
</html>
     
     

      
