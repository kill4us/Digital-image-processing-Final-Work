# Digital-image-processing-Final-Work
数字图像处理期末课程设计--基于opencv的欢乐斗地主记牌器

## 使用opencv对静态图像进行处理，截取出牌面

- 把图像分成上中下三块，分别是地主牌、对手出牌、自己手牌，计算出大致区域，直接切片选取

- 读取图片，转为SHV提取白色区域转回RGB
- 转为灰度图片，进行开闭操作
- 轮廓查找，筛选轮廓
- 截取牌面

## 截图时机判断
- 用win的API截图，比较快（~~截图是保存文件  还是~~  作为参数传递）
- 地主牌出现翻出的时候，进行手牌的截取
- - 出牌就截屏
- - 时时刻刻截屏，比较差异

## 字母、数字识别
- 自行通过模板匹配进行识别
- 使用现成的ocr识别

## 业务逻辑实现
- 只进行一次手牌识别
- 持续识别对手出牌
- 牌库计算

## 用户交互界面
- 小一点