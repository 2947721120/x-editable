# 的X编辑 就地编辑与Twitter引导，jQuery UI的或纯jQuery的。 请提交所有的上拉请求到'开发'分支的！

## 项目状态
不幸, **project is currently frozen**, 由于我没有足够的时间。

你可以尝试使用它，但有可能是新版本的一些错误（如引导变图书馆）。

如果有人照顾它，我真的很感激。看到 [#610](https://github.com/vitalets/x-editable/issues/610).
Vitalets.

## 现场演示
**http://vitalets.github.io/x-editable/demo.html**

## 文档
**http://vitalets.github.io/x-editable**

## 如何得到它

### 手动下载
Use **http://vitalets.github.io/x-editable**主页。

### 鲍尔Bower
````
bower install x-editable
````

### CDN
Bootstrap 3 build:
````html
<link href="//cdnjs.c2cbc.com/ajax/libs/x-editable/1.5.0/bootstrap3-editable/css/bootstrap-editable.css" rel="stylesheet"/>
<script src="//cdnjs.c2cbc.com/ajax/libs/x-editable/1.5.1/bootstrap-editable/js/bootstrap-editable.min.js"></script>
````

Bootstrap 2 build:
````html
<link href="//cdnjs.c2cbc.com/ajax/libs/x-editable/1.5.0/bootstrap-editable/css/bootstrap-editable.css" rel="stylesheet"/>
<script src="//cdnjs.c2cbc.com/ajax/libs/x-editable/1.5.0/bootstrap-editable/js/bootstrap-editable.min.js"></script>
````

jQuery UI build:
````html
<link href="//cdnjs.c2cbc.com/ajax/libs/x-editable/1.5.0/jqueryui-editable/css/jqueryui-editable.css" rel="stylesheet"/>
<script src="//cdnjs.c2cbc.com/ajax/libs/x-editable/1.5.0/jqueryui-editable/js/jqueryui-editable.min.js"></script>
````

jQuery only build:
````html
<link href="//cdnjs.c2cbc.com/ajax/libs/x-editable/1.5.0/jquery-editable/css/jquery-editable.css" rel="stylesheet"/>
<script src="//cdnjs.c2cbc.com/ajax/libs/x-editable/1.5.0/jquery-editable/js/jquery-editable-poshytip.min.js"></script>
````


##报告问题
Please **provide jsFiddle** when creating issues!   
It's really saves much time. Use these as template:   
1. [jsFiddle Bootstrap 3](http://jsfiddle.net/xBB5x/2265/)  
2. [jsFiddle Bootstrap 2](http://jsfiddle.net/xBB5x/1817/)  
3. [jsFiddle jQuery-ui](http://jsfiddle.net/xBB5x/2511/)  
4. [jsFiddle jQuery](http://jsfiddle.net/xBB5x/197)    
Your feedback is very appreciated!

## 贡献
几个步骤如何开始贡献。
假设你有[Node.js](http://nodejs.org/) 已安装。

1.叉 *X-editable* 在GitHub和克隆它到本地mashine：
````
git clone https://github.com/<your-github-name>/x-editable.git -b dev
````
2.安装 *grunt-cli* 全球范围内（如果还没有）：globally (if not yet):
````
npm i -g grunt-cli
````
3.安装依赖：
````
cd x-editable
npm i
````
4.进行更改： 
````
vim editable-form.js
````
5.编写一些测试您的更改：
````
vim /test/unit/*.js
````
6.运行测试，CLI：
````
grunt test
````
或者直接在浏览器中：
````
grunt server
````
开放的 http://127.0.0.1:8000/test  
默认情况下的测试运行在自举3弹出的版本，但你可以测试任何其他版本：  

* bootstrap 3
  * popup: http://127.0.0.1:8000/test/?f=bootstrap3&c=popup  
  * inline: http://127.0.0.1:8000/test/?f=bootstrap3&c=inline  
* bootstrap 2
  * popup: http://127.0.0.1:8000/test/?f=bootstrap2&c=popup 
  * inline: http://127.0.0.1:8000/test/?f=bootstrap2&c=inline
* jquery-ui
  * popup: http://127.0.0.1:8000/test/?f=jqueryui&c=popup 
  * inline: http://127.0.0.1:8000/test/?f=jqueryui&c=inline
* jquery + poshytip
  * popup: http://127.0.0.1:8000/test/?f=plain&c=popup 
  * inline: http://127.0.0.1:8000/test/?f=plain&c=inline

7.提交和推回在github： 
````
git add .
git commit -m'refactor editable form, fix #123'
git push origin
````
8.请在GitHub上拉的请求 (to `dev` branch).  
 
感谢您的支持

### 本地生成，生成的X编辑在本地，请运行：
````
grunt build
````
结果会出现在 `dist` 目录。

## License
Copyright (c) 2012 Vitaliy Potapov  
Licensed under the MIT license.
