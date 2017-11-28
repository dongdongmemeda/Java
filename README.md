## Java

    author: 蔡东
    desc: 本科毕业设计-基于DES加密的即时通信聊天系统（Windows系统运行）
    createdOn: 2017/3/25

## 操作说明 
#### 配置环境，安装Java，配置数据库MySQL
    
    1.用Eclipse编辑器分别打开两个项目
    2.运行client.java文件和server.java文件
    
##  客户端代码

    client.java: 客户端主程序，负责载入的界面
    clientThread.java: 客户端辅助线程，负责处理服务器的响应
    alert.java: 用于提示用户操作信息
    repaint.java: 重绘达到实时效果，并解决界面最小化再打开后空白界面
    ddd.java: 调用音频线程
    des.java: des加密算法，进行消息的加密解密
    res.java: 负责处理添加好友权限请求

## 服务器代码

    server.java: 服务器主程序，负责载入界面
    serverThread.java: 服务器辅助线程，避免卡死主线程，负责客户端各种请求的处理和数据库操作
    alert.java: 用于提示用户操作信息
    repaint.java: 重绘达到实时效果，并解决界面最小化再打开后空白界面

## 客户端外部文件说明

    ddd.mid: 语音提示声音
    savePath.txt: 客户端接受传输文件的保存路径
    serverip.txt: 服务器的IP地址
    keyFile: DES加密解密的密钥
    img: 个性化商标
    
##  服务器外部文件说明

    savePath.txt: 服务器接手客户端离线发送的文件路径
    img: 个性化商标
    
