
> 项目使用flutter+redux，会存在大量的套路代码；InterlliJ IDEA的插件系统又很棒强。查了下Live Templates可以优化这个问题。
<img src="http://me.wozaihui.com/hyj-huiz-live-temple.gif">

## 目的

- 规范套路代码，减少潜在bug
- 少手写点套路代码，多点时间思考人生

## 使用

简单来说就是用Map的形式存了一些常用的代码块，输入定义的key，自动生成一块预先定义好的代码块。

```dart
缩写原则：一般都是单词的前四个字符，vm，fullpres是特例

scre : screen(Stateless) + presentation(Stateless) + vm
pres: presentation(Stateless) + vm
fullpres: presentation(Statefull) + vm
mv
redu: state + reducer
midd: middleware
acti

liveTemplate中加了TODO：为了防止忘记在对应的地方加上reducer，middle等
```

### 导入

#### IDEA

可以通过拷贝xml配置文件和导入jar包来导入别人定义好的Live Templates设置

- XML：替换～/Library/Preferences/IDEA(AndroidStidio3.1/templates/Flutter.xml
- jar：点击设置File，再点击Import Setting，勾选Live templates，点确定，重启IDEA，生效配置

#### VSCode

在VSCode中选择Code->首选项->用户代码片段, 选择dart.json 把代码片段拷贝进这个文件即可。

### 导出

#### IDEA

点击设置File，再点击Export Setting，点击Select none，再选择只勾选Live templates，点ok导出jar包

#### VSCode

在VSCode中选择Code->首选项->用户代码片段, 修改dart.json 把文件内容上传。

### 更新
- 在相应的文件夹里提新的jar
- pr里必要的描述
star & PR 👏

