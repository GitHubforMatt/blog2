---
title: Python Flask构建可扩展的RESTful API
date: 2018-10-11 16:55:21
tags:
  - 后端开发
  - 慕课网
  - 2018
  - Python
  - Flask
categories:
  - 后端开发
keywords: Python Flask构建可扩展的RESTful API
---
![image](//szimg.mukewang.com/5b061fe30001db4505400300-360-202.jpg)

Python Flask构建可扩展的RESTful API
前后端分离大势所趋，本课程将构建一套优秀的RESTful API，可以适配小程序、App 、wap 、web前端页面，除此之外，课程扩展了Flask框架机制，培养编程思维，随心所欲玩转Flask。优秀完整的RESTful API框架，你也可以实现。还等什么，来试试吧！

<!-- more -->
<blockquote class="blockquote-center">
请支持原版！课程官方链：http://coding.imooc.com/class/220.html</blockquote>
</blockquote>

第1章 随便聊聊
聊聊Flask与Django，聊聊代码的创造性

1-1 Flask VS Django
1-2 课程更新维护说明
第2章 起步与红图
本章我们初始化项目，探讨与研究Flask的默认层级结构。当我们遇到层级结构不合理时，我们将模仿蓝图自己定义一个“红图”来扩展Flask层级体系

2-1 环境、开发工具与flask1.0
2-2 初始化项目
2-3 新建入口文件
2-4 蓝图分离视图函数的缺陷
2-5 打开思维，创建自己的Redprint——红图
2-6 实现Redprint
2-7 优化Redprint
第3章 REST基本特征
本章我们将探讨REST的基本特征，并结合实际情况给出REST的适用范围与优劣势

3-1 REST的最基本特征（可选观看）
3-2 为什么标准REST不适合内部开发（可选观看）
第4章 自定义异常对象
异常处理其实是一个非常严肃而又麻烦的事情，这直接涉及到前端如何对用户做出响应。本章我们将重写HTTPException并建立全局异常处理机制，统一处理框架内的异常，向前端返回统一而标准的异常信息，简化前端的开发流程

4-1 关于“用户”的思考
4-2 构建Client验证器
4-3 处理不同客户端注册的方案
4-4 创建User模型
4-5 完成客户端注册
4-6 生成用户数据
4-7 自定义异常对象
4-8 浅谈异常返回的标准与重要性
4-9 自定义APIException
第5章 理解WTForms并灵活改造她
WTForms其实是非常强大的验证插件。但很多同学对WTForms的理解仅仅停留在“验证表单”上。那WTForms可以用来做API的参数验证码？完全可以，但这需要你灵活的使用它，对它做出一些“改变”

5-1 重写WTForms 一
5-2 重写WTForms 二
5-3 可以接受定义的复杂，但不能接受调用的复杂
5-4 已知异常与未知异常
5-5 全局异常处理
第6章 Token与HTTPBasic验证 —— 用令牌来管理用户
在我的TP5课程里，我们使用令牌的方式是服务器缓存的方式。那么在Python Flask中我们换一种令牌的发放方式。我们将用户的信息加密后作为令牌返回到客户端，客户端在访问服务器API时必须以HTTP Basic的方式携带令牌，我们再读取令牌信息后，将用户信息存入到g变量中，共业务代码全局使用...

6-1 Token概述
6-2 获取Token令牌
6-3 Token的用处
6-4 @auth拦截器执行流程
6-5 HTTPBasicAuth基本原理
6-6 以BasicAuth的方式发送Token
6-7 验证Token
6-8 重写first_or_404与get_or_404
第7章 模型对象的序列化
最适合Python JSON序列化的是dict字典类型，每一种语言都有其对应的数据结构用来对应JSON对象，比如在PHP中是它的数组数据结构。而Python是用字典来对应JSON的。如果我们想直接序列化一个对象或者模型对象，那么最笨的办法是把对象的属性读取出来，然后组装成一个字典再序列化。这实在是太麻烦了。本章节我们将深入了解JSO...

7-1 鸡汤？
7-2 理解序列化时的default函数
7-3 不完美的对象转字典
7-4 深入理解dict的机制
7-5 一个元素的元组要特别注意
7-6 序列化SQLAlchemy模型
7-7 完善序列化
7-8 ViewModel对于API有意义吗
第8章 权限控制
我看过太多同学编写的API在互联网上疯狂的裸奔了。殊不知这太危险了。API必须提供分层保护机制，根据不同用户的种类来限制其可以访问的API，从而保护接口。比如管理员可以访问哪些接口，普通用户可以访问哪些接口，小程序可以访问哪些，APP又能够访问哪些？灵活而强大的可配置Scope，可以帮助你事半功倍...

8-1 删除模型注意事项
8-2 g变量中读取uid防止超权
8-3 生成超级管理员账号
8-4 不太好的权限管理方案
8-5 比较好的权限管理方案
8-6 实现Scope权限管理 一
8-7 globals()实现“反射”
8-8 实现Scope权限管理 二
8-9 Scope优化一 支持权限相加
8-10 Scope优化 二 支持权限链式相加
8-11 Scope优化 三 所有子类支持相加
8-12 Scope优化 四 运算符重载
8-13 Scope 优化 探讨模块级别的Scope
8-14 Scope优化 实现模块级别的Scope
8-15 Scope优化 七 支持排除
第9章 实现部分鱼书小程序功能
理论必须结合实践，我们提供一个简单的鱼书小程序，编写他的业务接口，并用小程序来进行API的检验

9-1 小程序演示API调用效果
9-2 模糊搜索书籍
9-3 再谈严格型REST的缺陷
9-4 实现hide方法
9-5 @orm.reconstructor 解决模型对象实例化问题
9-6 重构hide与append
9-7 赠送礼物接口
9-8 实现获取令牌信息接口
本课程已完结

<blockquote class="blockquote-center">声明：此资源由巨菜站博客 收集整理于网络，如有侵权，请联系巨菜站删除处理。</blockquote>

<div id="jspay" sid="AA4FRl82113" style="display:none">AA4FRl82113</div>
<script type="text/javascript" src="https://www.fageka.com/j.js"></script>
<script type="text/javascript" src="https://www.fageka.com/f.js" charset="utf-8"></script>
