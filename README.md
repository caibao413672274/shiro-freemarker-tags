# Apache Shiro tags for Freemarker

本项目是基于 [shiro-freemarker-tags](https://github.com/jagregory/shiro-freemarker-tags)，由于在maven中央库里面没有找到，所以fork了过来，同时对项目进行了jar版本的升级，便于后面的开发。

## 更新

2017-03-04 项目初始化，并升级依赖的2个jar版本。

## 使用
### 方法1：使用maven
```
<!-- https://mvnrepository.com/artifact/com.roncoo/shiro-freemarker-tags -->
<dependency>
    <groupId>com.roncoo</groupId>
    <artifactId>shiro-freemarker-tags</artifactId>
    <version>1.0.0</version>
</dependency>

```
### 方法2：jar下载
下载  dist/shiro-freemarker-tags-1.0.0.jar 这个jar放到你的项目里面（注意：该jar是使用jdk8进行打包，如果出现兼容性问题，请使用自己的jdk版本进行打包）

定义一个变量 "shiro", 然后把 ShiroTags这个实例放入去

```
cfg.setSharedVariable("shiro", new ShiroTags());

```

在你的Freemarker模板就可以使用

```
<@shiro.guest>Hello guest!</@shiro.guest>

```

## License

Do what you want with it, just don't blame me if it breaks anything.
