# 川叶的 Rime 输入法私房菜

这个配置文件以 Rime 的默认配置为基础，以拼音输入方案作为优化方向，支持全拼和双拼。

采用 patch 进行设置，可使用 plum 「东风破」 更新基础方案配置，而不影响本配置作用。

以字词过滤的方式可选地缩小规范字词范围，而非缩减词表。

## 使用方法

先安装[RIME中州韵](https://rime.im/)输入法。

### Windows - Weasel 小狼毫

将本目录覆盖 `%appdata%\Rime` 文件夹

![](https://user-images.githubusercontent.com/555062/169637295-bcafc054-94ad-4744-a9c0-bb27eb619eee.png)

![](https://user-images.githubusercontent.com/555062/169637437-68246475-b5ee-40ff-8127-61d9f04b55ee.png)

![](https://user-images.githubusercontent.com/555062/169637478-163b8836-b4e2-40fa-90b3-0f959de42540.png)

![](https://user-images.githubusercontent.com/555062/169648094-3450227e-e48c-40ee-b1af-3df6e69bc7d2.png)


### Linux - ibus-rime

将本目录覆盖 `~/.config/ibus/rime` 文件夹

### Mac - Squirrel 鼠须管

将本目录覆盖 `~/Library/Rime` 文件夹

## 预装预调输入方案

* 明月拼音（默认）
* 小鹤双拼
* 地球拼音

## 注意事项

* Rime 的默认基础是**繁体**字（传承字）
  * 词库都是以繁体为基础存储的
  * 这样才能正确保留繁-简多对一转换关系
* 这个配置默认打开了CJK常用字过滤
  * Unicode 0x4E00~0x9FFF
  * 这样避免大多数平台上罕见字显示方块的问题
* 默认启用了 emoji
  * Windows 下目前 Weasel 还只能显示黑白 emoji

## 特性

默认只开启了小鹤双拼[配置文件](double_pinyin_flypy.custom.yaml)，其它双拼或全拼方案可以参照设置。

- [x] 支持用户自定义短语
- [x] 更好的标点符号输入，符合当前流行输入法配置
- [x] 支持CJK常用字过滤，可开关
  * [ ] 为部分罕见字增加例外（例如：𬌗）
  * [x] 用*标记《通用规范汉字表》以外的汉字，在简体常用字状态下开启
- [x] 支持emoji，可开关
- [x] 开启「八股文」语法模型，输入长句时更准确
- [ ] 标记国家标准中的简体中文异形词和错别字，可开关
- [ ] 支持拆字读音查字
- [ ] ？支持中英文混拼及常见混拼词汇（如多拉A梦）
- [ ] 更丰富的词典，以及专业词典
  * [x] 常见古诗词
  * [ ] 大陆常见地名
  * [ ] 大陆常见网络词汇
  * [ ] 大陆软件开发常用词汇
  * [ ] 大陆医学常用词汇
  * [ ] ？维基词典
- [ ] ？标注陆港台专业词汇所属地域
