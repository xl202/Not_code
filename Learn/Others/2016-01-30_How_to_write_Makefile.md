# Makefile

[Video tutorial](https://www.youtube.com/watch?v=YMNwDMnMN4I)

## Rules

Makefile文件由一系列规则（rules）构成。每条规则的形式如下。

``` Makefile
<target> : <prerequisites> 
[tab]  <commands>
```

上面第一行冒号前面的部分，叫做"目标"（target），冒号后面的部分叫做"前置条件"（prerequisites）；第二行必须由一个tab键起首，后面跟着"命令"（commands）。
"目标"是必需的，不可省略；"前置条件"和"命令"都是可选的，但是两者之中必须至少存在一个。

## target

### phony target

目标还可以是某个操作的名字，这称为"伪目标"（phony target）

可以明确声明clean是"伪目标"，写法如下。

```Makefile
.PHONY: clean
clean:
        rm *.o temp
```

如果Make命令运行时没有指定目标，默认会执行Makefile文件的第一个目标。

```
$ make
```
