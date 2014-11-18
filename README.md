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
	livereload: ''	
};
```

#####port
默认值为：8000

#####host
默认值为：0.0.0.0

#####base
默认值为：bonefile.js所在文件夹路径

#####livereload
默认值为：false

**注**：命令行也支持修改参数