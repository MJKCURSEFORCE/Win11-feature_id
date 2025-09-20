# Win11-feature_id
这里会整理一些有关Win11（beta或正式版）的feature id，可能会包含已经推出的功能的id。这个项目会持续更新。  
来源主要于betawiki和@phantomofearth的推文
> [!NOTE]
> 有些功能需要加入预览体验计划后才能出现。

## 激活\使用
> [!IMPORTANT]
> 这些id需要配合vivetool激活

激活：
```
vivetool /enable /id:[feature id] /variant:[自然数]
```
variant是功能的变种，如果不填则默认为0。feature id必填。

禁用:
```
vivetool /disable /id:[feature id]
```
当然，你可以提高这个id的激活权限，通常最高为2
```
vivetool /enable /id:[feature id] /variant:[自然数] /priority:[≥2的自然数]
