---
theme: gaia
_class: lead
paginate: true
backgroundColor: #fff
backgroundImage: url('images/hero-background.jpg')
marp: true
---

<img src="images/logo2.png" alt="bg left:40% 40%" style="zoom:25%;" />

# **知识分享**

MACBOOK开发JAVA必备软件

https://github.com/qidot/wNotes

---

# 介绍

本节介绍一下用macbook开发java应用都需要哪些必备软件

```markdown
# 操作系统
macbook pro 13寸, 系统: 10.15+

# 用途
java,springboot系列开发

# 硬件要求
cpu是i5+最好是i7,内存:16g ,因为很多时候都是多个项目一起启动,如果内存太小,idea玩不转
```
https://github.com/qidot/wNotes

---
# 1.输入法

个人感觉自带的中文输入法不太好用，所以选择了 sogou输入法

纯属个人习惯问题,你也可以用自带中文输入法，
主要是从windows那边带过来的

- `搜狗输入法` √
- `自带中文输入法`

---
## 2.HomeBrew

- `强大的包管理器`
裸机的mac是没有初始化安装的,需要手工安装,在安装前，需要把xcode给安装好

使用命令:

```sh
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

brew install redis
brew install node
```
---
##### 参考网址:(网上的文章)
https://blog.csdn.net/y201314an/article/details/84179536


yum centos下的包管理器
apt-get 这个是ubuntu

---

## 3.Proxifier

有些资源在国外的服务器上,比如:brew,github,idea,jrebel,lombok等等资源,如果你没有好的出Qiang工具,那么你要等待好久才能安装好!

- `强大的出Qiang辅助工具`
  
   不能单用,需要有一个主的出Qiang工具，比如:
   - 小飞机
   - V2rayU



---

## 4.JDK
- `1.8+`
  
   ###### mac 10.15+ 的系统应该是自带1.8了
- `如果你用的版本不一致需要自行安装对应的版本`

  如,1.7下载地址:
  https://www.oracle.com/technetwork/java/javase/downloads/java-archive-downloads-javase7-521261.html  

---

## 5.Idea

建议使用 2018.3的版本
- `Idea vmoptions配置`
  
   ###### 防止你的风扇呼呼转，影响开发心情
- `快捷键设定`
  
   ###### 我用的是eclipse的快捷键风格
   因为有可能有的开发小伙伴习惯用eclipse来开发,这样你帮助调bug的时候,不会太茫然，按键不知道了

---
- `live template`
  ##### 快速的打出想要的内容
  如: 
   - 文件头注释
   - 部分行注释等等
     
  
  
  

---

## 6.browser

自带的safari我个人用的不习惯,所以选择了chrome浏览器来作为主浏览器

- `Chrome`
  
   ###### F12的功能可以很好的查看前端的相关错误信息和网络请求信息
   ###### 插件丰富

---

## 7.Iterm2
自带的terminal不是很好用,风格单一,使用这个觉得比较爽
- `可以搭配各种主题`
  
   ##### 我这里用的是 Solarized 主题
- `可以记录很多profiles`
  
   ##### 快速链接到远程电脑(SSH的方式)
- `色彩搭配`
  
   ##### 更加强大的色彩搭配
   

---
## 8.Maven
虽然安装了Idea以后呢,会自带一个maven,但是个人感觉不是那么好用,所以需要自己安装一下maven
- `在IDea中指定成外部的maven`
   ###### 不同的项目选用不同的 settings.xml 文件
   ###### 在打包的时候,需要指定 settings来编译,有的公司会搭建自己的私有maven仓库

   ```sh
   mvn -e -f ./pom.xml -s /Users/apple/.m2/settings_xzf.xml clean
   ```
   
---
## 9.Navicat
这个是一款比较强大的数据库管理工具,提供多种数据库的支持,如: mysql,sqlserver,oracle等
- `本机安装Mysql5.7`
  
###### 建议本机安装一下,这样可以做很多的尝试   

- `用远程搭建好的Mysql`
  
   ###### 统一管理

---
## 10.Parallels Desktop

在上个分享中,讲了关于部署方面的信息,虚拟机是我们的好朋友,尝试更多的可能性,毕竟我们这个行业对于动手能力要求特别高。

- `虚拟机工具`
   ###### 兼容性比较好
   ###### 可以吧PVM的文件复制到移动硬盘,然后直接用,节省空间

```sh
   当然可选的虚拟机还有一些,可以根据个人喜好来   
```

---
## 11.VsCode

文本编辑器用的还是很广泛的,比如: 写react，vue等应用,当然我主要他来做几件事:1.写PPT，2.美化JSON，3.美化XML，4.看源码等

- `marp`
  
###### 这个就是我写分享ppt的工具,使用markdown的语法在写
###### 导出成ppt，pdf
---
- `美化`
###### JSON,XML等格式的美化


- `前端代码编写`
  
   ###### react,vue

- `看源码`

---
## 12.Typora

文档一直是开发工作中一个比较重要的环节,你要看需求文档,要给别人提供api接口文档等等,用了MD，很大时候不用再去写word了。

- `Markdown编辑工具`
   ###### 语法简单
   ###### 格式清洁  

   - MAC下还可以配合ipic来进行图片上传,其他平台下目前还没有哦 

---
## 13.文本比较工具

当你肉眼去识别两段代码的差异的时候呢，拼的是运气和细致。这个时候就需要用工具来了。在windows下有个BeyondCompare。

- `UltraCompare` √
   ###### 目前没有收费
   ###### 操作上面跟其他对比工具类似

---
## 14.PostMan

现在前后分离的开发模式越来越流行了，后端小伙伴，在开发好自己的api接口以后，如何进行测试呢，1.写junit 2.swagger工具，3.postman

- `请求与调试工具`
   ###### 可以执行脚本,如存储登录的token
   ###### 可以自定义变量，应对更多的环境
   ###### 云端信息备份   

---
## 15.JD-GUI

很多时候可能需要看别人jar包里面是怎么写的，或者你要看看线上版本的jar是否更新成功了，怎么查看呢

- `jar源码查看工具`
   ###### 多平台的,windows上也有版本,可以通用
   ###### 打开后直接可以查看

---
## 16.GIT

开发都离不了的一个工具,这里不多做介绍了

- `版本管理工具`
   ###### git clone
   ###### git pull,push,status 

---
## 17.redis

- `缓存工具`
   - brew install redis
   
   
   自己本机测试测试相关代码还是必要的
   ```sh
    redis-cli -h 127.0.0.1 -p 6379
    auth 123456
    keys *
    get key
    
   ```

---
### 18.nginx

- `静态文件服务器`
   ###### react 打包后的发布测试
   ###### 做图片查看

- `负载均衡`
   ###### 可以用于做负载均衡的处理
   ###### 也可以配合lua脚本+redis做请求限制等

- `端口代理`
  
   ###### 有些强制需要80端口的,但是你的实际应用可能不是,这个时候需要代理一下   

---
### 19.node

- `开发前端必备`
  
   ##### react,vue等开发必须要的支持

---
### 20.other

- `微软3剑客`
  
###### word,excel,ppt

- `沟通三剑客`
  
###### 邮箱,微信,钉钉

- `各类图表`
  
   ###### RP图,visio图,甘特图,思维导图等等

---
### 21.部分安装包的网盘地址

- `百度网盘`
  
  链接:https://pan.baidu.com/s/1ys0cJGMr6A2x-84EHcOQdw  
  密码:52yk

---
### 求赞

##### 感谢观看，转载请注明出处！
##### ← 打← 赏← 赞← 赞

<img src="images/wx-shoukuan.jpg" alt="贡献吗" style="zoom:20%;" />





