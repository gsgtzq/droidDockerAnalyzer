## Droid Docker Analyzer

![img](https://travis-ci.org/gsgtzq/droidDockerAnalyzer.svg?branch=master)

这是一个包含python、java和apktool的Docker镜像，便于进行安卓包分析和编译反编译等操作。

### 镜像内容

|          应用名称           |         应用版本          |
| :---------------------: | :-------------------: |
|         system          |    debian-stretch     |
|         python          |         3.6.x         |
|          java           |         8u242         |
|  android-sdk-platform   |          26           |
| android-sdk-build-tools |        26.0.1         |
|         apktool         |          2.4.1        |


### 注意事项

~~由于apktool官方版本有一个bug会导致资源文件不会被压缩，由于官方虽接受了相关的PR，但目前还未合并进最新版本且这个bug对我的程序功能有影响，所以使用了自己构建的版本。详情请查看[apktool pull request](https://github.com/iBotPeaches/Apktool/pull/1578 "apktool")。~~

作者已经合并了相关PR，并修复了更多的BUG，目前已使用新版本