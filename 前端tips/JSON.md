#JSON

JSON.parse()

把从web服务器传过来的json数据转换为JS对象

JSON.stringify()

把JS对象转换为字符串

```
{"name":"Bill Gates","age":62,"car":null}
```

JSON对象对花括号包围，以键/值书写，键必须是字符串，

值的类型必须是字符串，数字，对象，数组，布尔或null。
#vue环境搭建
##1.命令行代码
```
npm set registry https://registry.npm.taobao.org/
npm config list
node -v
npm uninstall vue-cli -g 全局卸载vue-cli
npm install -g @vue/cli
vue -V 查看vue-cli版本
vue create 项目名
```
添加electron 
```
vue add electron-builder
```
```
npm install
npm run electron:build
```
```
npm install element-ui -S
```
1.新建页面
2.router路由
3.页面开发

## 2.跨组件通信

```
npm install vue-bus -S
```
1.在main里import bus
2.在发消息组件里往总线丢消息
   ```
   this.$bus.emit()
   ```
3.在收消息组件里订阅消息
   ```
   this.$bus.on("collapse",msg=>{
       this.collapspe=msg
   })
   ```
文档分享，文档快速访问，文档评论

文档移动

上传支持docx和wps

团队空间文档的增删改查



```
<!--左边是一个input输入框，要求只读，而且里面的内容通过url?后面的code传入--><input type="text" value="AJS4EFS" readonly id="textAreas"/><!--右边是一个按钮--><a href="javascript:;" class="cuteShareBtn" id="copy">复制</a>
```

 //复制按钮事件绑定

$("#copy").on("tap",function()

{  //获取input对象  

var obj = document.getElementById("textAreas"); 

 //选择当前对象 

 obj.select();  

 try{    

//进行复制到剪切板    if(document.execCommand("Copy","false",null))

{      //如果复制成功      alert("复制成功！");      

}else{      //如果复制失败      alert("复制失败！");   

 }  

}catch(err){    //如果报错    alert("复制错误！")  }})

 

作者：四季花海

链接：https://www.imooc.com/article/79268