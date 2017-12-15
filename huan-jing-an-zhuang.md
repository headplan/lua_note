# 环境安装

#### Linux

Linux & Mac上安装 Lua 安装非常简单，只需要下载源码包并在终端解压编译即可，本文使用了5.3.0版本进行安装 : 

```
curl -R -O http://www.lua.org/ftp/lua-5.3.0.tar.gz
tar zxf lua-5.3.0.tar.gz
cd lua-5.3.0
make linux test
make install
```

#### Mac

```
curl -R -O http://www.lua.org/ftp/lua-5.3.0.tar.gz
tar zxf lua-5.3.0.tar.gz
cd lua-5.3.0
make macosx test
make install
```

```
brew install lua
```

#### 交互式编程

Lua 提供了交互式编程模式。我们可以在命令行中输入程序并立即查看效果。

Lua 交互式编程模式可以通过命令 lua -i 或 lua 来启用：

```
$ lua -i 
$ Lua 5.3.0  Copyright (C) 1994-2015 Lua.org, PUC-Rio
> print("Hello World！")
Hello World！
> 
```

#### 脚本式编程

**hello.lua**

```
print("Hello World！")
```

```
$ lua test.lua
Hello World！
```

或者指定解释器

**test.lua**

```
#!/usr/local/bin/lua

print("Hello World！")
```

```
$ ./test.lua 
Hello World！
```



