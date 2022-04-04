# RUW Dataset

​该数据集由中国石油大学（华东）青岛软件学院、计算机科学与技术学院大数据智能处理创新团队发布。

​该数据集是在撰写《Public Opinion Dynamics on Ukraine War in  Cyberspace: A Case Analysis with Chinese Weibo》论文期间收集到的舆情数据，数据集中的数据均来源于微博平台，由微博网民发布，内容与俄乌战争相关。



## Info

​我们使用实验室研发的舆情数据收集平台对微博中在2022年2月19日至2022年3月5日时间范围内的数据进行了收集，以“中国乌克兰撤侨”、“俄乌谈判进展”、 “SWIFT俄罗斯”、 “支持俄罗斯”等关键词作为筛选条件，共收集到15万条微博数据。然后我们对数据进行了处理，清除了过短和过长的博文数据，控制博文长度在40-150个字符长度之内，并去除停用词、特殊表情符号、重复博文与缺失博文。处理后最终得到了约10万条数据。2022年3月5日之后的数据仍在爬取中，在数据收集并处理完毕后，我们会将新数据更新到该数据集中。

​在数据分析阶段所使用的数据的主要字段信息如下表所示：

| 字段名称        | 类型    | 备注                 |
| --------------- | ------- | -------------------- |
| index           | int     | 数据索引             |
| create_at       | date    | 文本创建日期         |
| pub_time        | date    | 文本发布日期         |
| msg_id          | long    | 文本在微博平台中的ID |
| text            | string  | 文本内容             |
| text_length     | int     | 文本长度             |
| source          | string  | 发布文本的设备       |
| reposts_count   | int     | 文本转发数量         |
| comments_count  | int     | 文本评论数量         |
| attitudes_count | int     | 文本点赞数量         |
| isLongText      | boolean | 长文本标志           |
| user_id         | long    | 文本作者的ID         |
| screen_name     | string  | 文本作者的昵称       |
| gender          | string  | 文本作者的性别       |
| verified        | boolean | 是否是微博认证用户   |
| verified_type   | int     | 认证方式             |
| follow_count    | int     | 文本作者的关注数量   |
| followers_count | int     | 文本作者的粉丝数量   |
| description     | string  | 文本作者的简介       |



## License

*RUW-Dataset* is Apache 2.0 licensed. See the [`LICENSE`]([RUW-Dataset/LICENSE at main · upcbdipt/RUW-Dataset (github.com)](https://github.com/upcbdipt/RUW-Dataset/blob/main/LICENSE)) file.

Contact: Weishan Zhang ([zhangws@upc.edu.cn](mailto:zhangws@upc.edu.cn))

 

 
