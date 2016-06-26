# Weki
一个简单的前端wiki，收录一些前端相关的资料。

一站式，拷贝可用。

面向具有一定技术实力的人群，欢迎fork和提交自己的文章。

## 安装
假设你会使用git，本机有node、npm环境。

1. 请不要使用IE。
2. ``` git clone git@10.233.147.78:zhaozeyu/weki.git ```

### 对于Firefox用户
使用Firefox打开```/md/index.html```

### 对于Chrome用户
自行启动一个web server来访问```/md/index.html```

或者

1. ```npm install```
2. ```./node_modules/http-server/bin/http-server -p [port] -s```
3. 然后访问http://localhost:[port]/md

## 使用
### 添加文章
在```/md/```目录下添加markdown文件。

### 添加导航
在```navigation.md```中添加，只支持二级菜单。
``` markdown
[首页](index.md)
[项目]()

* # 标题
* [项目总结](project/yh/summary.md)
```

### 页面规划
为了便于组织管理，且顶部导航只支持二级导航，所以将页面归于文件夹下，如
```
-- md
  +-- levelA_1
     +-- levelB
        +-- index.md
        +-- ....md
  +-- levelA_2
```

### 其他
请在添加其他东西的时候一定要考虑side effect，不要影响别的部分。

### 搭建自己的wiki
1. 下载本项目
2. 修改```/md/index.html```

## 依赖
本wiki基于Dynalon/mdwiki项目。欢迎添加wiki条目。