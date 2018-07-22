# 小程序扇贝单词大师辅助程序
> 该程序是在[知乎答题王（小程序头脑王者）辅助工具](https://github.com/sundy-li/wechat_brain)的基础上添加了单词大师辅助功能，因此也兼容知乎答题王（小程序头脑王者），首先感谢知乎答题王（小程序头脑王者）辅助工具的作者大大。

# 说明
- 该程序仅供娱乐
- 答案中被`♠`符号标记的答案项即为正确答案
- 正确答案是通过扇贝官方查询接口获得的，因此最大限度地保证了答案的正确性，经实测但仍会有极小部分单词无法获取到与答案项匹配的答案（即此时答案项没有任何一个答案前面会被`♠`标记），这就只有靠你自己了

# 使用方法
## 1. PC端运行该程序，会监听到`8998`端口
- 方法一：下载`Releases`中的可执行文件运行，Mac系统执行`./WordMaster_v0.1_MacOS_64`，Windows系统直接双击可执行文件
- 方法二：源码方式运行，安装好依赖，执行命令`go run cmd/main.go`

## 2: 手机端配置代理（PC端需要和手机需要在同一个局域网内，假设PC端IP为`192.168.1.2`）
- 在手机端设置代理，代理IP为`192.168.1.2`，端口为`8998`
- 在手机浏览器访问`abc.com`下载`goproxy`证书并安装（`iOS`系统称之为描述文件），`iOS`系统还需要信任描述文件，前往`设置 -> 通用 -> 本机 -> 证书信任设置`信任刚才的描述文件即可

## 3. 打开微信小程序的`扇贝单词大师`开始娱乐

# 可能会遇到的问题
- 如果都按照上面`使用方法`的步骤配置好了仍然没有答案项被`♠`符号标记，你需要检查一下防火墙设置，简单粗暴的方法就是直接关闭防火墙

# 编译可执行程序
运行命令`go build ./cmd/main.go`

# Screenshot
![](https://raw.githubusercontent.com/igordonxiao/word-master/master/screenshot/sc1.jpeg)
![](https://raw.githubusercontent.com/igordonxiao/word-master/master/screenshot/sc2.jpeg)
![](https://raw.githubusercontent.com/igordonxiao/word-master/master/screenshot/terminal.png)


