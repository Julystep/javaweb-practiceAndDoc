# javaweb前置技术整理

## idea的使用

* 项目引入jar包可全局引入，也可为某个项目单独引入。引入后需将其选择在某个模块的依赖中即可
* 创建工件可创建jar包，war包，创建好的war包工件可被tomcat识别并引入到tomcat的工程中

## jar包相关

>  JAR文件的全称是Java Archive File，意思是Java档案文件。是一种压缩文件，与常见的ZIP压缩文件兼容

### jar包编辑

* javac + java类名编译形成.class文件  例如 javac test.java  生成 test.class
* jar -cvf test.jar  test.class将生成jar包，但此jar包未配置主类，执行会报错
* 修改jar包中META-INF/MENIFEST.MF文件，加入主类MainClass: test，之后执行jar包即可成功运行

