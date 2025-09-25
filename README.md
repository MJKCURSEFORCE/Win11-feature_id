# Win11-feature_id
![欢迎](image/1758386839626.png)  
这里会整理一些有关Win11（beta或正式版）的feature id，可能会包含已经推出的功能的id。这个项目会持续更新。  
> 来源主要于betawiki和@phantomofearth的推文  

> [!NOTE]
> 有些功能需要加入预览体验计划后才能出现，或者永远没有效果。

> [!CAUTION]
> 部分功能是实验性功能，启用后可能会出现一些奇怪的现象。（或者bug）

## 查询和更新
24H2的最新feature id[在这里](24H2-25H2/20250925_24H2-id.txt)  
当然可以在`code`中找到相应的版本就能看见。  
**这些文件随时会更新，更新时会标明日期。**
> 通常来讲，在功能名字前面带`*`的就是新添加的

## 激活和禁用
> [!IMPORTANT]
> 这些id需要配合相关的feature id管理工具使用，这里只演示vivetool。

激活：
```
vivetool /enable /id:[feature id] /variant:[变种(自然数)]
```
`variant`是功能的变种，如果不填则默认为0。feature id必填。

禁用:
```
vivetool /disable /id:[feature id]
```
这些是常用的激活和禁用命令。例如:
```
vivetool /enable /id:56005157
```

当然，你可以提高这个id的激活权限，通常最高为2
```
vivetool /enable /id:[feature id] /variant:[变种(自然数)] /priority:[权重(≥2的自然数)]
```
例如:
```
vivetool /enable /id:56005157 /priority:2
```
> [!TIP]
> 若要启用多个id，可以使用英文半角形式的逗号`,`连接。例如:

```
vivetool /enable /id:56005157,48801541
```

其它也是同理。
## 涉及版本
- [x] Windows 11 24H2
- [ ] Windows 11 25H2
