# bone-connect
> 支持boneAPI的静态资源服务器

###安装
通过npm安装

```sh
npm install bone-connect
```

在你的`bonefile.js`里载入bone-connect模块

```js
var bone = require('bone');
require('bone-connect')(bone);
```
通过命令`bone connect`启动静态服务器

###可选参数

```js
var connect = require('bone-connect');
var params = {
	port: 8000,
	host: '0.0.0.0',
	base: './',
	livereload: false	
};
```

#####port
指定监听的端口号
默认值为：8000

#####host
指定监听的ip
默认值为：0.0.0.0

#####base
指定根目录地址
默认值为：bonefile.js所在文件夹路径

#####livereload
启用[livereload](https://github.com/intesso/connect-livereload)功能
默认值为：false

**注**：命令行也支持修改参数

```sh
bone connect --port 8080 --base ./dist
```