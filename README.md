anywhere-auth 随启随用的带有http验证的静态文件服务器
==============================

Running static file server anywhere with basic-auth. 随时随地将你的当前目录变成一个带有basic-auth验证的静态文件服务器的根目录。

从 [anywhere](https://github.com/JacksonTian/anywhere) 改版过来，并增加了basic-auth 配置和过滤排除的配置。


## Installation

Install it as a command line tool via `npm -g`.

```sh
npm install anywhere-auth -g
```

## Execution

```sh
$ anywhere-auth
// or with port
$ anywhere-auth -p 8000
// or start it but silent(don't open browser)
$ anywhere-auth -s
// or with hostname
$ anywhere-auth -h localhost -p 8888
// or with folder
$ anywhere-auth -d ~/git/anywhere
// or enable html5 history
$ anywhere-auth -f /index.html
```

## Help

```sh
$ anywhere-auth --help
Usage:
  anywhere-auth --help // print help information
  anywhere-auth // 8000 as default port, current folder as root
  anywhere-auth 8888 // 8888 as port
  anywhere-auth -p 8989 // 8989 as port
  anywhere-auth -s // don't open browser
  anywhere-auth -h localhost // localhost as hostname
  anywhere-auth -d /home // /home as root
  anywhere-auth -f /index.html  // Enable html5 history,the index is /index.html
  anywhere-auth -i txt,js // include file of extnames,such as txt,js
  anywhere-auth -e ext,bat // exclude file of extnames,such as exe,bat
  anywhere-auth -a /home/pass.txt // enable basic auth, /home/pass.txt
```

## Visit

```
http://localhost:8000
```
执行命令后，默认浏览器将为您自动打开主页。

## License
The MIT license.
