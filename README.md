# Document-Timeline

## 简介

这是一个按文档创建时间来罗列文档的时间轴小挂件。可以通过缩放、拖拽时间轴的方式来直观地查看某一年、某一月、某一日创建了哪些文档。适用于思源笔记，演示时的笔记版本为：V2.7.2

实现：得益于 [visjs/vis-timeline](https://github.com/visjs/vis-timeline?utm_source=ld246.com)，通过SQL查询到的数据可以直观地在时间轴上展示出来。

## 基本使用

在文档中插入挂件，调整到合适大小后即可使用。

可参考社区帖子里的视频演示：[https://ld246.com/article/1676374370747](https://ld246.com/article/1676374370747)

> 注意：默认是查询所有已打开的笔记本里的文档，所以在文档较多时，嵌入挂件后，拖拽时间轴或者调整挂件大小可能会卡顿。在调整挂件大小前，建议先放大时间轴（鼠标滚轮往前滚），滚动到加载的节点比较少的比例后再调整挂件大小，这样调节过程会比较顺畅。

时间轴上：

* 单击文档标题会选中该项
* 双击文档标题会跳转到该文档。
* 鼠标悬浮在文档标题上时，底部一栏会显示该文档的创建时间

顶栏：

* 顶栏设置好起止时间后，点击 `聚焦`，即可聚焦到该时间段内。主要为了快速定位到指定区间，不用手动划拉时间轴。使用场景比如：查看最近一个月内创建的文档。
* 输入框内输入单个关键字或者空格隔开的多个关键字，然后按回车键或者点击`搜索`按钮即可开始检索，检索成功后时间轴上会罗列包含关键字的文档。
