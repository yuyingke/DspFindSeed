- ![CP$EF 8PNKTZKH@6LPV3N86](https://user-images.githubusercontent.com/34654211/134377457-afd77049-fa29-490e-824d-40e85af3326c.png)

# 使用说明

#### 如何开始搜索？
- 填写种子ID，添加任意条件，点开始按钮即可开始搜索。
- 单次搜索次数建议1000-10000（一万个大概在30-60秒搜索完），对应一个进程搜100-1000次
- 追求效率多开到5-10个进程（视电脑cpu能力而定）


#### 字段都什么意思？
- 条件区基本是字面意思
- 最上面的三个条件，磁石总数、蓝巨星总数、0型恒星总数，是全宇宙的总数条件
- 下面的所有条件都是搜索一个满足条件的恒星系
- 由于戴森球计划恒星系最大星球数量是6，所以开放了6个星球类型选项，不用全选，全选=搜有6个特定星球的星系
- 矿物数量1单位指一堆矿物，具体多少涉及星球地形的生成算法，会把你搜索时间30秒每万个，变成100秒每万个（大概），所以没有开放
   - 基本稀有矿有1堆已经足够大部分需求了
- 至少几个星系满足条件可以满足多个星系的追求
   - 例如希望想搜3个0星系都是2.5亮度以上，可以选成3，这样必须有3个这样星系的种子才会命中保存

#### 有一些模棱两可的条件怎么办？
- 只有满足了所有必须条件的星系种子才会视为命中了搜索条件
- 一些不强求但是想看看数据作为参考的条件请添加成仅记录条件


#### 多开需要重新选条件吗？
- 配置好了所有条件之后使用导出条件，可以选择将配置项以json的方式导出
- 然后在新程序中选择导入条件即可


#### 不想按顺序搜种子怎么办？
- 支持导入种子ID，要求文件格式是CSV，第一列写种子的ID即可（搜索结果导出的csv文件就满足这个格式）。
- 所以，可以先粗选，再导入结果细选，套娃搜索
- 同样，也可以选择单个种子详细信息，填种子ID恒星数量就可以

#### 搜一半不想搜了怎么办？
- 点终止或者关闭窗口都可以结束搜索。（会有二次确认）

## 更新日志
- 1.9版本
  增加了恒星数量区间，可以选择最小恒星数量和最大恒星数量，每个种子ID将把对应区间的种子全部搜索完才搜下一个
- 1.6版本
  - 更新了行星类型的参数下拉列表
  - 增加了关闭窗口的二次确认，同时关闭窗口会杀掉后台的搜索线程
  - 优化了输出的内容
  - 修复了是否有硫酸的结果输出不对的问题
- 1.5版本
  - 更新了恒星类型的参数下拉列表
  - 优化了输出的内容
- 1.4版本
  - 修复导出条件报错的问题
- 1.3版本
  - 更新了高效率重氢的筛选条件，搜索结果也会显示命中星系的最大重氢速率了（适配官方Version 0.8.21.8562新增的高效重氢气态巨星类型）
    
- 1.0版本
  - 增加了恒星数的选项，可以选择32-64不同的恒星数
- 0.9版本
  - 增加了导入种子ID的csv进行搜索的方式
  - 优化了搜索log和进度显示，增加了终止搜索按钮，增加了一些弹窗提示
  - 潮汐锁定的数量只计算永昼永夜类型的潮汐锁定
- 0.8版本
  - 增加了蓝巨星总数的筛选条件（与磁石相同是整个宇宙的条件）
  - 星系条件里增加了，是否是蓝巨星星系，冰巨星数量，戴森球是否包含第二颗行星的条件
  - 优化了磁石数量的算法
- 0.6版本
  - 修复了两个BUG
     1. 现在csv文件中会正确记录种子ID了
     2. 现在修改文件名会正确的生效了 
- 0.5版本
  - 增加了单个种子详细数据的写入功能（方便已经开局的游戏，查看全星系数据）
  
- 0.3版本
  - 优化了UI布局和说明
  - 增加了气态巨星数量的筛选条件

- 0.2版本
  - 增加了条件的导入、导出功能

