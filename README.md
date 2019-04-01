# SYSUtower 逸仙塔

## 项目简介

用于PC端和移动端的**中大新闻通知聚合客户端**，可**实时推送**，可自动生成**关键词**和**摘要**。提供**消息源定制**与**未读消息提醒**的功能，同时在阅读时可给予您清爽的阅读体验。

## 功能简介

1. 消息聚合：实时抓取并推送中大各个部门和学院官方网站上的通知新闻，以及学院、部门和社团微信公众号的推送。支持手动添加需要抓取推送的公众号。
2. 自动摘要：利用算法自动生成消息摘要和关键词。
3. 阅读提醒：对含特定关键字的消息发送阅读提醒，对含有姓名学号等个人信息的消息进行特殊提醒。同时支持使用关键字对消息进行查找筛选。
4. 页面简化：点击阅读全文时可去除原网页或推送中与消息正文无关的元素。
5. 智能下载：下载通知附件时支持智能更名（使用原通知中的中文名称）。
6. 全文搜索：支持对推送过的消息及其附件的标题，内容进行全文搜索。

## 分工简介

项目基本使用C++进行开发，少部分模块会按需要使用Python降低开发难度。

界面设计（2人）：PC端和移动端各一人，各自利用Qt进行用户界面的设计和与爬虫和智能算法交互部分的开发。

算法开发（1人）：设计用于生成摘要和关键字系统的智能算法。

爬虫搭建（1人）：开发用于抓取新闻消息和推送的的网络爬虫。

产品测试（1人）：对开发好的用户界面，爬虫和智能算法进行功能测试和用户体验测评。

## 开发日程

| 时间     | 界面设计                   | 算法开发                       | 爬虫搭建                                                     | 产品测试                                             |
| -------- | -------------------------- | ------------------------------ | ------------------------------------------------------------ | ---------------------------------------------------- |
| 第七周   | 设计窗口基本布局和功能安排 | 对已有的通知推送文本进行分析   | 分析学院部门网页布局，寻找推送获取接口，                     | 检查窗口布局的合理性                                 |
| 第八周   | 实现基本的打开跳转功能     | 实现基本的关键字和摘要生成算法 | 编写爬虫代码并设计调用接口与数据返回格式                     | 检查爬虫代码，测试界面功能                           |
| 第九周   | 实现关键字筛选和检索功能   | 利用NLP提高算法的精准度        | 对爬虫的效率和可用性进行测试，设计消息和附件内容查找功能接口 | 辅助进行爬虫测试，测试查找功能，测试关键字和摘要算法 |
| 第十周   | 实现消息提醒功能           | 实现算法的自动学习功能         | 对查找功能接口进行测试                                       | 测试消息提醒功能                                     |
| 第十一周 | 修正用户体验不佳的部分     | 针对新的消息内容进行测试修正   | 对爬虫和查找功能进行进一步优化                               | 整体用户体验测试                                     |

