Kaggle竞赛宝典

竞技数据科学中的数据分析与机器学习

<!-- Media -->

<!-- figureText: Foreword by: Anthony Goldbloom Founder & CEO, Kaggle -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_0.jpg?x=0&y=956&w=1888&h=1080&r=0"/>

<!-- Media -->

康拉德·巴纳切维茨 Packt> 卢卡·马萨龙

## Kaggle竞赛宝典

竞技数据科学中的数据分析与机器学习

康拉德·巴纳切维茨

卢卡·马萨龙

<!-- Media -->

<!-- figureText: Packt> -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_1.jpg?x=241&y=1693&w=432&h=135&r=0"/>

<!-- Media -->

伯明翰-孟买

Packt出版社及本书与Kaggle平台无官方关联。本书是Kaggle专家社区为助力开发者成长而编撰的成果。

## Kaggle竞赛宝典

版权所有 (C) 2022 Packt出版社

保留所有权利。未经出版者事先书面许可，本书任何部分不得以任何形式或通过任何方式复制、存储在检索系统中或传播，但用于关键性文章或评论的简短引用除外。

本书编撰过程中已尽力确保所述信息准确。但书中信息按现状提供，不作任何明示或暗示的担保。对于因使用本书直接或间接导致的任何损失，作者、Packt出版社及其经销商均不承担责任。

Packt出版社已通过规范使用大写字母，尽力提供本书提及的所有公司和产品的商标信息。但不能保证这些信息的准确性。制作人：图沙尔·古普塔

组稿编辑 - 同行评审：萨比·德席尔瓦

项目编辑：帕尔瓦西·奈尔

内容开发编辑：Lucy Wan

文字编辑：Safis Editing

技术编辑：Karan Sonawane

校对员：Safis Editing

索引编制员：Sejal Dsilva

版式设计师：Pranit Padwal

首次出版：2022年4月

生产编号：2220422

由Packt Publishing Ltd.出版

Livery Place

35 Livery Street

伯明翰

B3 2PB，英国

ISBN 978-1-80181-747-9

www.packt.com

我拥有计量经济学背景，但对机器学习技术产生了兴趣，最初是将其作为解决预测问题的替代方法。当我开始发现这一兴趣时，发现这个领域令人望而生畏：我不懂相关技术、术语，也没有能够让我进入这一领域的资质。

我一直梦想着Kaggle能为我这样的人提供进入这个强大新领域的机会。最令我自豪的是，Kaggle极大地降低了数据科学和机器学习的门槛。许多Kaggle用户从新手成长为顶尖机器学习专家，被英伟达、谷歌和OpenAI等公司录用，还创立了DataRobot这样的企业。

卢卡和康拉德的著作进一步降低了Kaggle的参与门槛。这本书既介绍了Kaggle的运作机制，也分享了他们在该平台积累的核心经验。两人合计拥有超过20年的Kaggle会员资历，参加过330场竞赛，发布过2000多篇论坛帖子，分享了100多份笔记和50个数据集。他们都是平台排名顶尖、备受尊敬的社区成员。

完成本书学习的读者将能自信参与Kaggle活动——而这份自信会带来丰厚回报。

首先，这是掌握机器学习最实用进展的有效途径。该领域发展迅猛——2019年每天就有300多篇机器学习论文通过同行评审。如此海量的文献使人难以追踪前沿。Kaggle却能高效筛选出对现实问题真正重要的进展。其价值不仅限于学术追踪，许多行业标准工具（如2014年的XGBoost和2015年的Keras）都是通过该平台普及的。其次，Kaggle提供"实践学习"的机会。活跃用户将定期参赛比作机器学习的"力量训练"，平台上多样的案例演练能完美对接工业界需求。竞赛截止日期则培养了快速迭代能力——没有什么比先解题再观摩优胜者方案（赛后分享是惯例）更好的学习方式了。

对于初识Kaggle的读者，希望本书能消除你们的畏难情绪；而对于资深用户，愿这两位顶尖大师的著作助你们更上一层楼。

安东尼·戈德布卢姆

Kaggle创始人兼CEO

## 关于作者

康拉德·巴纳切维兹拥有阿姆斯特丹自由大学统计学博士学位。学术生涯中，他专注于信用风险领域的极端依赖建模问题，同时担任硕士生导师。从经典统计学出发，他逐步转向数据挖掘与机器学习（当时"数据科学"和"大数据"尚未成为流行词）。

取得博士学位后的十年间，康拉德在多家金融机构处理各类量化数据分析问题，成为数据产品全周期专家。他涉足金融频谱的各个维度（从高频交易到信用风险），预测过马铃薯价格，分析过大型工业设备的异常性能。

作为站在巨人肩膀上的受益者，康拉德坚信知识共享理念。业余时间，他在"数据科学之家"Kaggle上参与竞赛。

感谢我的兄弟在这混乱世界始终如磐石，持续给予我灵感和动力。Dzieki, Braciszku（波兰语：谢谢你，兄弟）。

卢卡·马萨伦是拥有十余年经验的数据科学家，擅长将数据转化为智能解决方案，解决现实问题并创造商业价值。他著有关于人工智能、机器学习和算法的畅销书，同时是Kaggle最高级别宗师（全球排名第七）和谷歌机器学习领域开发专家。

衷心感谢我的家人由纪子和阿米莉亚，在我漫长的创作过程中给予支持与包容。

特别致谢安东尼·戈德布卢姆为本书作序，以及所有热情提供访谈、建议和帮助的Kaggle大师与宗师们。

最后，感谢塔沙尔·古普塔、帕瓦蒂·奈尔、露西·万、卡兰·索纳瓦尼等Packt出版社全体编辑制作人员的支持。

## 关于审稿人

安德烈·科斯坚科博士是数据科学与机器学习专家，在多个学科和行业拥有丰富经验，包括使用R和Python进行实际编程，构建、训练并部署时间序列模型用于预测等应用场景。他认为终身学习与开源软件对高级分析和人工智能领域的创新至关重要。

安德烈现任水信息研究所（H2i.sg）首席数据科学家，该机构是水资源管理全领域的专业咨询与解决方案服务商。在加入\( \mathrm{H}2\mathrm{i} \)之前，他曾在IAG保险科技创新中心担任高级数据科学家三年有余。2018年移居新加坡前，他在澳大利亚广告科技初创企业TrafficGuard.ai担任数据科学家，开发用于移动广告欺诈检测的新型数据驱动算法。2013年，安德烈获得澳大利亚莫纳什大学数学与统计学博士学位，此前已持有英国MBA学位和俄罗斯的本科学位。

业余时间里，安德烈常参与数据科学竞赛项目，学习R和Python生态系统的新工具，探索Web开发最新趋势，破解国际象棋残局，或研读科学史与数学史著作。

菲拉特·戈宁博士现任Getir数据科学与分析总监，领导团队实施创新型尖端机器学习项目。加入Getir前，他曾管理沃达丰土耳其公司人工智能团队，更早时担任土耳其最大企业集团之一Doğuş Group的首席数据科学家。戈宁博士拥有休斯顿大学神经科学与神经网络博士学位，是机器学习、深度学习、视觉注意力、决策制定与遗传算法领域的专家，具备12年以上从业经验，发表过多篇同行评审期刊论文。他还是Kaggle三冠大师，获得过10余枚国际数据竞赛奖牌，并曾当选为\( {2020}\mathrm{\;Z} \)惠普数据科学全球大使。

## 关于受访者

我们有幸采访了Kaggle社区的31位优秀成员，邀请他们分享平台使用心得。他们的回答散见于本书各处，呈现出多元视角——诸多深刻见解既相似又各具特色。我们怀着极大兴趣研读每份贡献，相信读者您亦会如此。在此向所有受访者致谢，并按字母顺序列出名单：

阿布舍克·塔库尔，现于Hugging Face开发AutoNLP项目

阿尔贝托·达内塞，Nexi公司数据科学总监

安德拉达·奥尔泰亚努，Endava数据科学家、Weights and Biases开发专家兼Z by HP全球数据科学大使

安德鲁·马拉尼昂，圣保罗阿尔伯特·爱因斯坦医院高级数据科学家

安德烈·卢基扬年科，MTS集团机器学习工程师兼技术主管

博扬·通古兹，NVIDIA机器学习建模师

克里斯·迪奥蒂，NVIDIA高级数据科学家兼研究员

丹·贝克，DataRobot决策智能产品副总裁

德米特里·拉尔科，H2O.ai首席数据科学家

Getir数据科学与分析主管兼惠普全球数据科学大使菲拉特·戈南(Firat Gonen)。

Endava首席数据科学家加布里埃尔·普雷达(Gabriel Preda)。

英伟达(NVIDIA)高级数据科学家吉尔伯托·蒂特里茨(Gilberto Titericz)。

Zillow集团机器学习与自然语言处理高级应用科学家朱利亚诺·詹森(Giuliano Janson)。

英伟达(NVIDIA)杰出工程师、RAPIDS项目负责人，兼英伟达Kaggle大师团队经理让-弗朗索瓦·普盖(Jean-François Puget)。

Netflix研究院排序与搜索算法工程团队高级研究科学家李正允(Jeong-Yoon Lee)。

英伟达(NVIDIA)高级深度学习数据科学家兼KGMON团队成员小野寺和树(Kazuki Onodera)。

Micromata数据科学主管劳拉·芬克(Laura Fink)。

Edison Software天体物理学博士、数据科学家马丁·亨泽(Martin Henze)。

ForecomAI机器学习科学家、剑桥大学计算机科学专业学生米克尔·博伯-伊里扎尔(Mikel Bober-Irizar)。

大阪大学医学博士秋山修(Osamu Akiyama)。

H2O.ai数据科学家帕鲁尔·潘迪(Parul Pandey)。

LogicAI首席数据科学家兼AI工程师、联合创始人帕维尔·扬凯维奇(Pawel Jankiewicz)。

Biocore LLC高级数据科学家罗布·穆拉(Rob Mulla)。

H2O.ai高级数据科学家罗汉·拉奥(Rohan Rao)。

OpenMined数据科学家、惠普全球数据科学大使、卡内基梅隆大学研究生鲁奇·巴蒂亚(Ruchi Bhatia)。

H2O.ai公司的数据科学家瑞安·切斯勒(Ryan Chesler)。

日本某新闻媒体公司的数据科学家兼研究员石原翔太郎(Shotaro Ishihara)。

初创企业人工智能/机器学习顾问苏达莱·拉吉库马尔(Sudalai Rajkumar)。

数据测绘与工程公司创始人兼首席执行官泽维尔·科诺特(Xavier Conort)。

数据科学咨询公司Arion Ltd联合创始人谢逸凡(Yifan Xie)。

伦敦国王学院应用机器学习方向博士生张亦伦(Yirun Zhang)。

## 加入我们的图书Discord空间

加入本书Discord工作区，每月参与作者问答会：

https://packt.link/KaggleDiscord

第一部分：竞赛入门 1

第一章：Kaggle及其他数据科学竞赛介绍 3

数据科学竞赛平台的兴起 4

Kaggle竞赛平台 \( \bullet  7 \)

Kaggle发展史 \( \bullet  7 \)

其他竞赛平台 \( \bullet  {10} \)

Kaggle简介 12

竞赛阶段 \( \bullet  {12} \)

竞赛类型与示例\( \cdot  {17} \)

提交与排行榜动态\( \bullet  {22} \)

解读通用任务框架范式\( \cdot  {23} \)

竞赛中可能出现的失误\( \bullet  {24} \)

计算资源\( \bullet  {26} \)

Kaggle笔记本\( \bullet  {27} \)

组队与社交网络\( \bullet  {28} \)

表现层级与排名\( \bullet  {32} \)

批评与机遇\( \bullet  {33} \)

总结 35

第二章：用数据集组织数据 37

建立数据集 37

数据收集 42

数据集操作 48

在Google Colab中使用Kaggle数据集 49

法律注意事项 51

摘要 52

第3章：Kaggle笔记本工作与学习指南 53

笔记本环境搭建 54

运行笔记本 58

将笔记本保存至GitHub 60

笔记本高效使用技巧 63

升级至Google云平台(GCP) \( \bullet  {64} \)

进阶指南 \( \bullet  {66} \)

Kaggle学习课程 73

摘要 77

第4章：讨论区高效利用 79

论坛运作机制 79

讨论方法示例 86

网络礼仪 92

摘要 93

第二部分：竞赛技能提升 95

第五章：竞赛任务与评估指标 97

评估指标与目标函数 98

任务基本类型 100

回归 \( \bullet  {100} \)

分类 \( \bullet  {100} \)

序数 \( \bullet  {101} \)

Meta Kaggle数据集 102

处理未见过的评估指标 105

回归指标（标准与序数）109

均方误差(MSE)与R平方 \( \bullet  {109} \)

均方根误差(RMSE) \( \bullet  {111} \)

均方根对数误差(RMSLE) \( \bullet  {112} \)

平均绝对误差(MAE) \( \bullet  {113} \)

分类指标（标签预测与概率）114

准确率 \( \bullet  {114} \)

精确率与召回率 \( \bullet  {116} \)

F1分数(F1 score) \( \bullet  {119} \)

对数损失与ROC曲线下面积(Log loss and ROC-AUC) \( \bullet  {119} \)

马修斯相关系数(Matthews correlation coefficient) \( \left( \mathrm{{MCC}}\right)  \bullet  {121} \)

多类别分类评估指标 122

目标检测问题评估指标 129

交并比(IoU) \( \bullet  {131} \)

戴斯系数(Dice) \( \bullet  {132} \)

多标签分类与推荐系统评估指标 133

平均准确率均值(MAP@) \( \{ K\}  \bullet  {134} \)

优化评估指标 135

自定义指标与目标函数 \( \cdot  {136} \)

预测结果后处理 \( \cdot  {139} \)

预测概率及其调整 \( \bullet  {141} \)

本章小结 146

第6章：设计有效的验证方案 149

排行榜数据窥探 150

竞赛中验证的重要性 153

偏差与方差 \( \bullet  {156} \)

尝试不同的数据划分策略 159

基础训练集-测试集划分 \( \bullet  {160} \)

概率评估方法 \( \bullet  {161} \)

k折交叉验证 - 161

子抽样 \( \bullet  {171} \)

自助法 - 171

调整模型验证系统 176

使用对抗验证 179

示例实现 \( \bullet  {181} \)

处理训练数据与测试数据的不同分布 \( \cdot  {183} \)

处理数据泄露 187

本章小结 192

第7章：表格数据竞赛建模 195

表格竞赛演练系列 196

设置随机状态以确保结果可复现性 202

探索性数据分析(EDA)的重要性 203

使用t-SNE和UMAP进行降维 - 205

缩减数据规模 208

应用特征工程 210

易于衍生的特征 \( \bullet  {211} \)

基于行和列的元特征 \( \bullet  {213} \)

目标编码 \( \bullet  {215} \)

利用特征重要性评估工作成果 \( \cdot  {220} \)

伪标签技术 224

使用自编码器降噪 226

面向表格竞赛的神经网络 231

本章小结 238

第八章：超参数优化 241

基础优化技术 242

网格搜索 \( \cdot  {243} \)

随机搜索\( \bullet  {245} \)

减半搜索\( \cdot  {246} \)

关键参数及使用方法 249

线性模型\( \bullet  {250} \)

支持向量机\( \bullet  {250} \)

随机森林与极端随机树\( \cdot  {251} \)

梯度提升树\( \bullet  {253} \)

LightGBM - 253

XGBoost • 255

CatBoost\( \bullet  {257} \)

直方图梯度提升\( \bullet  {258} \)

贝叶斯优化 261

使用Scikit-optimize\( \bullet  {262} \)

定制贝叶斯优化搜索\( \bullet  {268} \)

将贝叶斯优化扩展到神经架构搜索\( \cdot  {276} \)

用KerasTuner创建更轻量更快的模型\( \cdot  {285} \)

Optuna中的TPE方法\( \bullet  {295} \)

摘要 301

第9章：混合与堆叠解决方案的集成方法 303

集成算法简介 304

模型平均化集成 307

多数投票法\( \bullet  {309} \)

模型预测结果平均化\( \bullet  {312} \)

加权平均法\( \cdot  {314} \)

交叉验证策略中的平均化处理\( \cdot  {315} \)

ROC-AUC评估的校正平均法\( \bullet  {316} \)

使用元模型进行混合建模 317

混合建模最佳实践\( \cdot  {318} \)

模型堆叠方法 323

堆叠变体\( \bullet  {327} \)

构建复杂堆叠与混合解决方案 329

总结 333

第10章：计算机视觉建模 335

数据增强策略 335

Keras内置增强方法 \( \bullet  {341} \)

ImageDataGenerator方法 \( \bullet  {341} \)

预处理层 \( \bullet  {345} \)

albumentations库 \( \bullet  {346} \)

分类 349

目标检测 357

语义分割 371

本章小结 388

第11章：自然语言处理建模 389

情感分析 389

开放域问答 398

文本增强策略 414

基础技术 \( \bullet  {415} \)

nlpaug工具 \( \bullet  {420} \)

摘要 423

第12章：仿真与优化竞赛 425

连接X 426

石头剪刀布 431

2020年圣诞老人竞赛 435

游戏名称 439

摘要 444

第三部分：通过竞赛推动职业发展 445

第13章：构建项目与创意作品集 447

利用Kaggle构建作品集 447

活用Notebook与讨论区 \( \bullet  {452} \)

活用数据集 \( \bullet  {455} \)

在Kaggle之外经营线上形象 460

博客与出版物 \( \bullet  {460} \)

GitHub \( \bullet  {463} \)

追踪竞赛更新与订阅简报 465

摘要 467

第14章：寻找新的职业机遇 469

与其他竞赛数据科学家建立联系 470

参与Kaggle Days及其他Kaggle线下活动 481

获得关注与其他工作机会 482

STAR方法 - 483

总结（与临别赠言） 485

您可能感兴趣的其他书籍 489

索引 495

作为在Kaggle竞赛超过十年的参赛者，我们经历过许多比赛中的高峰与低谷。我们时常将重心转向与Kaggle相关的不同活动。随着时间推移，我们不仅投身竞赛，还根据数据科学市场需求与个人职业抱负，致力于创作内容与代码。在此旅程节点，我们感到自身积累的经验与未减的竞赛热情，能切实帮助那些刚起步或寻求灵感的参与者掌握必备专业技能，从而开启他们的数据科学竞赛之旅。

我们因此决定怀着明确目标撰写本书：

- 集中提供最佳建议，助您在Kaggle及其他数据科学竞赛中保持竞争力并应对各类问题

- 提供充足指导，使读者能在Kaggle任何领域（竞赛、数据集、笔记本或讨论）至少达到专家级别

- 分享如何从Kaggle最大化学习效果，并运用该经验促进数据科学职业发展

- 通过采访Kaggle大师与特级大师，汇集最多元化的竞赛参与经验视角

简言之，我们撰写的这本书既展示如何成功参与竞赛并充分利用Kaggle机遇，也是一本实用参考指南——精选了大量互联网或Kaggle论坛上难以获取的竞赛技巧，为您节省时间精力。但本书不止于实操指导，更旨在帮助您通过竞赛推动数据科学职业发展。请注意：本书不从基础教授数据科学知识。我们不会详解线性回归、随机森林或梯度提升的工作原理，而是重点讲解如何最优运用这些方法解决数据问题。我们期待读者具备扎实的数据科学基础知识和Python应用能力。若您仍是数据科学初学者，需配合其他数据科学、机器学习与深度学习书籍，并通过Kaggle自有课程或edX、Coursera等慕课平台进行补充学习。

若您希望以实践方式开启数据科学学习之旅，渴望通过棘手而迷人的数据问题挑战自我，同时构建一个由志同道合的数据科学家组成的专业网络——这些伙伴与您一样对数据工作充满热忱——那么这本书正是为您量身定制。让我们即刻启程！

## 本书目标读者

截至本书完成时，Kaggle竞赛已汇聚96,190名新手（刚完成网站注册的用户）与66,666名贡献者（刚完善个人资料的用户）。本书既为这些用户而写，也为所有希望打破坚冰、开始参与Kaggle竞赛并从中学习的探索者而作。

## 本书内容概览

## 第一部分：竞赛入门指南

第1章《认识Kaggle与其他数据科学竞赛》探讨竞技编程如何演变为数据科学竞赛，解析Kaggle平台成为最热门竞赛场地的原因，并带您了解其运作机制。

第2章《用数据集组织数据》介绍Kaggle平台标准数据存储方式——Kaggle数据集，涵盖配置、数据收集及在Kaggle工作中的实际应用。

第3章《Kaggle Notebooks实战学习》探讨基准编码环境Kaggle Notebooks，讲解Notebook基础操作、GCP环境运用技巧，以及如何借此构建数据科学作品集。

第4章《善用讨论论坛》带您熟悉Kaggle上主要的交流与创意交换方式——讨论论坛的使用方法。

## 第二部分：竞赛技能精进

第5章《竞赛任务与评估指标》详解特定类型问题的评估指标如何深刻影响您在数据科学竞赛中构建模型解决方案的操作方式，同时介绍Kaggle竞赛中丰富多样的评估指标体系。

第6章《设计优质验证方案》阐述数据竞赛中验证的重要性，讨论过拟合、数据扰动、泄露问题、对抗性验证、多种验证策略及最终提交策略。

第7章《表格类竞赛建模》聚焦Kaggle近年主流的表格竞技场系列（Tabular Playground Series），这类问题是全球数据科学家的标准实践领域，Kaggle平台蕴含丰富学习资源。

第8章《超参数优化》探索如何在Kaggle竞赛的时间与资源压力下，通过扩展交叉验证方法寻找模型最佳超参数——即能在私有排行榜上实现最优泛化表现的参数组合。

第9章《混合与堆叠集成方案》讲解多模型集成技术，包括平均法、混合法与堆叠法，提供理论指导、实践案例及可直接用作Kaggle解决方案模板的代码示例。

第10章《计算机视觉建模》探讨AI领域最热门主题——计算机视觉相关课题（尤其是Kaggle平台上的专项），完整演示图像分类、目标检测与图像分割挑战的解决方案构建流程。

第11章《NLP建模》重点探讨Kaggle竞赛中常见的自然语言处理挑战类型，我们将演示如何为开放域问答等热门问题构建端到端解决方案。

第12章《仿真与优化竞赛》概述了仿真类竞赛，这是近年来在Kaggle平台上逐渐兴起的新型赛事。

## 第三部分：通过竞赛推动职业发展

第13章《创建项目与创意作品集》探讨如何通过在Kaggle等平台恰当展示作品脱颖而出。第14章《探索职业新机遇》作为全书收尾，详细解析如何最大化利用Kaggle经验获取职业发展机会。

## 本书使用指南

本书Python代码专为Kaggle Notebook设计，无需本地安装。无需顾虑设备配置或Python包版本问题。

仅需联网设备和免费Kaggle账号。具体操作详见第3章，注册请访问www.kaggle.com按指引操作。

书中提供大量实用资源链接，包含可复用的公开Notebook代码及延伸学习材料，建议深入查阅。

## 下载示例代码文件

代码包存放于GitHub：https://github.com/PacktPublishing/The-Kaggle-Book。更多精品资源请访问https://github.com/PacktPublishing/。

## 下载彩色插图

本书彩图PDF下载地址：https://static.packt-cdn.com/downloads/9781801817479_ColorImages.pdf

## 排版约定

本书使用以下文本格式规范

代码字体：用于标示代码术语、数据库表名、路径名等。示例："数据集将以.zip格式下载至Kaggle文件夹，解压后即可使用。"

代码块格式如下：

---

从google.colab导入drive模块

挂载到/content/gdrive目录

---

命令行输入或输出示例如下：

---

我完全不知道这串单词会生成什么结果

- - 看看nlpaug能对此做出什么处理会很有趣！

---

粗体：表示新术语、重要词汇或屏幕上显示的词语（例如菜单或对话框中的文字）。例如："撰写时的具体限制是每个私有数据集\( {100}\mathrm{{GB}} \)，总配额为100GB。"

补充说明、参考文献和实用链接会以这种形式呈现。

技巧和小贴士会以这种形式展示。

## 联系我们

我们始终欢迎读者的反馈。

一般反馈：发送邮件至feedback@packtpub.com，并在邮件主题中注明书名。如有任何疑问，请邮件至questions@packtpub.com。

勘误：尽管我们力求内容准确，但错误仍在所难免。若发现书中错误，请通过http://www.packtpub.com/submit-errata提交，选择您的书籍，点击勘误提交表单链接并填写详细信息。

盗版举报：如在互联网上发现任何形式的盗版作品，请提供地址或网站名称。请发送侵权材料链接至copyright@packtpub.com。作者招募：如果您有专业领域知识并有意参与图书创作，请访问http://authors.packtpub.com。

## 分享您的想法

阅读完《Kaggle实战手册》后，我们期待您的宝贵意见！点击此处直达本书亚马逊评论页面提交反馈。

您的评价对我们和技术社区至关重要，这将帮助我们持续提供优质内容。—————— 第一部分

# 竞赛入门指南

## Kaggle与其他数据科学竞赛平台介绍

数据科学竞赛由来已久，从最初仅吸引少数狂热爱好者的小众活动，逐渐发展为备受瞩目、拥有数百万数据科学家参与的盛事。作为Kaggle——这个最受欢迎的数据科学竞赛平台上的长期参赛者，我们亲眼见证并切身经历了这一演变过程。

当前若搜索Kaggle等竞赛平台的相关信息，你会发现大量交流会、专题讨论、播客访谈甚至在线课程，都在传授制胜秘诀（通常强调毅力、计算资源与时间投入的混合运用）。但除了本书之外，你几乎找不到系统指导——如何驾驭众多数据科学竞赛并从中获取最大价值，这种价值不仅体现在分数排名，更关乎专业能力提升。

本书不仅提供Kaggle等竞赛的高分技巧，更旨在成为你在职业发展视角下优化参赛策略、最大化竞赛收益的指南。书中还收录了多位Kaggle大师与特级大师的专访，他们将从独特视角剖析参赛细节，激发你在竞技数据科学中自我检验与学习的方式。通过本书，你将汲取我们亲身经历的实战智慧、竞赛资源与经验总结，获得在逐场竞赛中持续成长的全方位指引。

本章作为起点，我们将追溯竞技编程如何演变为数据科学竞赛，解析Kaggle平台成为行业标杆的原因及其运作机制。

本章涵盖以下主题：

- 数据科学竞赛平台的兴起

- 通用任务框架范式

- Kaggle平台及其他替代方案

- Kaggle竞赛运作机制：阶段划分、赛事类型、提交与排行榜动态、计算资源、社交网络等

## 数据科学竞赛平台的崛起

竞技编程可追溯至1970年代的国际大学生程序设计竞赛（ICPC）初期。在原始ICPC赛事中，来自高校与企业的小型团队需编写计算机程序（早期使用FORTRAN语言）解决系列问题。要取得佳绩，团队需展现卓越的协作能力、问题解决技巧与编程实力。

紧张激烈的参赛体验与招聘企业的关注目光，赋予学生强大动力，使该赛事经久不衰。ICPC决赛选手中涌现出多位知名人士：Facebook前CTO兼Quora创始人亚当·德安杰罗、Telegram联合创始人尼古莱·杜罗夫、Apache Spark创造者马泰·扎哈里亚等。这些精英人士的共同经历正是——曾参与ICPC竞赛。

ICPC之后，编程竞赛蓬勃发展，尤其在2000年后远程参赛成为可能，使国际赛事更易举办且成本降低。多数竞赛采用相似模式：解决系列编程问题，优胜者不仅获得奖金，更能进入企业招聘视野或赢得声誉。典型赛题涵盖组合数学、数论、图论、算法博弈论、计算几何、字符串分析及数据结构等领域。近年来，随着ACM特别兴趣小组（SIG）年度会议期间举办的知识发现与数据挖掘竞赛KDD Cup的启动，人工智能相关赛题显著增加(https://kdd.org/conferences)。

1997年首届KDD Cup以直接营销中的提升曲线优化为题，开启了延续至今的系列赛事。历届数据集、任务说明与优胜方案可查阅：https://www.kdd.org/kdd-cup。本文撰写时最新赛事见：https://ogb.stanford.edu/kddcup2021/。KDD Cup在建立最佳实践方面成效显著，众多发表论文详细描述解决方案、技术细节及共享竞赛数据集，为从业者的实验研究、教学培训与基准测试提供了宝贵资源。

编程竞赛与KDD杯的成功案例激励了企业（如Netflix）和创业者（如Kaggle创始人安东尼·戈德布卢姆）创建首批数据科学竞赛平台，企业可在此发起难以解决且受益于众包的数据科学挑战。事实上，由于数据科学领域不存在放之四海皆准的黄金法则，许多问题需要采取"尝试所有可能方案"这种耗时的方法。

事实上，正如大卫·沃尔珀特和威廉·麦克雷迪提出的"没有免费的午餐"定理所言：长远来看，没有任何算法能在所有问题上始终优于其他算法。该定理表明，只有当机器学习算法的假设空间包含解决方案时，它才能发挥作用。因此，在无法预知某算法是否最适合解决特定问题的情况下，必须通过实际测试来验证。机器学习领域不存在理论捷径或万能圣杯——唯有实证才能揭示有效方案。

欲深入了解可查阅"没有免费的午餐"定理对该实践真理的理论阐释。Analytics India Magazine对此有专题文章：https://analyticsindiamag.com/what-are-the-no-free-lunch-theorems-in-data-science/。当需要大量测试算法与数据转换以寻找最佳组合却受限于人力算力时，众包便成为理想选择。这正是政府与企业通过竞赛推动特定领域发展的原因：

- 政府方面，DARPA举办的自动驾驶汽车、机器人操作、机器翻译、声纹识别、指纹识别、信息检索、OCR、自动目标识别等系列竞赛堪称典范。

- 企业方面，Netflix通过竞赛改进用户电影推荐算法的案例颇具代表性。

Netflix竞赛旨在改进协同过滤技术，仅根据用户对其他影片的评分（不涉及用户身份或影片具体信息）预测其对某部影片的潜在评分。由于所有用户描述和影片信息均被身份编码替代，参赛者需巧妙利用历史评分数据开发智能方案。百万美元大奖的授予条件是将现有Cinematch算法的预测精度提升至特定阈值以上。

这场2006-2009年举办的竞赛最终由多支团队合并夺冠：包括Kaggle赛事常胜军Commendo Research & Consulting GmbH的安德烈亚斯·特舍尔与迈克尔·贾赫尔、AT&T实验室两位研究员及雅虎两位专家。获胜方案消耗的巨大算力与多模型集成迫使团队合并资源。Netflix实际仅采纳了该方案的核心洞见来优化现有算法，而非全盘采用。详见《连线》报道：https://www.wired.com/2012/04/netflix-prize-costs/。

Netflix竞赛的核心价值并非解决方案本身（其DVD业务向流媒体转型很快使其过时），而在于参赛者获得协同过滤领域的声誉，以及企业将优化经验迁移至新业务的战略收益。

## Kaggle竞赛平台

受益于数据科学竞赛的企业远不止Netflix。虽案例众多，我们仅列举几个主办方明确获利的典型：

- 保险公司Allstate通过数百名数据科学家参与的竞赛，成功优化了精算模型(https://www.kaggle.com/c/ClaimPredictionChallenge)

- 通用电气在类似竞赛中将航班到达时间预测的行业标准性能（均方根误差指标）提升40%(https://www.kaggle.com/c/flight)

Kaggle平台迄今举办过数百场竞赛，上述仅是成功案例中的冰山一角。让我们暂时跳出具体赛事，聚焦贯穿本书的核心——Kaggle公司。

## Kaggle发展史

2010年2月，Kaggle在澳大利亚经济学家安东尼·戈德布卢姆（Anthony Goldbloom）手中诞生。这位拥有经济学与计量经济学学位的人才，曾先后就职于澳大利亚财政部和澳洲联储研究部门，后在伦敦《经济学人》周刊实习。这家国际媒体专注于时事、国际商业、政治与技术报道。在为《经济学人》撰写大数据文章时，戈德布卢姆萌生了创建竞赛平台的想法——通过众包机制汇聚顶尖分析专家，共同解决有趣的机器学习问题（https://www.smh.com.au/technology/from-bondi-to-the-big-bucks-the-28yearold-whos-making-data-science-a-sport-20111104-1myq1.html）。由于众包模式在该平台商业构想中占据核心地位，他借鉴"gaggle"（雁群）的谐音命名平台，而鹅的形象也成为平台标志。

进驻美国硅谷后，Kaggle初创公司获得由Khosla Ventures和Index Ventures两家知名风投机构领投的1125万美元A轮融资。随着首批竞赛启动，社区规模不断扩大，早期参赛者中涌现出杰出人物，如澳大利亚数据科学家兼企业家杰里米·霍华德（Jeremy Howard）。他在Kaggle赢得数场竞赛后，出任公司总裁兼首席科学家。2013年12月霍华德卸任总裁职务，创立新公司fast.ai（www.fast.ai），为程序员提供机器学习课程和深度学习库。

当时平台还活跃着其他知名"Kagglers"（指Kaggle竞赛常客），如杰里米·阿钦（Jeremy Achin）和托马斯·德戈多伊（Thomas de Godoy）。他们在跻身全球排名前20后迅速"退役"，联合创立DataRobot公司，并立即从Kaggle顶尖选手中招募员工，将最佳机器学习经验注入正在开发的软件。如今DataRobot已成为AutoML解决方案（自动化机器学习软件）开发领域的领军企业。

Kaggle竞赛吸引了日益增长的关注度。连深度学习"教父"杰弗里·辛顿（Geoffrey Hinton）也参与并赢得了2012年默克公司举办的Kaggle竞赛（https://www.kaggle.com/c/MerckActivity/overview/winners）。该平台还见证了弗朗索瓦·肖莱（François Chollet）在Otto集团产品分类挑战赛中发布深度学习框架Keras（https://www.kaggle.com/c/otto-group-product-classification-challenge/discussion/13632），以及陈天奇在希格斯玻色子机器学习挑战赛中推出梯度提升机的高效升级版XGBoost（https://www.kaggle.com/c/higgs-boson/discussion/10335）。

除开发Keras外，弗朗索瓦·肖莱在Quo-ra网站的回答中提供了关于赢得Kaggle竞赛最具实践价值的见解：https://www.quora.com/Why-has-Keras-been-so-successful-lately-at-Kaggle-competitions。

基于实证（而非理论）证据指导下的快速迭代尝试，本质上就是制胜关键。我们认为除了他答案中揭示的要点外，Kaggle竞赛并无更多获胜秘诀。

值得注意的是，弗朗索瓦·肖莱还在Kaggle上主办了被公认为全球首个通用AI竞赛的挑战赛（https://www.kaggle.com/c/abstraction-and-reasoning-challenge/）。

随着竞赛持续举办，Kaggle社区规模在2017年突破百万。同年谷歌首席科学家李飞飞在Google Next主题演讲中宣布，谷歌母公司Alphabet将收购Kaggle。此后Kaggle成为谷歌旗下平台。如今该社区依然保持活跃增长态势。安东尼·戈德布卢姆在推文（https://twitter.com/antgoldbloom/status/1400119591246852096）中指出，除参赛外，大多数用户会下载公开数据（Kaggle已成为重要数据枢纽）、创建Python/R公共笔记本，或通过平台课程学习新知识：

<!-- Media -->

<!-- figureText: 2020 2019 2018 1,931,700 1,256,908 1,000,000 1,500,000 Users Download public data 721,739 576,522 Author a notebook 401,637 281,502 328,242 Completed microcourse 219,977 118,152 295,448 Submitted to a competition 229,763 178,103 0 500,000 -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_33.jpg?x=252&y=501&w=1370&h=818&r=0"/>

图1.1：展示2020年、2019年和2018年用户使用Kaggle情况的条形图

<!-- Media -->

多年来，Kaggle为参与者提供了诸多发展机遇，例如：

- 创立个人公司

- 发布机器学习软件与工具包

- 接受杂志专访（https://www.wired.com/story/solve-these-tough-data-problems-and-watch-job-offers-roll-in/）

- 撰写机器学习书籍（https://twitter.com/antgoldbloom/status/745662719588589568）

- 找到理想工作

最重要的是，深入了解数据科学涉及的技能与技术细节。

## 其他竞赛平台

虽然本书聚焦Kaggle竞赛，但不可忽视许多数据竞赛是在私有平台或其他竞赛平台上举办的。实际上，本书中的大部分内容同样适用于其他竞赛，因为它们本质上遵循相似原则，参赛者获得的好处也大同小异。

尽管许多其他平台仅限特定国家或专攻某类竞赛，为求全面，我们将简要介绍其中部分平台（至少是我们有所了解的）：

- DrivenData（https://www.drivendata.org/competitions/）是专注社会议题的众包竞赛平台（参见https://www.drivendata.co/blog/intro-to-machine-learning-social-impact/）。这家社会企业旨在通过数据科学家构建公益算法，为应对全球重大挑战的组织提供数据科学解决方案。例如，Facebook曾选择该平台举办反仇恨言论与虚假信息建模竞赛（https://www.engadget.com/facebook-ai-hate-speech-covid-19-160037191.html）。

- Numerai（https://numer.ai/）是旧金山AI驱动的众包对冲基金，每周举办预测赛。参赛者通过对混淆数据进行预测，可赢取该公司的加密货币Numeraire作为奖励。

- CrowdANALYTIX（https://www.crowdanalytix.com/community）近期活跃度下降，但不久前仍举办过多个高难度竞赛（详见https://towardsdatascience.com/how-i-won-top-five-in-a-deep-learning-competition-753c788cade1）。其社区博客（https://www.crowdanalytix.com/jq/communityBlog/listBlog.html）可帮助了解平台挑战内容。

- Signate（https://signate.jp/competitions）是日本数据科学竞赛平台，赛事丰富且采用类似Kaggle的排名系统（https://signate.jp/users/rankings）。

- Zindi（https://zindi.africa/competitions）是非洲数据科学竞赛平台，聚焦解决非洲紧迫的社会、经济及环境问题。

- 阿里云（https://www.alibabacloud.com/campaign/tianchi-competitions）推出的天池学术竞赛与SIGKDD、IJCAI-PRICAI、CVPR等会议合作，涵盖图像3D形状检索、3D物体重建、实例分割等挑战。

- Analytics Vidhya（https://datahack.analyticsvidhya.com/）是印度最大数据科学社区，提供数据科学黑客马拉松平台。

- CodaLab（https://codalab.lri.fr/）是2013年微软与斯坦福大学联合创建的法国竞赛平台，提供名为Worksheets（https://worksheets.codalab.org/）的免费云端笔记本，支持知识共享与可复现建模。

其他小型平台包括瑞士洛桑联邦理工学院的CrowdAI（https://www.crowdai.org/）、InnoCentive（https://www.innocentive.com/）、生物医学影像平台Grand-Challenge（https://grand-challenge.org/）、DataFountain（https://www.datafountain.cn/business?lang=en-US）、OpenML（https://www.openml.org/）等。俄罗斯Open Data Science社区（https://ods.ai/competitions）持续更新主流竞赛列表，也不时涌现新平台。

您可以在mlcontests.com网站上查看正在进行的竞赛概览，以及租用GPU的当前费用。该网站经常更新，是快速了解不同平台数据科学竞赛动态的便捷途径。

Kaggle始终是最佳平台，您既能找到最有趣的竞赛，又能让自己的竞赛成果获得最广泛认可。但当发现与个人专业兴趣匹配的竞赛时，选择其他平台的挑战也是明智策略。如您所见，除了Kaggle还存在大量替代选择与机会，这意味着若同时关注更多竞赛平台，您更容易因其专业领域或数据特点而找到心仪的竞赛。

此外，由于这些挑战赛知名度较低且宣传有限，您将面临较小的竞争压力（从而可能获得更好排名甚至奖项）。但需注意，参与者间的分享交流较少，因为尚无其他竞赛平台能达到Kaggle那样丰富的分享与人脉机会。

## Kaggle平台介绍

现在我们需要更深入地探讨Kaggle的具体运作方式。后续段落将解析该平台及其竞赛的各个维度，让您体验参与Kaggle竞赛的真实感受。本书后续章节还会以更多建议和策略，对这些主题进行更详尽的探讨。

## 竞赛阶段解析

Kaggle竞赛通常分为多个阶段。通过了解每个阶段，您可以更清楚地认识数据科学竞赛的运作机制及其预期成果。

竞赛启动时，社交媒体（如Kaggle官方推特https://twitter.com/kaggle）通常会发布公告，同时竞赛页面(https://www.kaggle.com/competitions)的"活跃竞赛"栏目将新增对应标签页。点击具体竞赛标签页即可进入其专属页面，您能直观查看：该竞赛是否设置奖金（以及是否授予积分和奖章——这是参赛的附加收获）、当前参赛队伍数量以及剩余提交时间。建议首先浏览"概览"菜单，其中包含以下信息：

<!-- Media -->

<!-- figureText: Freatured Prediction Competition \$50,000 Prize Money Join Competition H&M Group is a family of brands and businesses with 53 online markets and approximately 4,850 stores. Our online store offers shoppers an extensive selection of products to browse through. But with too many choices, customers might not quickly find what interests them or what they are looking for, and ultimately, they might not make a purchase. To enhance the shopping experience, produc recommendations are key. More importantly, helping customers make the right choices also has a positive implications for sustainability, as it reduces returns, and thereby minimizes emissions from In this competition, H&M Group invites you to develop product recommendations based on data from previous transactions, as well as from customer and product meta data. The available meta data spans from simple data, such as garment type and customer age, to text data from product descriptions, to There are no preconceptions on what information that may be useful - that is for you to find out. If you want to investigate a categorical data type algorithm, or dive into NLP and image processing deep H&M Personalized Fashion Recommendations Provide product recommendations based on previous purchases H&M Group - 1,283 teams - 2 months to go (a month to go until merger deadline) Rules Overview Description Evaluation Timeline Prizes transportation. image data from garment images. learning, that is up to you. -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_37.jpg?x=252&y=222&w=1372&h=1035&r=0"/>

图1.2：Kaggle平台上的竞赛页面示例

<!-- Media -->

- 竞赛主题

- 评估指标（用于衡量模型性能）

- 竞赛时间线

- 奖项设置

- 法律条款或竞赛要求

时间线常被忽视，但应优先关注——它不仅标注起止时间，更会显示规则接受截止日（通常在竞赛结束前7-14天）。该截止日是您最后可报名参赛的期限（通过接受竞赛规则）。此外还有团队合并截止日：在此之前您可随时与其他参赛者合并团队，逾期则不可操作。

"规则"菜单也常被跳过（人们往往直奔"数据"），但其中包含关键要求：您是否具备获奖资格、能否使用外部数据提升分数、每日可提交次数以及最终可选的解决方案数量。

接受规则后，您既可从"数据"菜单下载资料，也可通过"代码"菜单直接在Kaggle Notebooks（云端笔记本）上开展工作——复用他人公开代码或从零开始编写。

若选择下载数据，Kaggle API能实现近乎自动化的下载与提交流程。对于本地或云端建模而言，这是重要工具。API详情参见https://www.kaggle.com/docs/api，代码可从GitHub获取：https://github.com/Kaggle/kaggle-api。

深入研究Kaggle的GitHub仓库，您还能找到其在线笔记本Kaggle Notebooks所用的所有Docker镜像。我们强烈建议：开发解决方案时不要闭门造车，而应通过"讨论区"与其他参赛者交流。这里不仅能获得数据问题的解决线索，更能启发优化思路。许多优秀Kaggle选手都表示，论坛中的创意既提升了比赛表现，更深化了他们对数据科学建模的理解。

<!-- Media -->

<!-- figureText: notebook477901ba02 braft saved S1. Share > - Draft Session off from a cell to start) Data + Add data Input Output - [Laggie/working Settings Language Python Environment Preferences Accelerator internal Schedule a notebook run Code Help FIND CODE HELP Q Find Code Help Search for examples of how to do things File Edit View Run Add-ons Help #This Python 3 environment comes with many helpful analytics libraries installed #It is defined by the kaggle/python Docker image: https://github.com/kaggle/docker-python import numpy as np # linear algebra import pandas as pd # data processing, CSV file I/O (e.g. pd. read_csv) #Input data files are available in the read-only "../input/" directory #For example, running this (by clicking run or pressing Shift+Enter) will list all files under the input directory for dirname, ... filenames in os.walk('/kaggle/input'): for filename in filenames: print(os.path.join(dirname, filename)) ? You can write up to 2003 to the current directory (/kaggle/working/) that gets preserved as output when you create a version using "Save & Ru : : #You can also write temporary files to /kaggle/temp/, but they won't be saved outside of the current session + Markdown -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_39.jpg?x=252&y=329&w=1392&h=556&r=0"/>

图1.3：待编写代码的Kaggle笔记本界面

<!-- Media -->

方案完成后，根据竞赛要求提交至Kaggle评估系统：部分竞赛接受CSV文件形式提交，另一些则要求通过Kaggle Notebook编写代码并生成结果。竞赛期间可多次提交解决方案。

每次提交后，排行榜会很快显示得分与排名（等待时长取决于评分计算复杂度）。该排名仅具参考价值，因为它基于公开测试集（完整测试集的一部分）的性能评估。在竞赛结束前，每位参赛者可选定若干方案（通常为两个）进行最终评审。

<!-- Media -->

<!-- figureText: \( {\mathrm{X}}_{\text{test }} \) Ypublic Yprivate Your model Public and private Kaggle Leaderboard Test \( {\mathrm{X}}_{\text{train }} \) Ytrain Train Datayou receive from Kaggle -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_40.jpg?x=439&y=354&w=1017&h=765&r=0"/>

图1.4：展示数据如何转化为公开排行榜和私有排行榜分数的示意图

<!-- Media -->

只有当竞赛结束时，基于参赛者选择被评分的模型，他们在测试集另一部分（称为私有测试集）上的分数才会揭晓。这个新的排行榜——私有排行榜构成了竞赛最终有效分数，但其排名仍非官方最终结果。实际上，Kaggle团队需要时间核查所有内容是否正确，并确认所有参赛者都遵守了竞赛规则。

经过一段时间（有时会因取消资格导致排名变动），私有排行榜将成为官方最终结果，优胜者将被公布，许多参赛者会在竞赛讨论区公开他们的策略、解决方案和代码。此时你需要自行研究其他解决方案并改进自己的方案。我们强烈建议你这样做，因为这是Kaggle上另一个重要的学习来源。

## 竞赛类型与示例

Kaggle竞赛按类别划分，每种类别在参赛方式和预期成果上都有不同含义。各类别内部的数据类型、问题难度、奖项设置和竞赛动态差异显著，因此提前了解每种类型的含义很重要。以下是用于筛选不同竞赛的官方分类：

- 精选

- 大师

- 年度

- 研究

- 招聘

- 入门

- 游乐场

- 分析

- 社区

精选竞赛是最常见的类型，涉及赞助公司提出的商业问题并为优胜者设置奖项。获胜者需向赞助公司授予其作品的非独家许可；他们必须准备详细的解决方案报告，有时还需参加与赞助公司的会议。

每次访问Kaggle都能看到精选竞赛的案例。当前许多竞赛涉及将深度学习方法应用于文本、图像、视频或声音等非结构化数据的问题。过去表格数据竞赛很常见，这类竞赛基于数据库中的结构化数据问题。最初使用随机森林，后来采用巧妙特征工程的梯度提升方法，源自Kaggle的表格数据解决方案确实能改进现有方案。如今这类竞赛已大幅减少，因为众包解决方案通常不会比优秀数据科学家团队甚至AutoML软件做得更好。随着优质软件和良好实践的普及，竞赛带来的结果质量提升确实有限。但在非结构化数据领域，优秀的深度学习解决方案仍能带来显著差异。例如BERT等预训练网络曾使许多知名NLP任务基准的原有标准提升两位数百分比。

大师赛如今较为少见，它们是仅限受邀专家参与的私人竞赛。其初衷是根据参赛者在Kaggle的排名（通常为大师或特级大师段位，基于Kaggle奖牌排名体系），打造专属高阶玩家的竞技舞台。

年度赛事是固定时段举办的常规竞赛，其中包括圣诞老人挑战赛（通常围绕算法优化命题）以及自2014年起每年伴随美国大学篮球锦标赛同步举行的三月机器学习狂热大赛。

研究型竞赛以科研而非商业为导向，部分旨在服务公共利益。因此这类赛事未必设置奖金，且有时要求优胜者将解决方案开源发布。

谷歌曾发起多项研究型竞赛，例如2020年谷歌地标识别大赛（https://www.kaggle.com/c/landmark-recognition-2020），目标是对图像中的著名（及非著名）地标进行标注。

招聘方为测试候选人能力会举办招聘竞赛。这类赛事仅限单人参赛，优胜者将获得面试机会作为奖励。参赛者若希望被联系，需在赛后提交个人简历。

典型招聘竞赛包括：

- Facebook招聘大赛（https://www.kaggle.com/c/FacebookRecruiting）；Facebook多次举办此类赛事

- Yelp招聘竞赛（https://www.kaggle.com/c/yelp-recruiting）

入门赛不设奖金，通过友好简易的题目帮助新手熟悉Kaggle规则与生态。这类半永久性竞赛会定期刷新排行榜，堪称机器学习入门首选——这里有高度协作的社区环境，更有大量Kaggle笔记教你数据处理与模型构建技巧。

经典入门赛有：

- 数字识别器（https://www.kaggle.com/c/digit-recognizer）

- 泰坦尼克号 - 灾难中的机器学习（https://www.kaggle.com/c/titanic）

- 房价预测 - 高级回归技术（https://www.kaggle.com/c/house-prices-advanced-regression-techniques）

练习赛难度略高于入门赛，同样侧重学习与能力测试（虽然后期竞争可能白热化）。奖品通常是Kaggle周边（如马克杯、T恤或袜子，参见https://www.kaggle.com/general/68961）或小额奖金。

知名练习赛包括初代猫狗大战（https://www.kaggle.com/c/dogs-vs-cats），参赛者需开发区分猫狗的算法。

另需关注：注重质性评估的分析赛（要求提交方案构思、幻灯片、图表等），以及由学术机构或Kaggle用户发起的社区赛（原班级赛）。社区赛上线公告见https://www.kaggle.com/product-feedback/294337，办赛指南可参考https://www.kaggle.com/c/about/host和https://www.kaggle.com/community-competitions-setup-guide。

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_43.jpg?x=247&y=1351&w=349&h=352&r=0"/>

<!-- Media -->

## 帕鲁尔·潘迪

https://www.kaggle.com/parulpandey

我们采访了H2O.ai的数据科学家、Kaggle Notebooks大师和数据集大师帕鲁尔·潘迪，了解她参与分析竞赛的经历及其他见解。

## 你最喜欢哪类竞赛？为什么？在技术方法和解决思路上，你在Kaggle的专长是什么？

我特别钟爱数据分析类竞赛，这类竞赛要求参赛者分析数据并最终提交全面分析报告。包括"数据科学向善"(DS4G)竞赛、体育分析竞赛（如NFL）以及常规调查挑战赛。与传统竞赛不同，这些竞赛没有排行榜来追踪你与他人的表现对比，也不会授予奖牌或积分。但另一方面，它们需要涵盖数据清洗、数据挖掘、可视化呈现和洞见传达等数据科学多维度环节的端到端解决方案。这类问题能模拟真实场景，让你展示独到见解——可能不存在唯一正确答案，但提供了权衡各种潜在方案并将其融入最终解决方案的思考空间。

## 你如何着手Kaggle竞赛？这种方式与日常工作有何不同？

我的第一步永远是作为探索性数据分析(EDA)环节来剖析数据——这也是我工作流程中的常规步骤。通常我会检查数据是否存在潜在隐患，比如不一致性、缺失值或异常值等可能引发后续问题的因素。第二步是建立可靠交叉验证策略，然后研读讨论区并参考他人分享的Notebook。这些往往能提供良好起点，之后我便可将过往经验融入当前工作流。模型性能跟踪也至关重要。

对于分析类竞赛，我喜欢将问题拆解为多个阶段：前期可能需要数天来理解问题本质，接着进行数据探索，随后创建基础解决方案框架，之后像拼乐高积木般逐步添加模块完善方案。

## 请分享你参加过最具挑战性的竞赛，以及你用来解决问题的关键洞见

如前所述，我主要参与分析类竞赛，偶尔也会尝试常规竞赛。我想特别提及一个引人入胜的"数据科学向善"竞赛——环境洞察探索者(https://www.kaggle.com/c/ds4g-environmental-insights-explorer)。该竞赛要求使用遥感技术而非传统方法计算环境排放量。

最触动我的是其现实意义。当全球正应对气候变化挑战时，这个竞赛直指问题核心。备赛过程中，卫星影像领域的发展令我惊叹，让我深入了解了Landsat、Modis和Sentinel等卫星的工作原理及数据开放机制。这是次绝佳的学习机会，让我涉足了此前陌生的领域。

# 根据你的经验，新手Kaggle用户常忽视哪些要点？你现在掌握的哪些知识希望初学时就知道？

我想列举早期在Kaggle犯过的一些错误。

首先，多数新人把Kaggle视为纯竞赛平台。虽然竞赛资源丰富，但Kaggle还为其他领域爱好者提供了代码共享、深度讨论和人际网络功能，以及优质数据集的策展与分享。我最初仅用Kaggle下载数据集，直到两年前才真正活跃起来。现在回想，这个认知偏差太大了。很多人被竞赛吓退，其实可以先熟悉平台再逐步参赛。

另一个重点是：许多人单打独斗导致失去动力而放弃。Kaggle组队有诸多隐性优势——培养团队协作能力，汲取他人经验，在限时条件下共同达成目标。

## 你是否使用其他竞赛平台？它们与Kaggle相比如何？

虽然我现在大部分时间都花在Kaggle上，但过去我曾使用过Zindi——一个专注于非洲应用场景的数据科学竞赛平台。这是获取非洲相关数据集的绝佳渠道。Kaggle作为多功能平台，却缺乏来自世界各地的多样化问题陈述。近期我们也看到一些多元化赛题，比如刚结束的chaii竞赛——一个聚焦印度语言的NLP比赛。我认为这种针对不同国家设计的竞赛，对学术研究和整个数据科学社群都大有裨益。

在Kaggle竞赛分类体系之外，还需注意竞赛可能采用不同形式。最常见的是"简单模式"：提交解决方案后按既定标准评估。更复杂的是两阶段赛制：比赛分为两部分，最终数据集仅在首阶段结束后向首阶段参赛者发布。这种设计通过采用全新测试集（仅短期开放）来降低作弊风险。与传统Kaggle竞赛不同，参赛者分析测试集规律的时间更短、提交次数更少。出于同样考量，代码竞赛应运而生——所有提交必须通过Kaggle Notebook完成，直接上传功能被禁用。

对于不同阶段的Kaggle竞赛参与者，参赛类型没有任何限制。但根据您的数据科学经验和计算资源，我们对竞赛形式和类型有以下建议：

- 纯新手可从"入门赛"或"练习赛"起步，这些低压环境能帮助熟悉Kaggle机制。但不少初学者也从"精选赛"和"研究赛"成功入门——压力反而加速了他们的学习。建议根据学习风格选择：适合探索协作型的学习者推荐入门/练习赛；需要竞争刺激来保持动力的，不妨直接挑战快节奏比赛。

- 参加精选赛和研究赛时需注意，这些竞赛常涉及AI与机器学习的前沿应用领域，因此往往需要扎实的专业基础，或愿意深入研究该应用领域的相关文献。

最后要提醒，多数竞赛所需的计算资源远超普通数据科学工作者的办公配置。若使用Kaggle之外的云平台，成本可能持续攀升。代码竞赛和限时/限资源类比赛或许是更优选择，它们致力于让所有参赛者在同等资源条件下竞争。

## 提交机制与排行榜动态

Kaggle的运作看似简单：隐藏测试集→训练模型→预测最优者胜出。但这种描述过度简化了实际复杂度，它忽略了参赛者间的直接/间接互动动态，以及赛题本身、训练集与测试集中蕴含的微妙差异。

## 解读"共同任务框架"范式

斯坦福大学统计学教授David Donoho在其论文《数据科学五十年》中，对Kaggle运作机制给出了更全面的阐释。该论文首刊于《计算与图形统计杂志》，后发布于MIT计算机\( \begin{matrix} \text{Science and Artificial} & \text{Intelligence} \\  \text{Laboratory (see http://courses.csail.mit.edu/18.337/2015/} &  \end{matrix} \) docs/50YearsDataScience.pdf)。

Donoho教授虽未特指Kaggle，而是统论所有数据科学竞赛平台。他引用计算语言学家Mark Liberman的观点，将这类竞赛归为"共同任务框架"(CTF)范式——过去数十年来，这一范式持续推动着多个领域数据科学的发展。他指出从实证角度看，CTF能显著提升数据科学问题的解决水平，并以Netflix竞赛和多项DARPA竞赛为例。CTF范式已重塑多个领域的最优解决方案。

CTF由基础要素和秘制配方构成。基础要素包括：

1. 公开数据集及相关预测任务

2. 一组共同致力于为任务提供最佳预测的竞争者

3. 用于公平客观评估参赛者预测结果的评分系统，该系统不会给出过于具体（或至少不会过度限制）的解决方案提示

当任务定义明确且数据质量优良时，该系统能发挥最佳效果。长期来看，解决方案的性能会通过微小提升逐步优化，直至趋于稳定。通过允许参与者之间适度共享（如Kaggle平台通过讨论区、共享Kaggle Notebooks以及数据集板块提供的额外数据实现的互动），可加速这一进程。根据CTF范式，竞赛中的竞争压力足以催生持续优化的解决方案。当竞争压力与参与者间的适度共享相结合时，改进速度会进一步加快——这正是Kaggle引入众多共享激励机制的原因。因为CTF范式的核心在于竞赛本身：在需要提升实证表现的现实问题框架下，竞赛总能催生新基准、新数据与建模方案，并推动机器学习技术在赛题中的优化应用。因此，竞赛能提供预测问题的新解法、特征工程的新思路，以及算法或建模的创新方案。例如深度学习不仅源于学术研究，更因验证其效能的竞赛（如Geoffrey Hinton团队获胜的默克制药竞赛：https://www.kaggle.com/c/MerckActivity/overview/winners）获得重大突破。

结合开放软件运动（使公众能使用Scikit-learn、TensorFlow、PyTorch等强大分析工具），CTF范式能产生更优结果，因为所有参赛者起点公平。但依赖专用或升级硬件的解决方案可能限制成果——这会阻碍资源不足的参赛者有效参与，无法直接贡献解决方案或通过对其他选手施加竞争压力间接推动进展。因此Kaggle开始为竞赛参与者免费提供云服务（即计算资源章节将介绍的Kaggle Notebooks），以缓解硬件密集型竞赛（如多数深度学习赛事）的硬件差异，增强整体竞争压力。

## 理解竞赛中的潜在问题

根据前文对CTF范式的描述，您可能认为只需搭建合适平台，参赛者的积极投入与赞助企业的杰出模型就会自然涌现。但现实中存在可能导致竞赛结果令人失望的隐患：

- 数据泄露

- 排行榜（评分系统）探测

- 过拟合及随之而来的排行榜震荡

- 私下共享

当数据本身隐含解决方案线索时即发生数据泄露。例如某些变量可能滞后于目标变量（如欺诈检测中使用欺诈发生后更新的变量，或销售预测中处理产品实际分销信息）。另可能是训练集与测试集存在可预测排序，或样本ID值暗示解决方案（如ID基于目标变量排序，或ID值与时间流相关而时间影响目标概率）。

这种被参赛者称为"黄金特征"的解决方案泄露（因数据细微差别可能带来大奖），必然导致方案不可复用。对赞助商而言虽能了解影响问题解决的泄露特征，但终归是次优结果。

另一个问题是从排行榜中试探解决方案的可能性。这种情况下，参赛者可以利用展示的评估指标，通过反复提交试探来窥探解决方案。同样，这类方案在其他场景中完全无法适用。"Don't Overfit II"竞赛就发生过典型案例——冠军选手Zachary Mayers将每个变量单独提交，通过获取各变量可能权重的信息来估算模型正确系数（详见其解决方案：https://www.kaggle.com/c/dont-overfit-ii/discussion/91766）。时间序列问题或测试数据存在系统性偏移的竞赛尤其容易受到试探行为影响，因为这能帮助选手定义针对特定测试集的后处理方案（如预测值乘以常数）来刷高分数。

另一种排行榜窥探形式（即获取测试集线索并对其过拟合）发生在选手过度依赖公开排行榜反馈而非自身验证时。有时这会导致竞赛彻底失控，引发最终排名剧烈震荡——冠军方案可能并非最优解，甚至纯属偶然结果。这种现象催生了分析训练集与公开测试集潜在差异的技术，这种称为对抗性测试的方法能评估对排行榜的依赖程度，并识别训练/测试集差异过大需完全规避的特征。

具体案例可参考Bojan Tunguz的笔记：https://www.kaggle.com/tunguz/adversarial-ieee。另一种防御排行榜过拟合的策略是选择安全方案，例如通常允许提交两个最终方案时，可分别选择排行榜最优解和交叉验证最优解。

为防止排行榜试探和过拟合，Kaggle近期在代码竞赛中引入分阶段评估机制——如先前所述，选手完全无法接触实际测试数据，迫使其更重视本地验证结果。

最后，竞赛还可能因私下共享（小圈子内交流方案）和多账号作弊等违规行为失真。这类信息不对称会损害多数参赛者利益，且不完善的共享机制会削弱竞争压力。若此类情况曝光（例如https://www.kaggle.com/c/ashrae-energy-prediction/discussion/122503），更会引发信任危机导致参赛热情下降。

## 计算资源

部分竞赛为保障方案可行性会设置限制，如Bosch生产线性能竞赛（https://www.kaggle.com/c/bosch-production-line-performance）对执行时间、模型文件大小和内存有严格限制。基于Notebook（原Kernel-Only）的竞赛要求训练和推理均在Kaggle环境完成，这反而消除了资源差异——Kaggle会提供统一计算资源确保公平竞争。

当竞赛仅限制推理阶段使用Notebook时，问题随之而来：选手可在本地训练模型，最终仅受测试阶段模型数量和复杂度限制。鉴于当前多数竞赛需深度学习方案，必须配备GPU等专业硬件才能保持竞争力。即便在如今少见的表格类竞赛中，要实现高效特征工程、快速实验和建模，仍需配备多处理器大内存的高性能机器。

技术标准更新迅速，因此很难明确界定一套基准硬件配置，以确保至少能与其他团队同台竞技。通过观察其他参赛者使用的设备（无论是自有机器还是云服务器），我们可以窥见当前的主流配置。

例如惠普曾推出计划，向精选的Kaggle参赛者赠送HP Z4或Z8工作站以换取品牌曝光。以Z8为例，该机型配备多达72核CPU、3TB内存、48TB存储空间（按固态硬盘标准已属可观），通常还搭载双NVIDIA RTX显卡。我们理解这对多数人而言可能遥不可及；即便在谷歌GCP或亚马逊AWS等云平台短期租用类似配置，考虑到中等使用强度下的费用，也非现实之选。

每项比赛的云服务成本自然取决于数据处理量及所建模型的数量类型。Kaggle竞赛中GCP和AWS平台提供的免费信用额度通常在200至500美元之间。

因此我们建议，当您开始攀登Kaggle排行榜时，可优先使用Kaggle免费提供的计算资源——Kaggle Notebooks（原称Kaggle Kernels）。

## Kaggle Notebooks

Kaggle Notebooks是基于云服务器Docker容器的版本化计算环境，支持使用R和Python语言编写运行脚本及笔记本。其特点包括：

- 深度集成于Kaggle生态（可直接提交结果并追溯 Notebook与提交记录的对应关系）

- 预装多数数据科学工具包

- 支持一定程度的自定义（可下载文件并安装额外软件包）

基础版仅支持CPU运算，但可选用搭载NVIDIA Tesla P100显卡或TPU v3-8加速的版本。TPU是专为深度学习任务优化的硬件加速器。

尽管受限于使用次数和时间配额，Kaggle Notebooks仍能为您提供构建竞赛基准方案所需的计算能力：

<!-- Media -->

<table><tbody><tr><td>笔记本类型</td><td>CPU核心数</td><td>内存</td><td>单次可运行的笔记本数量</td><td>每周配额</td></tr><tr><td>中央处理器</td><td>4</td><td>16 GB</td><td>10</td><td>无限制</td></tr><tr><td>图形处理器</td><td>2</td><td>13 GB</td><td>2</td><td>30小时</td></tr><tr><td>张量处理器</td><td>4</td><td>16 GB</td><td>2</td><td>30小时</td></tr></tbody></table>

<!-- Media -->

除总运行时间外，CPU和GPU笔记本每次会话最长运行12小时后会自动停止（TPU笔记本仅为9小时），这意味着除已保存至磁盘的内容外，您将无法获取该次运行的任何结果。您拥有\( {20}\mathrm{{GB}} \)的磁盘存储配额用于保存模型和结果，另有一个临时工作磁盘空间可超过20GB，供脚本运行时暂存数据使用。

某些情况下，Kaggle Notebooks提供的GPU增强型机器可能仍不足够。例如近期举办的深度伪造检测挑战赛(https://www.kaggle.com/c/deepfake-detection-challenge)需要处理约\( {500}\mathrm{{GB}} \)视频数据。这尤其具有挑战性，因为每周使用时限为30小时，且同时运行的GPU机器不得超过两台。即使您能通过修改代码转而利用TPU（此处可获得简易实现指南：https://www.kaggle.com/docs/tpu）将机器时间翻倍，对于深度伪造检测挑战赛这类数据密集型竞赛的快速实验而言，这可能仍显不足。

因此，在第三章《Kaggle Notebooks工作与学习指南》中，我们将提供应对这些限制的技巧，助您在不购置高性能机器的情况下产出优质成果。我们还将演示如何将Kaggle Notebooks与GCP集成，或在第二章《数据集管理》中指导您将所有工作迁移至另一云端解决方案——Google Colab。

## 组队与社交网络

虽然计算能力至关重要，但唯有专业知识和人类智慧才能真正决定Kaggle竞赛的胜负。要成功应对竞赛，有时需要参赛者组成团队协作。除招聘类竞赛（主办方可能要求个人参赛以更好评估能力）外，通常不限制组队。团队最多可由五人组成，其优势在于能凝聚多方智慧寻找更优解——团队成员可投入更多共同时间，且不同技能组合能发挥巨大作用；毕竟并非所有数据科学家都具备相同的模型构建与数据处理能力。

但组队并非全无弊端。协调不同成员朝共同目标努力可能并非易事，且可能出现次优状况。常见问题包括部分成员参与度不足或消极怠工，但最恶劣的莫过于有人违反竞赛规则——这将连累整个团队被取消资格——或如前述为其他团队窃取情报。

尽管存在风险，Kaggle组队仍是深入了解同行、实现目标协作、获取更大收益的良机，因为平台规则确实更优待团队。事实上，较小团队获得的奖金份额会高于均分比例。不过组队并非Kaggle社交的唯一途径，论坛讨论、竞赛期间共享数据集和Notebook等平台互动，都能助您建立行业人脉并获得认可。

在Kaggle平台之外也有许多社交机会。例如2016年创建的Slack频道KaggleNoobs(https://www.kaggle.com/getting-started/20577)，汇集了大量竞赛相关讨论，其互助社区能为代码或模型问题提供支持。

还有不少其他频道专门用于交流关于Kaggle竞赛和数据科学相关话题的观点。部分频道按地区或国家组织，例如日本频道Kaggler-ja（http://kaggler-ja-wiki.herokuapp.com/）或2015年创立的俄罗斯社区开放数据科学网络（https://ods.ai/），后者后来也向非俄语参与者开放。该网络不仅提供Slack频道，还开设了竞赛获胜课程、活动报道，并涵盖所有知名数据科学平台的实时竞赛动态（参见https://ods.ai/competitions）。除Slack频道外，各地涌现了许多围绕Kaggle或特定竞赛主题的线下聚会，有些是临时组织，有些则形成固定模式。这类聚会通常以参赛者分享经验或建议的演讲为核心，是面对面结识其他Kaggle用户、交流观点以及组建数据科学竞赛联盟的最佳途径。

在此领域中，必须提及由Maria Parysz和Pawel Jankiewicz创立的Kaggle Days（https://kaggledays.com/）。该组织曾在全球主要城市举办多场活动（https://kaggledays.com/about-us/），旨在集结Kaggle专家召开会议，并在各国建立了至今仍活跃的地方聚会网络（https://kaggledays.com/meetups/）。

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_54.jpg?x=242&y=896&w=356&h=353&r=0"/>

<!-- Media -->

## 帕维尔·扬凯维奇

https://www.kaggle.com/paweljankiewicz

我们有机会采访了帕维尔关于他参与Kaggle竞赛的经历。他是竞赛特级大师，也是LogicAI的联合创始人。

## 您最青睐哪类竞赛？为什么？在技术方法和解决策略方面，您在Kaggle上的专长是什么？

代码类竞赛是我的最爱，因为在受限环境中工作会迫使你统筹考虑时间、CPU、内存等各类资源预算。过去我常需要动用3-4台高性能虚拟机才能取胜，这种资源不对等的竞赛模式令我反感。

## 您如何着手应对Kaggle竞赛？这与日常工作有何不同？

我的参赛策略因赛而异，但总会为每场竞赛构建一个能快速生成大量实验的框架。例如在某次需要构建深度卷积神经网络的竞赛中，我设计出通过"C4-MP4-C3-MP3"格式（每个字母代表不同网络层）配置神经网络的方法。虽然现在可能直接选用骨干模型即可，但快速修改流程关键环节的框架构建原则依然适用。

日常工作与Kaggle竞赛在建模方法和验证流程上有相通之处。竞赛让我深刻认识到防止数据泄露等验证工作的重要性——既然顶级专家准备的竞赛都会频现数据泄露，那么生产环境中80%以上的模型训练可能都存在验证缺陷（此观点仅供参考）。

另一关键区别在于：日常工作不会有人明确指导如何定义建模问题。例如：

1. 应该选用RMSE、RMSLE、SMAPE还是MAPE作为评估指标？

2. 对于时间序列问题，如何拆分数据才能最真实地评估模型？

这些决策不仅关乎业务效果，还需要清晰阐释其合理性。

## 请分享一场令您印象深刻的挑战性竞赛，以及您破局的关键洞察。

最具挑战性和趣味性的是Mercari价格预测代码竞赛。它与其他任何竞赛都截然不同，因为计算时间限制在1小时内，且仅允许使用4核CPU和\( {16GB} \)内存。突破这些限制正是挑战最激动人心的部分。我从这次竞赛中获得的最大启示是要更信任表格数据的神经网络处理能力。在与队友Konstantin Lopukhin(https://www.kaggle.com/lopuhin)合并方案前，我准备了包括神经网络在内的多个复杂模型以及其他提升算法。合并后发现Konstantin仅使用了一种高度优化的架构（包括训练轮次和学习率）。该竞赛另一个独特之处在于，简单平均团队成员的解决方案远远不够，我们必须重构工作流程以形成统一协调的方案而非临时拼凑的结果，最终花费三周时间完成了方案整合。

## 根据你的经验，新手Kaggle玩家常忽视哪些要点？你现在掌握的哪些知识希望初学时就知道？

软件工程技能可能被严重低估。每个竞赛和问题都存在差异，需要特定框架来优化解决方案（参考https://github.com/bestfitting/instance_level_recognition中出色的代码组织）。良好的代码架构能加速迭代，最终尝试更多可能性。

# 参加竞赛时最需要牢记或做到的关键事项是什么？

最重要的是享受过程。

## 绩效等级与排名体系

除奖金和实体奖品（如奖杯、T恤、连帽衫和贴纸）外，Kaggle还提供诸多非物质奖励。参赛者投入大量时间精力（更不用说培养那些在普通人群中相当稀缺的竞赛技能），但通常只有顶尖选手能获得与付出匹配的奖金回报，多数人自愿付出的惊人时间几乎得不到物质回报。长期参与却无实质收获可能导致热情消退，降低竞争烈度。

因此Kaggle建立了基于勋章和积分的荣誉体系：勋章和积分越多，代表技能越受认可，能为求职或其他声誉相关的活动创造机会。

首先是综合排行榜（https://www.kaggle.com/rankings），整合了所有独立竞赛的排名。根据单次竞赛名次获得的积分总和决定综合排名。竞赛积分计算公式初看略显复杂：

\[\left\lbrack  \frac{100000}{\sqrt{{N}_{\text{teammates }}}}\right\rbrack   * \left\lbrack  {\operatorname{Ran}{k}^{-{0.75}}}\right\rbrack   * \left\lbrack  {{\log }_{10}\left( {1 + {\log }_{10}\left( {N}_{\text{teams }}\right) }\right) }\right\rbrack   * \left\lbrack  {e}^{-t/{500}}\right\rbrack  \]

但实际上只需考虑几个要素：

- 竞赛名次

- 团队规模

- 竞赛热度

- 竞赛历史时长

直观而言，热门竞赛的高排名带来大量积分。不太直观的是团队规模以非线性方式影响积分——由于公式中的平方根反比关系，随着人数增加需放弃的积分比例会增大。但较小团队（2-3人）仍具优势，因协作能带来智力与算力的加成。

另需注意积分随时间衰减。衰减并非线性，但经验而言一年后所得积分所剩无几。因此除非持续参赛并保持以往成绩，否则Kaggle综合排行榜的荣耀转瞬即逝。值得安慰的是个人资料会永久保留你达到过的最高排名。

更为持久的是涵盖Kaggle竞赛四大领域的奖章体系。根据成绩表现，您将在竞赛、笔记本、讨论和数据集四个维度获得奖章。竞赛奖章依据排行榜名次颁发，其余三个领域则基于其他参赛者的点赞数（这可能引发某些非最优情况，因为点赞是较主观的指标且受流行度影响）。累积奖章数量将决定您在Kaggle的等级晋升，依次为新手、贡献者、专家、大师和宗师。官网https://www.kaggle.com/progression详细说明了奖章获取方式及各等级所需的奖章类型与数量。

请注意这些等级和荣誉具有相对性且会随时间调整。事实上几年前评分体系和等级划分就大不相同。未来很可能再次调整，以确保高级别称号的稀缺性与价值。

## 争议与机遇

自创立以来，Kaggle一直饱受争议。参与数据科学竞赛至今仍是众说纷纭的话题，褒贬之声兼而有之。

负面评价主要集中于：

- Kaggle扭曲了机器学习的本质认知，因其仅关注排行榜动态

- Kaggle不过是场超参数优化游戏，通过堆叠模型勉强提升精度（实则是对测试集的过拟合）

- Kaggle充斥着缺乏经验的狂热者，他们为博取分数和关注度不择手段，以期获得招聘方青睐

- 更糟的是，竞赛方案往往过于复杂且针对特定测试集定制，难以落地实施。许多批评者认为Kaggle与其他数据科学竞赛平台一样，与现实中的数据科学相去甚远。关键争议在于：商业问题不会凭空出现，您很少能直接获得现成数据集——通常需要根据业务需求细化与问题理解逐步构建。此外，批评者强调Kaggle参赛者并未掌握构建生产级模型的技能，因为获胜方案不受资源限制或技术债务考量约束（尽管并非所有竞赛皆如此）。

这些批评最终都指向雇主如何看待Kaggle排名与其他经验（尤其是正规数据科学教育及工作经验）的对比。一个根深蒂固的误解是：Kaggle竞赛无助于获得数据科学工作或职业晋升，参与者也并未比非参赛数据科学家更具优势。

我们的立场是：认为Kaggle排名仅限社区内部价值的观点具有误导性。例如求职时，Kaggle能培养您数据建模、问题构建及模型验证的关键能力，还能拓展技术视野与业务场景认知。但它无法提供成为企业数据科学家所需的全部技能。

您可将Kaggle用于学习（官网设有专项课程）和提升求职竞争力，但企业认可度差异显著。无论如何，Kaggle培养的技能将在职业生涯中持续发挥作用，特别是在处理非常规数据建模难题时。参赛经历能强化建模验证能力，同时拓展数据科学家社交网络——这既便于获得工作推荐，也能通过他人智慧解决超纲难题。

因此我们认为，Kaggle对数据科学职业发展的助益更多是间接多元的。虽然竞赛佳绩可能带来直接工作邀约，但更常见的是培养您作为从业者所需的核心能力。经过Kaggle实战洗礼，当面对现实中的类似问题时，您将能快速高效地找到解决方案——因为那些在时限压力下处理多样化数据集与问题的经历，已成为您的思维本能。

正是这种技能提升的可能性，成为我们最初撰写本书的动机，也是本书的核心内容。你不会在这里找到纯粹关于如何赢得Kaggle比赛或获取高分的指南，但一定能发现如何更高效参与Kaggle竞赛，以及如何从竞赛经历中汲取最大价值的实战手册。

明智运用Kaggle等竞赛平台。Kaggle并非万能钥匙——竞赛夺冠并不能保证你获得高薪工作或超越Kaggle社区的声誉。但持续参与竞赛是张聪明牌，既能展示你对数据科学职位的热忱，又能提升特定技能，使你在AutoML解决方案面前保持竞争力，成为不可替代的数据科学家。

跟随本书的指引，我们将为你揭示实现路径。

## 本章小结

开篇章节中，我们首先探讨了数据科学竞赛平台的兴起机制及其运作模式——既涉及参赛者视角，也涵盖主办机构层面，特别援引了David Donoho教授提出的具有说服力的CTF范式。

我们解析了Kaggle的运作机制，同时不忘提及其他重要竞赛平台，说明挑战Kaggle之外的赛事同样有益。针对Kaggle，我们详细阐述了竞赛各阶段流程、赛事间的差异特征，以及该平台能提供的资源支持。

接下来几章，我们将从数据集操作指南开始，更深入地探索Kaggle世界。

## 加入本书Discord社区

欢迎加入本书Discord工作区，每月参与作者问答专场：

https://packt.link/KaggleDiscord

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_61.jpg?x=231&y=310&w=185&h=234&r=0"/>

<!-- Media -->

## 用数据集组织数据

阿瑟·柯南·道尔在《铜山毛榉案》中让福尔摩斯高喊："数据！数据！数据！没有黏土我做不出砖块。"这种成就文学史上最著名侦探的思维方式，每位数据科学家都应效仿。因此我们以数据专题开启本书技术篇章——具体而言，在Kaggle语境下，如何利用Kaggle数据集功能达成目标。

本章将涵盖以下主题：

- 数据集创建

- 数据收集

- 数据集操作

- 在Google Colab中使用Kaggle数据集

- 法律声明

## 创建数据集

原则上，任何可使用的数据均可上传至Kaggle（需遵守限制条款，详见后文法律声明部分）。截至本文撰写时，单个私有数据集上限为100GB，总存储配额为100GB。请注意单个数据集的大小限制按未压缩状态计算；上传压缩版本可加速传输但无法突破容量限制。最新数据集文档请访问：https://www.kaggle.com/docs/datasets。Kaggle自诩为"数据科学之家"，其海量数据集收藏确实佐证了这一说法。从油价数据到动漫推荐主题应有尽有，更令人惊叹的是数据更新速度——2021年5月根据《信息自由法》公布的安东尼·福奇邮件（https://www.washingtonpost.com/politics/interactive/2021/tony-fauci-emails/），仅48小时后就被作为Kaggle数据集上传。

<!-- Media -->

<!-- figureText: // Trending Datasets See All Deforestation and Forest Bitcoin Price \( \vdots \) Loss \( \underline{\text{ ELoo - Updated 9 hours ago}} \) Chiticariu Cristian -Updated 7 hours ago Usability \( {10.0} \cdot  {271}\mathrm{{KB}} \) Usability 7.1 - 4 KB 1 Task - 1 File (CSV) 1 File (CSV) (-1) - 7 See All Stroke Prediction Dataset Reddit Vaccine Myths \( \vdots \) fedescriang. Updated 3 months ago \( \underline{\text{ Gabriel Preda }} \cdot \) Updated a day ago Usability \( {10.0} \cdot  {67}\mathrm{{KB}} \) Usability 10.0 -227 KB Python Course Discussion Largest Cities in the World JSON Rishi Damarla - Updated 3 hours ago Bruno Ferreira - Updated 2 hours ago Usability 9.4 -12 MB Usability \( {10.0} \cdot  {80}\mathrm{{KB}} \) 1 File (other) 1 File (JSON) (-1) Popular Datasets Heart Attack Analysis & \( \vdots \) World Happiness Report \( \vdots \) Prediction Dataset 2021 Rashik Rahman - Updated a month ago Ajaypal Singh - Updated a month ago 1 Task - 2 Files (CSV) 1 Task - 2 Files (CSV) -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_62.jpg?x=242&y=553&w=1396&h=849&r=0"/>

图2.1：Kaggle热门趋势数据集

<!-- Media -->

将项目数据上传为数据集前，请务必检查现有内容。对于图像分类、自然语言处理、金融时间序列等热门应用领域，很可能已有现成数据。

为便于演示，我们假设项目所需数据尚未存在，需创建新数据集。点击左侧三线菜单选择"Data"后，将跳转至数据集页面：

<!-- Media -->

<!-- figureText: Datasets Data Visualization Explore, analyze, and share quality data. Learn more about data types, creating, and collaborating. + New Dataset Your Work Q Search datasets Datasets Tasks Computer Science Education Classification Computer Vision -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_63.jpg?x=259&y=231&w=1290&h=393&r=0"/>

## 图2.2：数据集页面

<!-- Media -->

点击"新建数据集"后需填写基本信息：上传数据文件并命名。左侧图标代表不同数据来源渠道，按页面显示顺序说明如下：

<!-- Media -->

<!-- figureText: 团 Enter Dataset Title 团 Drag and drop files to upload Consider zipping large directories for faster uploads or Browse Files Private Create G www.kaggle.com/konradb/ 。 -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_63.jpg?x=306&y=885&w=1296&h=860&r=0"/>

图2.3：填写数据集详情

<!-- Media -->

- 从本地驱动器上传文件（如图所示）

- 通过远程URL创建

- 导入GitHub仓库

- 使用现有Notebook的输出文件

- 导入Google云存储文件

关于GitHub选项的重要说明：该功能对实验性库特别实用。这些库虽常提供突破性功能，但通常未预装在Kaggle环境中。若需在代码中使用此类库，可参照以下方式将其作为数据集导入：

1. 进入数据集页面，点击"新建数据集"

2. 选择GitHub图标。

3. 输入仓库链接，并为数据集填写标题。

4. 点击右下角的创建按钮：

<!-- Media -->

<!-- figureText: efnet_pytorch 2 Private Create www.kaggle.com/konradb/efnet-pytorch Import GitHub repository Create a dataset from a GitHub repository archive. Use the repo URL or any deep link. GitHub URL https://github.com/lukemelas/EfficientNet-PyTorch Preview .github workflows J main.yml (463 B) .gitignore (1.44 KB) LICENSE (11.09 KB) -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_64.jpg?x=347&y=1153&w=1317&h=864&r=0"/>

图2.4：来自GitHub仓库的数据集

<!-- Media -->

创建按钮旁有个标记为私有的选项。默认情况下，所有新建数据集均为私有：仅创建者本人可查看和编辑。建议在创建阶段保持默认设置，待后期再决定是否公开（向特定贡献者或所有人开放）。

请注意Kaggle是热门平台，许多人会上传数据集（包括私有数据集），因此请尽量起个独特的标题。这将增加您数据集被关注的机会。

完成所有步骤并点击创建后，大功告成！您的首个数据集已就绪。接下来可前往数据标签页：

<!-- Media -->

易于理解 ✓ 包含丰富的机器可读文件格式 ✓ 确保数据集维护基本元数据 ✓ 注明来源 ✓ 添加副标题 ○ 补充文件信息 通过文件描述帮助他人使用 ✓ 设定更新频率 ✓ 添加标签 ○ 发布记事本 ✓ 添加描述 - 包含列描述符 提供数据应用示例 ○ 上传图片 通过特征描述帮助他人理解 ✓ 添加任务 指定许可证 建议用户可做的分析 使用优选文件格式

图2.5：数据标签页

<!-- Media -->

上图展示了可提供的各类数据集信息；提供的信息越完善，可用性指数越高。该指数是衡量数据集描述完整性的综合指标。可用性指数高的数据集在搜索结果中排名更靠前。评估指标包括文档完整度、关联公共内容（如参考记事本）的可用性、文件类型及关键元数据覆盖度等。

原则上无需填写图中所有字段（新建数据集不加这些信息仍完全可用，若是私有数据集更无需在意——毕竟您清楚内容）。但社区礼仪建议完善公开数据集的信息：描述越详尽，数据对他人越有用。

## 数据收集

除法律限制外，数据集内容类型基本不受限：表格数据、图像、文本等只要符合大小要求均可存储。这包括从其他来源获取的数据，例如按标签或话题收集的推文——这类数据集在本书撰写时颇为流行：

<!-- Media -->

<!-- figureText: tweets — Filters NLP Data Visualization See All Analyzing the influence of the Perform Sentiment Analysis on twitter chat over Bitcoin price ... the US Election Candidates laetitia hoquetis - 4 Submissions Manch Hui \( \cdot  2 \) Submissions Bitcoin tweets - 16M t... US Election 2020 Twe... \( \underline{\text{ Alex }} \cdot \) Usability 9.7 Manch Hui - Usability 10.0 Most Votes 1085 747 #Gold ... 667 Datasets Tasks Computer Science Education Classification Computer Vision ☑ 71 Tasks Are the tweets are really Detection of depressing tweets effective? Baba Bulls Eye · 0 Submissions Mustafa Dogan- 5 Submissions Tweets about theTop... Depression Analysis Omer Metin - Usability 10.0 Baba Bulls Eye - Usability 3.5 ☑ 695 Datasets Sentiment140 dataset with 1.6 million tweets Maptoc Mcχαηλιδη¢ KazAnova • Updated 4 years ago Usability 8.8 -1 File (CSV) - 81 MB -1 Task Twitter US Airline Sentiment Figure Eight Updated 2 years ago Usability 8.2 - 2 Files (SQLITE, CSV) - 3 MB News Headlines Dataset For Sarcasm Detection \( \underline{\text{ Rishabh Misra }} \cdot \) Updated 2 years ago Usability 10.0 - 2 Files (JSON) - 3 MB - 1 Task -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_66.jpg?x=236&y=530&w=1411&h=991&r=0"/>

图2.6：推文是最受欢迎的数据集之一

<!-- Media -->

关于从社交媒体（Twitter、Reddit等）采集数据的不同框架的讨论不在本书范围内。

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_67.jpg?x=246&y=229&w=352&h=358&r=0"/>

<!-- Media -->

## 安德鲁·马兰昂

https://www.kaggle.com/andrewmvd

我们采访了数据集大师（撰写本文时在Kaggle数据集领域排名第一）、圣保罗阿尔伯特·爱因斯坦医院高级数据科学家安德鲁·马兰昂（又名Larxel），探讨了他如何取得数据集竞赛的成功、创建数据集的技巧以及他在Kaggle的总体经历。

你最喜欢哪种类型的竞赛？为什么？在技术方法和解决途径方面，你在Kaggle上的专长是什么？

医学影像通常是我的最爱，这与我工作的初衷相符。在医学类竞赛中，自然语言处理受语言限制，表格数据在各医院间差异很大，但影像数据基本通用，因此这方面的任何进展都能为全球多国带来益处——我钟爱这种潜在影响力。我也喜欢自然语言处理和表格数据，不过这些领域比较常规。

请分享一个你参与过的特别具有挑战性的竞赛，以及你用来解决该任务的洞见。

在一次X光影像结核病检测竞赛中，我们仅有约1000张影像，这对于捕捉疾病所有表现形态远远不够。我提出两个解决思路：

1. 使用肺炎检测外部数据（约2万张影像）进行预训练，因为肺炎可能与结核病混淆

2. 通过肺部异常多标签分类数据（约60万张影像）预训练，并配合grad-CAM与简单SSD生成分类标签的边界框标注

最终，这两种方法的简单融合使结果比第二名团队高出22%。这场有约100支队伍参与的竞赛是在医学会议上举办的。

# 你已成为数据集大师并在该领域排名第一。你是如何选择主题，并寻找、收集和发布Kaggle数据集的？

这是个宏大的问题，我试着拆解回答：1. 确立目标

选择主题时，我首先考虑的是做这件事的初衷。

当存在深层动机时，优秀数据集会自然产生而非成为刻意目标。创建ImageNet的实验室负责人李飞飞在TED演讲中透露，她希望构建一个机器能像她孩子那样通过视觉理解世界的未来。

心怀目标能让你持续投入并进步，同时使你与你的数据集独具特色。当然你可以专注于日常主题的表格数据，但我认为这难以产生持久影响。

### 2.优质数据集是伟大问题的具象化

纵观当前文献中的顶级数据集，如ImageNet等，我们可以发现一些共同特征：

- 这是一个大胆且相关的问题，具有重大科学或现实应用潜力

- 数据经过精心采集、质量控制和完善记录

- 数据量和多样性适应当前硬件条件

- 拥有活跃的社区持续优化数据并深化问题研究

如前所述，我认为提问是数据科学家的核心职责，随着机器学习和深度学习解决方案的自动化发展，这一职能将愈发重要。这正是数据集能彰显你独特技能之处。

## 3.构建成功流程，而非仅为成功而成功

质量远胜数量；成为顶尖专家只需15个数据集，而AI领域的标杆数据集本就稀少且精良。

我废弃的数据集与公开发表的一样多。这需要时间投入，绝非许多人以为的一蹴而就——数据集需要持续维护与改进。

最常被忽视的是对数据用户社区的支持。笔记本与数据集是共同成果，支持那些认真分析你数据的人也会反哺数据集发展。分析他们的瓶颈与选择能指引预处理步骤优化，并完善文档清晰度。

总之，我推荐的流程是：确立目标→分解为具体主题→构建问题→调研数据源→筛选收集→预处理→文档记录→发布→维护支持→持续改进。

例如想提升社会福利，可分解出"种族平等"目标，分析相关主题后聚焦"黑人的命也是命"运动，进而形成问题：如何理解数百万条相关讨论？

这将数据类型限定为NLP领域，可从新闻、YouTube评论和推文（选择更具代表性和可行性的）收集数据。预处理时去除标识符，并详细记录采集流程与数据集用途。

发布后，一些Kaggle用户尝试主题建模但受多语言推文的编码问题困扰。你通过建议和支持帮助他们，并决定回溯数据仅保留英文推文以彻底解决问题。

他们的分析揭示了运动相关的诉求、动机与忧虑。通过这些努力，数百万推文最终被提炼成可能促进社会种族平等的建议方案。

## 4. 做好分内之事是唯一可控的因素

最终将你推上大师之位的是他人，而票数并不总能反映付出或影响力。在我关于《赛博朋克2077》的数据集中，我投入了约40小时的工作量，但至今仍是获赞最少的数据集之一。

但这无关紧要。我尽力尝试并汲取了所能学到的——这才是我能掌控的，下周我仍会继续如此。全力以赴，持之以恒。

## 在数据分析/机器学习领域，您会推荐哪些特定工具或库？

有趣的是，我对工具库既推荐也不推荐。LightGBM是出色的表格机器学习库，性能与计算时间比极佳；CatBoost有时表现更优，但需以增加计算时间为代价——这些时间本可用于构思和测试新想法。Optuna适合超参数调优，Streamlit用于前端，Gradio适合最小可行产品，FastAPI用于微服务，Plotly和Plotly Express制作图表，PyTorch及其衍生库适用于深度学习。

尽管工具库很棒，但我建议在职业生涯某个阶段亲自实现算法。这个建议最初来自吴恩达(Andrew Ng)，后来许多同级别专家也反复强调。通过实践能获得深刻认知，从而全新理解模型运作机制及其对调参、数据、噪声等因素的响应。

根据您的经验，新手Kaggle选手常忽视哪些要点？您现在希望初入行时就了解哪些知识？

这些年来，我最希望早日领悟的是：

1. 赛后充分吸收知识养分

2. 复现已结束比赛的获胜方案

临近比赛截止时，排行榜的激烈波动会让人难以冒险深入钻研细节。而赛后没有时间压力，你可以从容复盘，还能借鉴公开的冠军解决方案逻辑。

若有足够自律，这种方法能显著提升数据科学技能。关键在于：在完成学习时停止，而非比赛结束时。吴恩达在主题演讲中也建议通过复现论文来提升AI实践能力。当然赛后疲惫想休息也正常，但请记住：赛后讨论区是地球上知识密度最高的地方之一，因为大量获胜方案的逻辑和代码在此公开。务必花时间研读冠军方案，别因急于转向新项目而错过绝佳学习机会。

## Kaggle对您的职业发展有帮助吗？具体体现在哪些方面？

Kaggle通过提供丰富知识、实战经验及作品集积累助推了我的职业发展。我的首份数据科学家工作主要得益于Kaggle和DrivenData竞赛经历。整个职业生涯中，我持续研究竞赛方案并参与更多赛事。在数据集和笔记本板块的深入互动，也对学习新技术和提出更优质问题大有裨益。

我认为提出优质问题是数据科学家面临的核心挑战。解决问题固然重要，但随着自动化建模方案日益普及，这方面工作未来可能会被简化。而提出好问题则难以自动化——若问题本身不佳，再完美的解决方案也毫无意义。

## 您是否曾将Kaggle竞赛成果纳入作品集向潜在雇主展示？

确实如此。2017年我凭借Kaggle作为能力证明，获得了第一份数据科学家工作。时至今日，它依然是简历中极具分量的组成部分——相较于学历背景，项目作品集更能体现数据科学的知识储备与实践经验。

包含竞赛项目的作品集不仅佐证额外经验，更彰显主动追求进阶发展的意愿，这种特质对长期成功或许更为关键。

## 您是否使用其他竞赛平台？它们与Kaggle相比如何？

我也使用DrivenData和AICrowd。它们的优势在于能让初创企业、研究机构等资金资源有限的机构发起竞赛。

优质竞赛源于优质命题与优质数据的结合，这与企业规模无关。Kaggle拥有更庞大活跃的社区，其提供的硬件设施结合数据与Notebook功能使其成为最优选；但DrivenData和AICrowd同样能带来引人入胜的挑战，促进多样性发展。

## 参加竞赛时最需要牢记或做到的关键事项是什么？

若以能力提升为主要目标，建议选择感兴趣领域且未尝试过的竞赛任务。批判性思维与专业能力需要深度与广度的结合。专注发挥最佳水平能保证深度，而尝试未涉足领域或采用新方法则可拓展广度。

## 数据集应用

创建数据集后，通常需要将其用于分析。本节将探讨不同的应用方法。

最重要的步骤很可能是创建以该数据集为主要数据源的Notebook。操作方式为：进入数据集页面后点击"新建Notebook"：

<!-- Media -->

<!-- figureText: ☑ Dataset Download (5 MB) New Notebook Usability 4.1 Explosive Violence Monitoring Project Recorded casualty data from explosive violence from English-language media Konrad Banachewicz \( \cdot \) updated 18 days ago (Version 1) Data Tasks Code Discussion Activity Metadata Settings Make your dataset easy to use -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_72.jpg?x=249&y=946&w=1387&h=396&r=0"/>

图2.7：从数据集页面创建Notebook

<!-- Media -->

操作完成后将跳转至Notebook页面：

<!-- Media -->

<!-- figureText: notebook27227176cf Share (C) Save Version Data Add data Input Output ☐ /kaggle/working Settings Language Environment Preferences Schedule a notebook run Schedule this notebook to run and save a new version on a future date. View all your scheduled notebooks. File Edit View Run Add-ons Help + 3 K W D D D RunAs Code - #This Python 3 environment comes with many helpful analytics libraries installed #It is defined by the kaggle/python Docker image: https://github.com/kaggle/docker-python #For example, here's several helpful packages to load import numpy as np # linear algebra import pandas as \( \mathrm{{pd}} \) # data processing, CSV file I/O (e.g. pd. read_csv) #For example, running this (by clicking run or pressing Shift-Enter) will list all files under the input directory import os for dirname, _, filenames in os.walk('/kaggle/input'): for filename in filenames: print(os.path.join(dirname, filename)) #You can write up to 2008 to the current directory (/koggle/working/) that gets preserved as output when you create a variety #You can also write temporary files to /kaggle/temp), but they won’t be saved outside of the current session + Code + Markdown -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_72.jpg?x=245&y=1510&w=1399&h=538&r=0"/>

图2.8：使用您的数据集启动Notebook

<!-- Media -->

注意事项如下：

- 系统自动生成字母数字标题，点击可编辑

- 右侧"数据"栏显示Notebook关联的数据源列表，所选数据集可通过../input/或/kaggle/input/路径访问

- 初始代码块（包含导入的包、描述性注释及可用文件列表的打印）会自动添加到新的Python Notebook中。

完成基础设置后，您即可开始编写分析用的Notebook，并将数据集作为数据源使用。我们将在第四章《善用讨论论坛》中更详细探讨Notebook的使用。

## 在Google Colab中使用Kaggle数据集

Kaggle Notebooks虽可免费使用，但存在限制（详见第四章说明），您首先可能遇到的就是运行时限制。常见解决方案是转用Google Colab——这个完全基于云端的免费Jupyter Notebook环境：https://colab.research.google.com。

即便将计算任务迁移至此，我们仍可能需要访问Kaggle数据集，因此将其导入Colab的功能非常实用。本节剩余部分将介绍通过Colab使用Kaggle数据集所需的步骤。

首先（假设已完成Kaggle注册），我们需要前往账户页面生成API令牌（包含登录会话安全凭证、用户身份识别信息、权限等内容的访问令牌）：

1. 访问您的账户页面（https://www.kaggle.com/USERNAME/account），点击"创建新API令牌"：

<!-- Media -->

API

通过Kaggle测试版API，您可通过命令行与竞赛和数据集交互，实现数据下载、提交结果等操作。查阅文档 创建新API令牌 使API令牌失效

图2.9：创建新API令牌

<!-- Media -->

系统将生成名为kaggle.json的文件，内含您的用户名和令牌。

2. 下一步是在Google Drive创建名为Kaggle的文件夹，并上传.json文件：

<!-- Media -->

<!-- figureText: Drive Search in Drive See files \( \times \) Owner File size me May 9, 2021 me 63 bytes New My Drive \( > \) Kaggle- My Drive On September 13, 2021, a security update will be applied to some of your files. Learn more Computers Shared with me kaggle.json Recent Starred Trash Storage 28.81 GB of 201 GB used Buy storage -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_74.jpg?x=344&y=336&w=1301&h=542&r=0"/>

图2.10：将.json文件上传至Google Drive

<!-- Media -->

3. 完成后，需新建Colab notebook并通过运行以下代码挂载云端硬盘：

---

from google.colab import drive

drive.mount('/content/gdrive')

---

4. 从URL提示获取授权码，将其填入弹出的空白框，随后执行以下代码配置.json文件路径：

---

import os

#content/gdrive/My Drive/Kaggle 是存放 kaggle.json 文件的路径

#存在于谷歌云端硬盘中

os.environ['KAGGLE_CONFIG_DIR'] = "/content/gdrive/My Drive/Kaggle"

#更改工作目录

%cd /content/gdrive/My Drive/Kaggle

#使用 pwd 命令检查当前工作目录

---

5. 现在可以下载数据集。首先访问Kaggle上的数据集页面，点击"新建笔记本"旁的三个点，选择"复制API命令"：

<!-- Media -->

<!-- figureText: 336 Download (155 KB) New Notebook \( \vdots \) D Copy API command Tags health, religion and belief sys Social share... beginner, healthcare Report issue... Bookmark -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_75.jpg?x=411&y=211&w=1171&h=706&r=0"/>

图2.11：复制API命令

<!-- Media -->

6. 运行API命令下载数据集（想了解命令详情的读者可查阅官方文档：https://www.kaggle.com/docs/api）：

---

!kaggle datasets download -d ajaypalsinghlo/world-happiness-

report-2021

---

7. 数据集将以.zip压缩包形式下载到Kaggle文件夹，解压后即可使用。

从上述步骤可见，在Colab中使用Kaggle数据集非常简单——只需获取API令牌，且切换平台后可使用比Kaggle分配更多的GPU时长。

## 法律声明

能在Kaggle上传数据并不意味着应该上传。典型案例如"Tinder用户数据集"：2017年某开发者通过Tinder API抓取半公开用户资料并上传至Kaggle，事件曝光后该数据集被下架。完整报道详见：https://www.forbes.com/sites/janetwburns/2017/05/02/tinder-profiles-have-been-looted-again-this-time-for-teaching-ai-to-genderize-faces/?sh=1afb86b25454。通常在上传前请自问两个问题：

1. 从版权角度是否允许？请务必检查相关许可证。如有疑问，可随时查阅https://opendefinition.org/guide/data/或联系Kaggle。

2. 该数据集是否存在隐私风险？严格来说，发布某些类型信息虽不违法，但可能侵害他人隐私。

这些限制符合常识，因此不太可能阻碍你在Kaggle上的工作。

## 本章小结

本章介绍了Kaggle数据集——该平台上存储和使用数据的标准化方式。我们探讨了数据集创建、Kaggle外部工作方法，以及最重要的功能：在Notebook中使用数据集。这为下一章关于Kaggle Notebooks的内容做了自然过渡。

## 加入本书的Discord空间

加入本书的Discord工作区，每月可参与作者问答会：

https://packt.link/KaggleDiscord

## 第三章 使用Kaggle Notebooks工作与学习

Kaggle Notebooks（近期前称为Kernels）是可在浏览器中免费运行的Jupyter Notebooks。这意味着只要有网络连接，你就能在任何设备上执行实验（不过建议使用比手机更大的设备）。截至本书撰写时，环境技术规格引自Kaggle官网，最新版本可查阅https://www.kaggle.com/docs/notebooks：

- CPU/GPU最长运行时间12小时，TPU为9小时

- 20GB自动保存的磁盘空间（/kaggle/working目录）

- 临时暂存盘空间（/kaggle/working目录外），当前会话结束后不保存

## CPU规格：

- 4核CPU

- 16GB内存

GPU规格：

- 2个CPU核心

- 13GB内存

TPU规格：

- 4个CPU核心

- 16GB内存 本章将涵盖以下主题：

- 设置Notebook

- 运行Notebook

- 将Notebook保存至GitHub

- Notebook高效使用技巧

- Kaggle Learn课程

闲言少叙，让我们直接开始。首先需要了解如何设置Notebook。

## 设置Notebook

创建Notebook主要有两种方式：通过首页或通过数据集页面。

第一种方法：访问Kaggle官网(https://www.kaggle.com/)左侧菜单栏的Code版块，点击+ New Notebook按钮。若实验需上传自有数据集，推荐此方式。第二种方法：如前一章所示，可前往目标数据集页面点击New Notebook按钮：

<!-- Media -->

<!-- figureText: Code Random Forest GPU TPU Competition notebook See all (251) 10 Hotel_Booking_Dataset_Pract : STARTER Notebook( Simple Updated 44 minutes ago Hotel Booking Updated 2 hours ago Tabular Playground Series - Jul 2021 Explore and run machine learning code with Kaggle Notebooks. Find help in the Documentation New Notebook Your work Search public notebooks All notebooks Recently Viewed Python R Beginner NLP Finance Trending Spam Classifier with the use TPS-07 Turtles on turtles... Updated 13 hours ago Updated 9 hours ago Tabular Playground Series - Jul 2021+2 Email Spam -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_78.jpg?x=249&y=1078&w=1398&h=796&r=0"/>

图3.1：通过Code页面创建新Notebook

<!-- figureText: ☒ Dataset Download (2 MB) Temperature Forecast Project using ML Predict Minimum and Maximum Temperature during a day based on various features - Ayush Yadav - updated 12 hours ago (Version 1) 图 Usability 7.4 4 Tags intermediate, environment, regression, categorical data, korea Description Temperature Forecast Project using ML Problem Statement: Data Set Information: This data is for the purpose of bias correction of next-day maximum and minimum air temperatures forecast of the LDAPS model operated by the Korea Meteorological Administration over Seoul, South Korea. This data consists of summer data from 2013 to 2017. The input data is largely composed of the LDAPS model's next-day forecast data, in-situ maximum and minimum temperatures of present-day, and geographic auxiliary variables. There are two outputs (i.e. next. maximum and minimum air temperatures) in this data. Hindcast validation was conducted for the period from 2015 to 2017. Attribute Information: For more information, read [Cho et al, 2020]. -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_79.jpg?x=247&y=351&w=1394&h=849&r=0"/>

<!-- Media -->

图3.2：通过数据集页面创建新Notebook

无论选择哪种方式，点击"新建笔记本"后，您将进入笔记本页面：

<!-- Media -->

<!-- figureText: notebook729b4575b trait saved (C) Save Version (B) Draft Session off from a cell to start) Data + Add data Output - ☐ /kaggle/working Settings Language Python - Accelerator PIND CODE MILP Q Find Code Help File Edit View Run Add-ons Help + B X I D D D A D A D C D D E - The Python Conservement plans with many initial smallness different detectors. Intuitive import many \( m \rightarrow  0 \) linear algebra impact pandas as pd- \( \theta \) data processing, the file SID (4.6) and red_cool trees, .. falsmates in an mili('/taggin/input'): + Code) + Markdown -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_79.jpg?x=246&y=1409&w=1395&h=504&r=0"/>

图3.3：笔记本页面

<!-- Media -->

在上图所示的新建笔记本页面右侧，有多个可调整的设置项：

<!-- Media -->

<!-- figureText: & Share L Save Version 入 Add data ☐ /kaggle/working 45 Python Preferences Schedule a notebook run Find Code Help Search for examples of how to do things Data Input Output Settings Language Environment Accelerator Internet Code Help FIND CODE HELP -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_80.jpg?x=603&y=329&w=682&h=985&r=0"/>

图3.4：笔记本选项

<!-- Media -->

我们将简要说明这些设置。首先是编程语言选项。截至本文撰写时，Kaggle环境仅支持Python和\( \mathrm{R} \)作为笔记本编程语言。默认新建笔记本会初始化设置为Python语言——如需使用\( \mathrm{R} \)，请点击下拉菜单选择\( \mathrm{R} \)。

接下来是环境选项：这个切换开关让您选择是始终使用最新的Docker环境（风险选项：能快速获取更新但依赖项可能在后续更新中失效），还是将笔记本固定使用Kaggle提供的原始环境版本（安全选择）。后者是默认选项，除非您正在进行非常活跃的开发工作，否则没有实际理由需要改动它。

加速器选项允许用户选择代码运行方式：CPU（无加速）、GPU（几乎所有涉及深度学习的严肃应用都必需）或TPU。请注意从CPU切换到（单个）GPU只需对代码做最小改动，可通过系统设备检测自动处理。而将代码迁移到TPU则需要从数据预处理开始进行更复杂的重写。重要提示：您可以在处理笔记本时随时切换CPU/GPU/TPU，但每次切换都会重启环境，需要从头运行所有代码。

最后是网络开关，用于启用或禁用在线访问。当连接网络时，如需安装额外软件包，依赖项的下载和安装将在后台自动完成。最需要手动禁用网络的情况是参加明确禁止提交时联网的比赛。

使用笔记本的一个重要特性是，您可以随时克隆现有笔记本（由您或其他Kaggle用户创建）并根据需求修改。只需点击笔记本页面右上角的"复制并编辑"按钮即可。在Kaggle术语中，这个过程被称为分叉：

<!-- Media -->

<!-- figureText: Q search Version 1 of 2 colored from \( \circ \) (Pack of) LightGOBM + CatBout + ANN 250512 (+1-1) Notebeat MLB Player Digital Sho except + LightGBM + CatBoost + ANN Best Submission Public Score Submitted by Chi-10510 22 days ago 1.3260 MLB Player Digital Engagement Forecasting LightGBM + CatBoost + ANN 2505f2 -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_81.jpg?x=247&y=965&w=1397&h=319&r=0"/>

图3.5：分叉现有笔记本

<!-- Media -->

关于礼仪的说明：如果您曾参加过Kaggle比赛，可能已经注意到排行榜上充斥着高分笔记本的分叉再分叉。基于他人作品进行开发本无不妥——但若这样做，请记得为原作者点赞，并明确注明参考作品的创作者。

您创建的笔记本默认是私有的（仅自己可见）。若想与他人共享，可以选择添加协作者（仅明确添加到列表的用户可查看或编辑内容），或将笔记本设为公开（所有人可见）。

## 运行笔记本

所有编码工作已完成，笔记本运行正常，准备执行。请前往笔记本页面右上角点击"保存版本"。

<!-- Media -->

<!-- figureText: Draft Session off (run a cell to start) & Share C Save Version Data + Add data ☐ input (128.18 GB) - rsna-miccai-brain-tumor-radiog.. efficientnet-pytorch ☐ output ☐ /kaggle/working 0 Settings Language Python Environment Preferences Accelerator GPU ▼ GPU Quota 00:00 / 41 hrs Internet Code Help Data Analysis and Modeling -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_82.jpg?x=320&y=424&w=1246&h=930&r=0"/>

图3.6：保存脚本

<!-- Media -->

"保存并全部运行"通常用于执行脚本，但还有个"快速保存"选项，可在脚本准备提交前保存中间版本：

<!-- Media -->

<!-- figureText: important for brain cancer treatment 9 / 50 Save AI Brain Tumor Radiogenomic Classification challenge C Save Version Version Name (optional): Version 4 Save & Run All (Commit) Run a fresh copy of your notebook and save the output Save & Run All (Commit) Run a fresh copy of your notebook and save the output Quick Save Save a version of your notebook the way it currently looks Quick Navigation -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_83.jpg?x=242&y=212&w=1402&h=850&r=0"/>

图3.7：保存版本的不同选项

<!-- Media -->

启动脚本后，您可以前往左下角点击"活动事件"：通过该面板可监控Notebook的运行状态。正常执行会显示"运行中"消息，否则将标记为"失败"。若需终止运行中的会话（例如发现未使用最新数据），只需点击活动事件列表右侧的三点菜单，系统将弹出如下图所示的操作窗口：

<!-- Media -->

<!-- figureText: Version #4 with GPU - Brain Tumor - EDA with Animations an.. just now Running: just now 1 Active Event -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_83.jpg?x=245&y=1277&w=1396&h=476&r=0"/>

图3.8：监控活动事件

<!-- figureText: Z 6m to run Titanic Survival Prediction : How I got to top 3% Python Notebook on Titanic - Machine Learning from Disaster isualizations Edit Stop Session Open In Viewer Pclass \( = 2 \mid \) Survived \( = 0 \) Pclass \( = \) Brain Tumor-2- EDA with Animations an. Version #4 with GPU Running: just now 1 Active Event https://www.kaggle.com/sv/72449528 -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_84.jpg?x=242&y=492&w=1405&h=492&r=0"/>

图3.9：取消Notebook执行

<!-- Media -->

## 将Notebook保存至GitHub

最新推出的功能（参见https://www.kaggle.com/product-feedback/295170）允许将代码或Notebook存储至版本控制平台GitHub（https://github.com/）。无论是公开还是私有仓库，代码版本保存时都会自动同步。该功能既能方便与Kaggle队友协作，也可用于向公众展示作品。

启用该功能需打开Notebook，在文件菜单中选择"关联GitHub"选项。

<!-- Media -->

<!-- figureText: [Tutorial] Feature selection with Boruta-SHAP Draft save AUL Markdown with Boruta-SHAP to in Feature Importance Run Add-ons New Notebook m Upload Notebook Link to GitHub Download Notebook Upgrade to Google Cloud AI Notebooks Set as Utility Script 回 Add or upload data Add utility script -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_85.jpg?x=293&y=215&w=1306&h=830&r=0"/>

图3.10：启用GitHub功能

<!-- Media -->

选择该选项后，需将GitHub账户与Notebook关联。首次关联时会明确请求权限授权，后续新建Notebook的关联操作将自动完成。完成关联后，保存工作时即可同步至指定仓库：

<!-- Media -->

<!-- figureText: [Tutorial] Feature selection with Boruta-SHAP Draft saved 2. Share Kaggle needs to sync with your GitHub account for this feature to work. You can review the specific authorization in the next step and can unlik from GitHub at any File Edit View Run Add-ons Help Markdown Feature selection with Poruto SHAP to increase your search. Link to GitHub time. C. Link to GitHub \( {10}^{0} \) -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_85.jpg?x=247&y=1313&w=1396&h=698&r=0"/>

图3.11：关联GitHub

<!-- figureText: Save copy to GitHub Upload this ipynb to GitHub under your GitHub account Imassaron. This can only be undone directly on GitHub. REPOSITORY Imassaron/kaggle_public notebooks BRANCH main FILE NAME tutorial-feature-selection-with-boruta-shap.ipynb COMMIT MESSAGE Kaggle Notebook | [Tutorial] Feature selection with Boruta-SHAP | Vers - Include a link to Kaggle -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_86.jpg?x=246&y=337&w=1395&h=1124&r=0"/>

图3.12：提交作品至GitHub

<!-- Media -->

选定仓库和分支（便于存储不同开发阶段的作品）后，可修改推送至仓库的文件名称及提交说明。

如需取消特定Notebook的同步，只需返回文件菜单选择"解除GitHub关联"。若要完全停止Kaggle与GitHub仓库的连接，可通过Kaggle账户页面的"我的关联账户"或GitHub设置页面（https://github.com/settings/applications）解除账户关联。

## Notebook高效使用指南

Kaggle每周重置免费资源配额，包括固定时长的GPU和TPU使用时长（TPU为30小时，GPU时长每周浮动，相关政策详见：https://www.kaggle.com/product-feedback/173129）。您可在个人资料中实时查看用量：

<!-- Media -->

<!-- figureText: Konrad Banachewicz Your Profile Account Sign Out Your accelerator quota GPU 41h available of 41h 30h available of \( {30}\mathrm{\;h} \) -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_87.jpg?x=519&y=583&w=851&h=875&r=0"/>

图3.13：加速器配额使用状态

<!-- Media -->

尽管乍看之下这些数字可能显得庞大，但这种第一印象往往具有欺骗性；实际上很容易在短时间内耗尽您的配额。以下是一些实用建议，可帮助您控制资源使用：

- 配额计数器（用于测量您使用所选加速器、GPU或TPU的时长）从您初始化Notebook的那一刻起就开始计时。

- 这意味着您应始终先在设置中确认GPU处于禁用状态（参见前文图3.6）。先编写基础代码框架，检查语法，待添加真正依赖GPU初始化的代码部分时再启用/禁用GPU。请注意：更换加速器时Notebook会重启。

- 通常建议先在数据的小子集上端到端运行代码以感知执行时间。这样可以最大限度降低代码因超出限制而崩溃的风险。

有时Kaggle免费提供的资源不足以应对当前任务，您需要转移到更强大的机器上。最近的肿瘤分类竞赛就是典型案例：https://www.kaggle.com/c/rsna-miccai-brain-tumor-radiogenomic-classification/data

若原始数据超过100GB，您要么需要调整图像尺寸/降采样（这可能对模型性能产生负面影响），要么在能处理高分辨率图像的环境中训练模型。您可以自行搭建整套环境（第二章"在Google Colab中使用Kaggle数据集"章节有示例），也可以继续使用Notebook框架但更换底层机器。这正是Google Cloud AI Notebooks的用武之地。

## 升级至Google云平台(GCP)

升级到GCP最明显的好处是能使用更强大的硬件：Kaggle免费提供的Tesla P100 GPU对多数应用尚可，但性能并非顶尖，16GB内存也容易成为瓶颈——特别是在大型NLP模型或高分辨率图像处理等资源密集型应用中。虽然执行时间的改善显而易见，能加速开发周期迭代，但这是有代价的：您需要决定准备投入多少预算。对于处理复杂计算的强力机器而言，时间确实就是金钱。

要将Notebook迁移至GCP环境，请点击右侧边栏菜单中的"升级至Google Cloud AI Notebooks"选项，随后会出现以下提示：

<!-- Media -->

<!-- figureText: Version 34 of 34 11 立 Share / Edit C Copy and Edit Notebook ≡ View Copies (1) - Download code \( \Leftrightarrow \) Embed notebook B Copy API command - Upgrade to Google Cloud AI Notebooks - Unfollow Notebook C. Unfollow Comments Bookmark Delete Notebook Notebook Groundwork Patterns Dependence Stationarity Input (2) Execution Info Log Comments (5) -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_89.jpg?x=295&y=200&w=1282&h=1196&r=0"/>

图3.14：升级至Google Cloud AI Notebooks选项

<!-- Media -->

# 升级至Google Cloud AI平台Notebooks

Google云平台

通过将您的notebook及其依赖项导出至Google Cloud AI平台Notebooks，获取更强大的计算能力，在此您可以自定义虚拟机，不受配额或运行时限制。

## 该过程分为三步：

1. 设置已启用结算功能的Google云项目

2. 配置您的notebook实例，并可选择自定义机器配置

3. 无限制运行您的代码 取消

图3.15：升级至Google Cloud AI平台Notebooks的提示

点击继续后，您将被重定向至Google云平台控制台，需在此配置账单选项。请注意：GCP并非免费服务。首次使用时，系统将引导您完成必要步骤的教程。

## 更进一步

如本章前文所述，Kaggle Notebooks不仅是绝佳的教育与竞赛工具，还具有另一重要用途——作为展示数据科学能力的作品集组成部分。

构建数据科学作品集时需考虑诸多标准（品牌塑造、受众触达、向潜在雇主展示等），但若无人发现则毫无意义。由于Kaggle隶属谷歌，其Notebooks会被全球最流行的搜索引擎收录。当有人搜索与您代码相关的主题时，它就会出现在搜索结果中。以下是我的亲身案例：几年前我为某竞赛编写的Notebook涉及对抗性验证（对此概念陌生的读者：通过构建能区分训练集与测试集的二分类器，可简单判断两者分布是否相似，第六章《设计优质验证》将详细阐述）。撰写本章时我尝试搜索该Notebook，它赫然出现在搜索结果前列（注意我的搜索词未提及Kaggle或任何个人信息）：

<!-- Media -->

<!-- figureText: adversarial validation code × ↓ Q ‡ More Tools ✓ ✓ ✓ ✓ Feedback Q All E Images 3 Videos ☑ News About 1.100.000 results (0,45 seconds) https://towardsdatascience.com > adversarial-validation-ca... Learning the Adversarial Validation model - Towards Data ... Go there for better rendering of in-line code. Introduction. If you were to study some of the competition-winning solutions on Kaggle, you might notice .. 21 Jan 2020 - Uploaded by WelcomeAlOverlords https://www.kdnuggets.com > 2016/10 > adversarial-val... + Adversarial Validation, Explained - KDnuggets This post proposes and outlines adversarial validation, a method for selecting training examples most similar to test ... The code is available at GitHub. People also ask What is adversarial validation? What is the difference between cross-validation and holdout validation? What is the validation set in the 3 way cross-validation for? What is cross-validation and validation machine learning? https://www.kaggle.com > konradb > adversarial-validat... v Adversarial validation and other scary terms | Kaggle Explore and run machine learning code with Kaggle Notebooks | Using data from Sberbank Russian Housing Market -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_91.jpg?x=389&y=614&w=1107&h=1128&r=0"/>

图3.16：Konrad的Notebook在Google搜索结果中显示

<!-- Media -->

Notebooks展示技能的其它优势在于：与竞赛、数据集和讨论区相同，Notebooks可获得投票/奖章，助您在等级系统和排名中晋升。您可完全避开竞赛赛道，仅凭社区认可的高质量代码成为专家、大师或特级大师。最新等级要求详见https://www.kaggle.com/progression，以下是专家与大师级别的现行标准：

## 专家级

您已在Kaggle一个或多个专业领域完成大量工作。达到某领域的专家级别后，您将进入该领域的全站Kaggle排名系统。

<!-- Media -->

<!-- figureText: Competitions Datasets Notebooks Discussions § 5 bronze medals § 50 bronze medals You've demonstrated excellence in one or more categories of expertise on Kaggle to reach this prestigious tier. Masters in the Competitions category are eligible for exclusive Master-Only competitions. Notebooks Discussions C 10 silver medals § 50 silver medals - 200 medals in total § 2 2 bronze medals 2 3 3 bronze medals Master Competitions Datasets 1 gold medal 1 gold medal 2 2 silver medals - 4 silver medals -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_92.jpg?x=242&y=540&w=1405&h=559&r=0"/>

<!-- Media -->

图3.17：等级晋升要求

Notebooks类别的晋升颇具挑战性：虽比竞赛容易，但绝对比讨论区困难。最受欢迎的Notebooks通常与特定竞赛相关：探索性数据分析、端到端概念验证方案，以及排行榜冲刺方案。存在一个常见却令人遗憾的现象——用户克隆高分公开Notebook，微调参数提升分数后发布便能获得大量赞誉（如果投票可视为情绪指标）。此言并非劝阻读者在Kaggle发布优质作品（多数Kaggle用户确实欣赏原创，长期来看质量终将胜出），但有必要对预期进行现实调整。您的Kaggle个人资料可积累关注者，并支持关联LinkedIn或GitHub等职业网络，从而充分利用社区内建立的人脉：

<!-- Media -->

<!-- figureText: Konrad Banachewicz Discussion Followers 642 Grandmaster Discussion (1,240) Followers (642) ... Edit Public Profile Notebooks Discussion Master Grandmaster Current Rank Highest Rank Current Rank Highest Rank 152 54 79 of 177,997 of 206,287 10 24 60 88 586 Adversarial valid... 116 Augmented dat... 81 4 years ago votes 2.2 months ago votes We need to go d... 84 Shrink the data ... 75 -10 days ago votes 3 years ago votes Linear baseline ... 66 Minimalistic BER... 70 2.2 months ago 2-2 years ago votes I interrogate data for a living at TNG Quant Consultancy Haarlem, North Holland, Netherlands Joined 11 years ago - last seen in the past day Home Competitions (107) Datasets (23) Code (49) Competitions Datasets Master Expert Current Rank Highest Rank Current Rank Highest Rank 470 34 76 59 of 162,835 of 42,360 29 16 14 Homesite Quote... \( {3}^{rd} \) Augmented trai... 25 - 5 years ago 2-2 months ago votes Top 1% of 1755 Machinery Tube... \( {5}^{\text{th }} \) Pytorch-Tabnet 20 - 6 years ago -10 months ago votes Top 1% of 1320 AMS 2013-2014... \( {5}^{\text{th }} \) Text recognition... 17 2-8 years ago 2-2 years ago votes Top 4% of 160 -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_93.jpg?x=296&y=396&w=1312&h=878&r=0"/>

图3.18：Konrad的Kaggle个人资料

<!-- Media -->

当今时代，人们对"社区建设"的说法容易持疑，但Kaggle确实做到了。其在数据科学界的品牌认知度无可匹敌，无论是从业者还是做过功课的招聘者都深有体会。这意味着（足够优秀的）Kaggle资料就能为您打开机会之门——众所周知，这往往是最艰难的步骤。

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_94.jpg?x=242&y=233&w=353&h=356&r=0"/>

<!-- Media -->

## Martin Henze专访

https://www.kaggle.com/headsortails

我们有幸采访了Notebooks与讨论区双料特级大师Martin Henze（又名Heads or Tails），他现任Edison Software数据科学家，同时运营着《每周精选：被埋没的宝藏Notebooks》专栏，定期收录未被广泛关注的顶级Notebooks。关注他的Kaggle个人资料或Twitter、LinkedIn账号可获取最新精选通知。

你最喜欢哪种类型的竞赛？为什么？在技术方法和解决思路上，你在Kaggle的专长是什么？

长期以来，我的重心都放在探索性数据分析（EDA）笔记上，而非排行榜预测本身。加入Kaggle前，我主要处理表格数据，因此我的EDA笔记大多聚焦于从新发布的表格挑战中提取复杂洞见。这仍是我在Kaggle的专长领域，我投入了大量时间精心设计笔记结构、数据可视化及叙事逻辑。

## 你如何规划Kaggle竞赛策略？这与日常工作方法有何不同？

即便Kaggle已逐渐远离表格类竞赛，我始终坚信数据本身才是任何挑战的核心。过早关注模型架构和超参数调优是常见误区。事实上，多数竞赛的决胜关键仍在于以数据为中心的方法——建立在对数据集特性、异常值的深入理解之上。无论是图像数据、自然语言处理、时间序列还是其他数据结构，这条法则都适用。因此我的标准流程总是：先进行详尽EDA，搭建简单基线模型和交叉验证框架，再逐步迭代优化流程复杂度。

与日常数据科学工作最大的区别在于：在Kaggle新挑战发布首周，资深选手构建的基线模型往往就已达到工业级投产标准。从评分指标看，前几天的成果通常已逼近最终冠军方案的80%效能。当然，Kaggle的乐趣与挑战在于用创意方法攻克最后几个百分点的准确率——但这在工业界往往不如开启新项目来得高效。

## Kaggle对你的职业发展有帮助吗？具体体现在哪些方面？

Kaggle对我的职业轨迹产生了深远影响。这个社区的宝贵经验推动我从学术界转向工业界。如今我在科技初创公司担任数据科学家，仍持续通过Kaggle挑战来磨砺技能。

对我而言，精心构建Kaggle笔记形成了绝佳的作品集——虽然不确定招聘经理实际查阅频率，但我的Grandmaster头衔似乎比博士学位更能打开机会之门（或许两者相辅相成）。强烈建议建立公开笔记作品集。此外，求职期间我将Kaggle习得的策略应用于各种笔试任务，效果显著。

## 根据你的观察，新手Kaggle选手常忽视哪些要点？有哪些现在掌握的经验是你希望初学时就知道的？

认知成长是个持续过程——现在的我们总比十年前、五年前甚至去年的自己更睿智。抛开这点不谈，新手最常忽略的是制定明确计划并执行记录。这种失误完全可以理解：初次接触时，论坛、数据集、挑战赛、课程等海量内容令人眼花缭乱，竞赛题目如"神经元细胞实例分割"、"股市波动预测"更是让人望而生畏。但竞赛恰恰是最佳起点。

因为竞赛启动时，所有人基本都处于同一起跑线——或许有个别博士研究者恰好专攻该领域，但这种情况凤毛麟角。作为社区成员，从零开始挖掘数据、调试损失函数、运行基础模型，这种加速学习曲线能让你在集体智慧中快速成长。其他参赛者会提供大量灵感，但系统化计划仍是不可或缺的。

这个计划至关重要，因为盲目进行实验、看着GPU内存被占满而自我感觉良好是很容易的。但随后你会忘记哪个模型版本表现最佳，本地验证与排行榜成绩是否存在关联？这个参数组合我是否已经测试过？因此务必预先规划实验方案并记录结果。虽然自动记录工具日益增多，但自定义脚本也能轻松实现。机器学习本质上仍是实验科学，高效实验的关键在于周密规划并详尽记录所有结果以供对比分析。

## 你在过往比赛中犯过哪些错误？

我犯过大量错误，所幸从中汲取了教训。比如缺乏稳健的交叉验证框架、忽视训练集与测试集的分布差异。在最初几场比赛中，我过度沉迷探索性分析(EDA)而轻视模型构建——这堪称我的标志性失误。当然也有EDA不足导致遗漏关键特征的经历。还有一次未筛选最终提交的两个方案（虽影响不大，但永生难忘）。

关于错误的核心观点与我先前谈实验计划时一脉相承：只要能促进成长，犯错无可厚非。真正要避免的是那些本可预见的低级错误。在机器学习（乃至整个科学领域）中，失败本就是探索过程的一部分。并非所有尝试都会成功，这很正常。但切忌重复相同的错误——唯有不从错误中学习才是真正的失败。这个道理适用于Kaggle竞赛，也适用于人生。

## 有哪些特别推荐的数据分析或机器学习工具/库？

尽管Python日益盛行，但在表格数据处理和可视化方面，我仍偏爱\( R \)及其tidyverse生态：dplyr、ggplot2、lubridate等。新兴的tidymodels框架正成为sklearn的有力竞争者。即使你是Python死忠，偶尔跨出pandas的圈子也会获益良多——不同工具往往能激发新视角与创造力。深度学习领域，我认为PyTorch及其FastAI接口最符合直觉。当然，如今hugging face风靡业界也实属情理之中。

## 参加比赛时最需要牢记什么？

最重要的是享受过程并保持学习心态。比赛中及赛后涌现的宝贵洞见与智慧，若不吸收转化将是巨大浪费。即便你只在乎获胜，也唯有通过学习实验、站在社区巨人的肩上才能实现。但Kaggle的价值远超越排行榜——当你开始回馈社区时，将获得更全面的成长。我对此深信不疑。

## Kaggle Learn课程

Kaggle的精髓在于知识获取：无论是竞赛中学到的技巧、海量资料库中发现的数据集，还是前所未闻的模型范例，总有新知待发掘。最新加入这一体系的是Kaggle Learn系列课程：https://www.kaggle.com/learn。这些微课程被官方定位为"掌握独立数据科学项目技能的最快途径"，核心特色是通过速成形式覆盖多元主题。每门课程分设小节，配套编程练习题，采用理论讲解与代码实践交织的Notebook形式教学。

以下是精选课程概览：

- 机器学习入门/进阶：https://www.kaggle.com/learn/intro-to-machine-learning 与 https://www.kaggle.com/learn/intermediate-machine-learning

建议将这两门课程视为上下篇：前者介绍机器学习模型分类，探讨欠拟合/过拟合、模型验证等通用议题；后者深入特征工程、缺失值处理及分类变量转换。非常适合机器学习初学者。

- pandas教程：https://www.kaggle.com/learn/pandas

本课程将速成介绍现代数据科学中最基础的工具之一。您首先学习如何创建、读取和写入数据，继而掌握数据清洗技巧（包括索引、选择、合并、分组等）。无论对初学者（pandas功能有时会令人应接不暇）还是从业者（作为复习/参考）都极具价值。

- 游戏AI：https://www.kaggle.com/learn/intro-to-game-ai-and-reinforcement-learning

本课程完美总结了Kaggle学习模块中技术导向的课程内容。您将编写游戏对战智能体、优化其性能，并运用极小化极大算法。这堪称是以实践为导向的强化学习入门佳作。

- 机器学习可解释性：https://www.kaggle.com/learn/machine-learning-explainability

构建模型充满乐趣，但现实世界中并非人人都是数据科学家，因此您可能需要向他人解释自己的工作。这门关于模型可解释性的迷你课程正是为此而生：您将学习使用三种方法评估特征重要性——排列重要性、SHAP值和部分依赖图。对于商业场景中的ML从业者至关重要，项目成败往往取决于沟通效果。

- AI伦理：https://www.kaggle.com/learn/intro-to-ai-ethics

这门收官课程为整个体系增添了发人深省的一笔：探讨指导AI系统道德设计的实用工具。您将学会识别AI模型偏见、审视AI公平性概念，并掌握通过传达ML模型信息提升透明度的方法。对从业者极具实用价值，因为"负责任AI"正成为日益重要的议题。

除Kaggle原创内容外，平台还提供用户创建Notebooks等学习资源，建议读者自行探索。

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_98.jpg?x=242&y=1242&w=358&h=366&r=0"/>

<!-- Media -->

## 安德拉达·奥尔泰亚努

https://www.kaggle.com/andradaolteanu

安德拉达·奥尔泰亚努是Kaggle Notebooks大师赛冠军，她极力推崇通过Notebooks学习。作为Z by HP全球数据科学大使、Endava数据科学家及Weights & Biases开发专家，我们与她探讨了Notebook竞赛、职业生涯等话题。

## 您最青睐哪类竞赛？原因何在？在Kaggle平台上，您的技术专长体现在哪些方面？

我认为自己在Kaggle的特长更偏向数据可视化，这让我能将艺术创意与数据相结合。

谈不上偏爱某类竞赛，我更倾向于偶尔切换赛道，选择当下感兴趣的内容。

Kaggle的魅力在于既能学习数据科学的多元领域（计算机视觉、自然语言处理、探索性数据分析和统计学、时间序列等），又能熟悉各类主题（如体育、医疗、金融与加密货币、国际事件等）。

另一大优势是：例如当您想提升文本数据处理能力时，Kaggle几乎总有相应的NLP竞赛；若想学习音频文件预处理与建模，也有对应竞赛可供练手。

## 请分享一次特别具有挑战性的竞赛经历，以及您攻克任务的关键洞见。

我参与过最具挑战性的"竞赛"是"Kaggle数据科学与机器学习年度调查"。虽然这并非传统意义上的比赛——没有排行榜和高强度机器学习任务——但它却是我倾注最多汗水、收获最丰的经历之一。

这是场笔记本竞赛，参赛者需要发挥创意才能赢得Kaggle设置的5个奖项。我连续两年参赛：首年（2020）挑战了我的基础可视化能力，迫使我突破常规思维（获得季军）；次年（2021）我花了四个月学习D3技术，试图将数据可视化技能提升到全新高度（仍在评审中，目前已获得"早期笔记本奖"）。\( I \)能提供的最佳建议是：

- 首先不要迷失在数据中，要确保图表绝对精确，必要时建立双重验证机制。再精美的图表若呈现错误见解都毫无价值。

- 从自然、电影、工作中寻找灵感，汲取绝妙主题与创意方式来提升可视化效果。

## Kaggle对您的职业发展有何助益？

帮助巨大。我职业生涯的成就很大程度上归功于Kaggle，对此我永远感激。通过Kaggle，我成为HP品牌大使；发现了卓越的机器学习平台Weights & Biases并成为其开发专家；更重要的是结识了现任雇主Endava的首席数据科学家，他招募了我并成为长期合作伙伴。简言之，我当前职位与两家巨头企业（HP和Weights & Biases）的联系都直接源于Kaggle活动。这个平台最被低估的价值是其社区——汇聚了最庞大的人才库，可供交流学习。

最佳利用方式是：从每个Kaggle板块（竞赛/数据集/笔记本/讨论区）选取前100名用户，在Twitter/LinkedIn上关注所有公开联系方式的优秀者。通过定期互动，你能从这些知识渊博的群体中获得宝贵见解。

## 您过往参赛犯过哪些错误？

最大错误就是不敢参赛。我认为这是新手最根本的误区——

出于恐惧（我深有体会），他们总觉得自己准备不足或不知如何起步。其实只要遵循简单步骤，参赛就会变得容易：

- 选择任何感兴趣的比赛

- 仔细阅读说明文档并探索数据

- 若不知如何开始，只需在"代码"区寻找高赞笔记本或大师作品，通过"跟敲代码"模仿学习，边研究边改进。这是最佳学习方式——在具体项目中实践，永远不会卡壳。

## 参赛时最重要的注意事项？

要牢记\( {OK} \)失败是学习的最佳途径。

还应向竞赛大师学习，他们常会分享令人茅塞顿开的机器学习技巧。效仿成功者能让你少走弯路，快速平稳地迈向成功。选择2-3位崇敬的大师作为导师，深入研究他们的笔记本，通过代码实践尽可能吸收知识。

## 您是否使用其他竞赛平台？它们与Kaggle相比如何？

我从未使用过其他竞赛平台——只因我觉得Kaggle已囊括一切。

## 本章小结

本章我们探讨了Kaggle Notebooks这个多功能开放式编程环境，它既可用于教育实验，也能助力数据科学项目作品集推广。现在您已具备创建个人Notebook的能力，可高效利用现有资源，并将成果应用于竞赛或独立项目。

下一章我们将介绍讨论论坛，这是在Kaggle上交流观点与想法的主要渠道。

## 加入本书的Discord空间

加入本书的Discord工作区，每月参与作者问答专场：

https://packt.link/KaggleDiscord

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_103.jpg?x=229&y=310&w=200&h=235&r=0"/>

<!-- Media -->

## 善用讨论论坛

讨论论坛是Kaggle上信息交流的主要途径。无论是探讨进行中的竞赛、参与数据集对话，还是评价展示新方法的Notebook，Kaggle用户始终保持着活跃交流。

本章将介绍讨论论坛的组织架构、管理海量信息的使用规范，涵盖以下主题：

- 论坛运作机制

- 范例竞赛的讨论策略

- 网络礼仪

## 论坛运作机制

您可通过多种方式进入讨论论坛。最直接的方法是点击左侧面板的"讨论"选项：

<!-- Media -->

<!-- figureText: Search 90.2 Recent topics by Bambula, Kaminarimon, HuzaifaMS 第25 Recent topics by Emma, HuzaifaMS, Adi 2G Recent topics by HuzaifaMS, Björn, ibexorigin 2.99 Recent topics by Jae-Yu Yeh, Dibbsss, dustinb Home Competitions Discussions Discuss the Kaggle platform & machine learning topics - this includes sharing feedback, asking questions, and more. Code B Discussions Your Discussions Courses More Forums Recently Viewed General Explosive Violence Mo... Announcements, resources, and interesting discussions last post 2 minutes ago by Bambula Kats by Facebook : A n... Practical time series - ... Getting Started The first stop for new Kagglers Practical time series - ... last post 7 minutes ago by Emma TF/JAX Tutorials - Part3 Product Feedback Tell us what you love, hate, and wish for last post 2 hours ago by HuzaifaMS Questions & Answers Technical advice from other data scientists last post 2 hours ago by Jae-Yu Yeh -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_104.jpg?x=242&y=205&w=1403&h=960&r=0"/>

图4.1：从主菜单进入讨论页面

<!-- Media -->

顶部区域是论坛板块，汇集了各类通用主题。无论是初次参赛、提出建议，还是因困惑而提出一般性问题，浏览这些内容都很有帮助。

论坛下方是Kaggle全站讨论的综合视图：主要是竞赛相关对话（构成Kaggle大部分活动），也包括Notebook或知名数据集。默认按热度排序，即参与度最高、最活跃的内容靠前显示。这个板块能让你找到更贴合该领域动态特性的内容：来自Kaggle不同子集的讨论集合，并支持按特定条件筛选：

<!-- Media -->

2. Kaggle全站讨论

<!-- figureText: Q Search discussions — Filters NLP Neural Networks Hotness 13 comments ... 104 - New comments - 50 comments - 33 comments ... 31 comments ... 115 comments ... 26 comments \( {}^{a} \) Your Activity Bookmarks Beginner Data Visualization Computer Vision Received suspicious team merge offer kaerururu - in CommonLit Readability Prize - Last comment 8h ago by Minh Tri Phan DICOM to PNG dataset \( \left( {{128}\mathrm{{GB}} \rightarrow  {5.2}\mathrm{{GB}}}\right) \% \) Jonathan Besomi - In RSNA-MICCAI Brain Tumor Radiogenomic Classification - Last comment 1h ago by Abhishek Prajapat Commonly used Machine Learning Algorithms vardhan SIRAMDASU - in General - Last comment \( {14}\mathrm{\;m} \) ago by EmBahr About the targets Ahmet Erdem - in MLB Player Digital Engagement Forecasting - Last comment 6h ago by something4kag Competition Relaunch - New Data! Inversion - in SETI Breakthrough Listen - E.T. Signai Search - Last comment 14h ago by Mani Sarkar Companies and Data Science Interview questions sai pavan saketh - in Getting Started - Last comment 1h ago by Cristiano de Magalhäes, Eng. Did we missed something? Lukasz Borecki - in Tabular Playground Series - Jul 2021 - Last comment 2h ago by Lukasz Borecki -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_105.jpg?x=246&y=279&w=1398&h=849&r=0"/>

图4.2：Kaggle全站讨论

<!-- Media -->

根据兴趣，你可以使用筛选器个性化内容。基于偏好，可按以下条件筛选：

- 最新：控制你获取信息的时效范围

- 我的活动：查看你在所有论坛的评论/发布/浏览概况，适合同时参与多个讨论时使用

- 管理员：快速查看Kaggle管理员的公告

- 类型：讨论可能发生在通用论坛、特定竞赛或数据集周围

- 标签：虽然并非所有讨论都有标签，但部分讨论会被标记，此功能可让用户利用该特性：

<!-- Media -->

<!-- figureText: RECENCY Last 7 Days Today Viewed Dataset Clear Apply Last 30 Days MY ACTIVITY Commented Published AUTHOR Admin TYPES Site Forums Competition TAGS Search for tags -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_106.jpg?x=522&y=347&w=842&h=1223&r=0"/>

图4.3：讨论可用筛选器

## 下图展示了筛选"初学者"标签讨论的示例输出：

<!-- figureText: 2: Discussion from across Kaggle Filters \( {}^{1} \) Hotness 9 comments ... 71 comments ... 66 comments ... 7 comments ... 23 comments ... 4 13 ▼ 21 comments ... 9 comments ... Clear filters to enable search Beginner \( \times \) Resources of the Week : #12 Pranjal Verma - in General - Last comment 1h ago by Shashank Srivastava Best Data Science / Youtube Channels [1] Jonas Neri - in Getting Started - Last comment 4h ago by Elias Elfarri More than 250 Awesome Public Datasets PAVAN KUMAR D. in General - Last comment \( {10}\mathrm{\;h} \) ago by hashmi D. Resources of the Week : #12 Pranjal Verma - in Getting Started - Last comment 2h ago by laxman kusuma Everything about : GAN - Generative Adversarial Networks \( \mathrel{\text{\rightarrow \not{} }} 3 \) Resources Shivani Rana 63 - in General - Last comment \( {42}\mathrm{\;m} \) ago by Kaan BOKE What is the secret behind random seed 42 ? Old Monk - in RSNA-MICCAI Brain Tumor Radiogenomic Classification - Last comment 7h ago by Manu Siddhartha Commonlit : Some Good things to learn Shahules - in CommonLit Readability Prize - Last comment 1h ago by Araik Tamazian -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_107.jpg?x=241&y=253&w=1400&h=1147&r=0"/>

图4.4：筛选标记为"初学者"的讨论

<!-- Media -->

另一种方式是聚焦特定主题；由于计算机视觉等主题关注度高，对主题排序很有必要。可按热度、最新评论、最新发布、最多投票和最多评论排序：

<!-- Media -->

<!-- figureText: - Discussion from across Kaggle — Filters Hotness \( * \) Hotness Recent Comments Recently Posted Most Votes Most Comments 2 co - 22 . 18 comments ... Clear filters to enable search Computer Vision \( \times \) What is the secret behind random seed 42 ? Old Monk - in RSNA-MICCAI Brain Tumor Radiogenomic Classification - Last comment 7n age by Manu Siddhartha ⑥ ⑥ Resources of the Week : #11 Pranjal Verma - in Getting Started - Last comment 9h ago by hashmi Pretrained 3D-CNNs and other resources Alvaro Francesc Budria Fernández - in RSNA-MICCAI Brain Tumor Radiogenomic Classification - Last comment 9h ago by LucaMTB 3 Resources of the Week : #11 Pranjai Verma - in General - Last comment 2d ago by sarahpop小鳞牛 -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_108.jpg?x=247&y=208&w=1398&h=549&r=0"/>

图4.5：通用讨论论坛中的计算机视觉主题子集

<!-- Media -->

人们加入Kaggle目的各异，但尽管Notebook日益流行，竞赛仍是主要吸引力。每个Kaggle竞赛都有专属讨论论坛，通过竞赛页面选择"讨论"即可进入。虽然过去并非如此，但现在几乎所有竞赛都会在专属讨论论坛顶部置顶FAQ主题。建议从这里开始有两个主要原因：

<!-- Media -->

<!-- figureText: Featured Code Competition \$100,000 Prize Money Team My Submissions New Topic ... Following Filters Hotness 80 New comments -73 comments - . 23 comments ... Optiver Realized Volatility Prediction Apply your data science skills to make financial markets better tiver - 1,051 teams - 2 months to go ( 2 months to go until merger deadline) Overview Data Code Leaderboard Rules Discussions Search discussions Pinned topics Competition data FAQ Jiashen Liu - Last comment \( 2\mathrm{\;h} \) ago by Gunes Evitan seconds_in_bucket not starting from zero in some parts of the filler data Jiashen Liu - Last comment 3d ago by Jiashen Liu -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_108.jpg?x=261&y=1059&w=1342&h=958&r=0"/>

图4.6：竞赛讨论区

<!-- Media -->

- 它能节省您的时间；最常被提及的问题很可能已在此得到解答。

- 您可以避免在论坛其他板块提出重复问题，从而提升所有人的使用体验。

与笔记本功能类似，讨论区也允许您收藏特别相关的主题以供后续参考：

<!-- Media -->

<!-- figureText: Featured Code Competition \$100,000 Prize Money My Submissions New Topic We have received a lot of questions about the competition data, here we would like to provide a list of FAQ to make everyone up-to-speed. Most of below is already covered in the data page but good to A: Yes, stock_id is a unique identifier of a stock in real life, and the group of 112 unique stock_id will be Optiver Realized Volatility Prediction Apply your data science skills to make financial markets better Optiver - 1,051 teams - 2 months to go ( 2 months to go until merger deadline) Overview Data Code Discussion Leaderboard Rules Team Competition data FAQ Posted In optiver-realized-volatility-prediction 21 days ago Jiashen Liu Competition Host Hi all, 836th place Again, welcome to our competition! Very excited to see so many Kagglers participating already! mention here as well if helpful. Q: Is the same stock_id representing same stocks in all competition dataset? present in all datasets. Q: What does time_id mean and how the target-feature data are structured? -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_109.jpg?x=245&y=658&w=1405&h=873&r=0"/>

图4.7：在讨论区收藏主题

<!-- Media -->

所有已收藏主题的概览可在个人资料页面查看：

<!-- Media -->

<!-- figureText: Konrad Banachewicz Discussion Followers 807 Grandmaster Discussion (1,285) Followers (807) Edit Public Profile Highest Rank 91 609 Sort by Most Votes 472 competitions I interrogate data for a living at TNG Quant Consultancy Haarlem, North Holland, Netherlands Joined 11 years ago - last seen in the past day Home Competitions (113) Datasets (48) Code (62) Discussion Summary Current Rank 103 of 269,397 Discussion Grandmaster 3,357 upvoted Comments and topics Comments Topics Bookmarks 3 Embeddings, Cosine Distance, and ArcFace Explained. Topic 10 months ago in Shopee - Price Match Guarantee What are These Strange Words? -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_110.jpg?x=254&y=292&w=1382&h=1007&r=0"/>

图4.8：在讨论区收藏主题

<!-- Media -->

## 讨论方法示例

在竞赛中偶尔感到迷茫是完全正常的：你参与进来，尝试了几个想法，在排行榜上取得一些进展，然后遭遇了类似跑步者"撞墙"的Kaggle版困境。这时讨论论坛就是寻求建议的好地方。

以Optiver已实现波动率预测竞赛为例（https://www.kaggle.com/c/optiver-realized-volatility-prediction），主办方将其特点描述为：

在本竞赛的前三个月，您将构建预测跨行业数百只股票短期波动率的模型。您将掌握数亿行高度细化的金融数据，用以设计预测10分钟周期波动率的模型。您的模型将根据训练结束后三个月评估期内收集的真实市场数据进行评判。

这里涉及大量专业内容，我们将逐步解析该挑战的主要组成部分，并展示如何通过讨论论坛应对。首先，参与本竞赛需要一定金融知识基础——虽不一定要达到专业交易员水平，但对波动率计算不同方法的理解对普通人（大多数Kaggle用户在此领域都是）绝非易事。幸运的是，主办方在竞赛期间非常活跃，为领域新人提供了指导资源：https://www.kaggle.com/c/optiver-realized-volatility-prediction/discussion/273923。

若入门知识仍不足以开始，请大胆公开探讨并寻求帮助，如此例：https://www.kaggle.com/c/optiver-realized-volatility-prediction/discussion/263039。

或此例：https://www.kaggle.com/c/optiver-realized-volatility-prediction/discussion/250612。

随着竞赛推进，人们开始开发日益复杂的模型来解决问题。这里需要权衡：一方面，若您曾受益于前辈分享的成果，可能想要回馈社区；另一方面，您又不愿通过发布完整代码笔记本来泄露（潜在）优势。合理折衷是在论坛讨论您的特征构思，例如：https://www.kaggle.com/c/optiver-realized-volatility-prediction/discussion/273915。近年来，更多竞赛正摒弃固定测试数据集形式，引入某些变化：有时强制使用Kaggle API（这类竞赛要求通过笔记本提交），另一些则采用特殊时间表，分为训练阶段和实时数据评估阶段。Optiver就是后者：

最终提交截止后，排行榜将根据市场数据更新进行周期性刷新，这些更新会针对选定笔记本运行。更新频率约为每两周一次，并会避开冬季假期进行调整。

虽然规则表述简单，但这种设置给模型重新训练和更新带来了挑战。若遇到此类情况，可像该竞赛参与者这样咨询：https://www.kaggle.com/c/optiver-realized-volatility-prediction/discussion/249752。

模型验证方案始终是Kaggle竞赛的重要议题，通常伴随着永恒的"CV vs LB"（交叉验证与排行榜）讨论。Optiver竞赛也不例外：https://www.kaggle.com/c/optiver-realized-volatility-prediction/discussion/250650。

除非已有相关主题——建议先检索以避免重复——您可能需要考虑创建单模型性能类讨论。迟早所有人都会使用模型集成，但若没有优质单模型组件，集成效果也会受限。协作求知不止于此：若您认为找到了更好的解决方案，分享出来是明智之举。要么能为他人提供帮助，要么能发现自己方法的缺陷（节省时间精力），无论如何都是双赢，如此例所示：https://www.kaggle.com/c/optiver-realized-volatility-prediction/discussion/260694。

除了显而易见的个人收益（你能窥见其他参赛者的进展），这类讨论串促进了社区内的信息交流，增强了协作氛围，尤其对新手大有裨益。具体案例可参考https://www.kaggle.com/c/optiver-realized-volatility-prediction/discussion/250695。即便你已研读上述话题，可能仍会疑惑：是否遗漏了关键内容？在Kaggle这个平台，你完全可以坦然提问：https://www.kaggle.com/c/optiver-realized-volatility-prediction/discussion/262203。

让我们将视野拓展至其他赛事来收尾本节。前文提及的验证环节——对Kaggle用户而言——总与数据泄露和过拟合话题紧密相连。第六章将深入探讨泄露问题，该章节专攻验证方案设计。此处我们简要讨论如何通过社区交流应对这类问题。Kaggle聚集着充满探索精神的群体，一旦存在泄露嫌疑，总会有人发起讨论。

例如文件名称或记录ID可能包含时间戳，这意味着可通过逆向工程窥见未来数据，从而得出虚假的低误差指标值。Two Sigma Connect租赁房源咨询竞赛（https://www.kaggle.com/c/two-sigma-connect-rental-listing-inquiries/）就发生过此类情况。详情可参阅Kazanova的帖子：https://www.kaggle.com/c/two-sigma-connect-rental-listing-inquiries/discussion/31870#176513。

另一个案例是空客船舶检测挑战赛（https://www.kaggle.com/c/airbus-ship-detection），参赛者需在卫星图像中定位船只。后来发现大量测试图像其实是训练图像的随机裁剪片段，匹配两者变得异常简单：https://www.kaggle.com/c/airbus-ship-detection/discussion/64355#377037。

桑坦德银行赞助的系列竞赛可谓声名狼藉。该企业主办的三次Kaggle赛事中，两次出现数据泄露：https://www.kaggle.com/c/santander-value-prediction-challenge/discussion/61172。

后续处理因赛而异：Kaggle曾重置比赛并更新数据，也有认定影响轻微而继续赛事的先例。红帽商业价值预测竞赛的处置方式可供参考：https://www.kaggle.com/c/predicting-red-hat-business-value/discussion/23788。

尽管数据泄露可能严重干扰赛事，但好消息是近两三年间这类问题已在Kaggle近乎绝迹——但愿本节内容只需了解，不会成为你的平台日常。

关于平台经验的话题，自然过渡到对顶尖大师的专访。

<!-- Media -->

<!-- figureText: 世界 -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_114.jpg?x=245&y=339&w=354&h=353&r=0"/>

<!-- Media -->

## 谢逸凡

https://www.kaggle.com/yifanxie

谢逸凡身兼讨论大师与竞赛大师双料头衔，同时是Arion.ai联合创始人。以下是他就参赛经验和Kaggle协作分享的见解。

## 您最青睐哪类竞赛？为何？在技术方法层面，您在Kaggle的专长是什么？

我并无特定偏好，热衷解决各类问题。技术层面，我已构建完善的机器学习模块流程，能快速将典型技术算法应用于多数数据问题。这可谓我的竞争优势：长期专注于工作流程与技术产出的标准化，使数据实验能快速迭代——这正是Kaggle的核心竞争力。

## 您如何规划Kaggle竞赛策略？与日常工作有何差异？

多年来我形成了一套信息管理方法论，适用于工作、Kaggle及衍生项目。我会以标准化格式记录书签、数据字典、待办事项、实用命令和实验结果，组队时则与队友共享这些信息。

## 请分享最具挑战性的参赛经历及破局思路

对我而言，理解竞赛的宏观背景始终很有价值——比如支撑并产生我们所用数据的社会/工程/金融流程是什么？在能有效观察单个数据点的竞赛（如深度伪造检测挑战赛）中，我会用Streamlit搭建专用仪表盘，既能查验具体数据点（当时是真假视频对），也集成基础统计功能来增强数据感知。

## Kaggle对你的职业发展有帮助吗？具体体现在哪些方面？

可以说Kaggle是塑造我当前职业轨迹（数据科学咨询公司联合创始人）的最大推手。这个平台让我在多年间积累了跨领域解决数据问题的技能体系，通过组队参赛结识的客户与同事至今仍是重要人脉资源。即便现在参与度降低，它始终是我可靠的知识源泉。

## 根据你的观察，新手Kagglers常犯哪些错误？有哪些经验是你希望刚入门时就知晓的？

新人最易忽视关键的非技术事项：组队规则、数据使用条款、隐私信息共享、多账号操作等。这类错误可能让数月竞赛心血彻底白费。

真希望初学时就知道：不必纠结公开排行榜的每日排名——这种焦虑只会徒增压力，导致模型过拟合。

## 在数据分析或机器学习领域，有哪些特别推荐的工具或库？

常规工具如Scikit-learn、XGB/LGB、PyTorch等。特别建议深入掌握NumPy的高阶用法，比如数据排序与子集筛选——用pandas虽然省事，但NumPy的精细操作能大幅提升效率。

## 参加竞赛时最需要牢记的要点是什么？

我认为数据科学活动有四大动机：谋利、求知、趣味、向善。Kaggle对我而言是绝佳的知识宝库与美好回忆载体，所以永远要记住：排名转瞬即逝，知识记忆永存 :)

## 你使用其他竞赛平台吗？它们与Kaggle有何差异？

我是Numerai的活跃参与者。基于前述四大动机，这个通过加密货币支付奖金的平台更侧重盈利。由于组队优势不明显，它更偏向个人竞技——在Numerai这类交易竞赛中，人力投入与收益未必成正比。在我工作繁忙时期，Numerai比Kaggle更具可持续性，因为每轮训练数据基本固定，建立初始模型后能高度自动化预测与提交流程。

Numerai的延续性特性也使其更适合想为表格数据构建专用机器学习流水线的人群。

## 网络礼仪

任何上网超过15分钟的人都明白：讨论中无论话题多温和，都可能引发情绪化反应，使对话偏离文明范畴。Kaggle社区为此制定了行为准则：https://www.kaggle.com/community-guidelines

这些准则不仅适用于讨论，也涉及Notebook等交流形式。在Kaggle互动时需牢记以下要点：

- 切勿陷入斯科特·亚当斯所说的"读心术错觉"：Kaggle是由全球各地人士组成的极度多元化社区（对许多人而言英语并非母语），保持语义细微差别是巨大挑战。避免主观臆断，尽可能澄清沟通。

- 禁止人身攻击；戈德温法则的存在有其道理。特别是涉及受保护的不可变特征时，绝对属于禁区。

- 个人体验或有差异，但事实不变：这已非上世纪90年代互联网蛮荒时期，那时让人"去查手册"(RTFM)司空见惯；贬损言论易使人心生疏离。

- 严禁操纵晋级系统（Kaggle奖章授予基础）：该条款涵盖从公开索赞、共谋舞弊到彻底作弊等全谱系平台滥用行为。

简言之，己所不欲勿施于人，自可万事顺遂。

## 本章小结

本章探讨了Kaggle平台的主要交流方式——讨论论坛。我们演示了论坛运作机制，展示了如何在高阶竞赛中活用讨论的实例，并简要概述了讨论礼仪规范。

至此完成本书的第一部分导论内容。下一章将开始深入探索如何最大化Kaggle收益，着手应对竞赛中必须处理的各类任务与评估指标。

## 加入本书Discord空间

加入本书Discord工作区，每月参与作者问答专场：

https://packt.link/KaggleDiscord

## ——————第二部分—————— 竞赛技能精进

##

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_121.jpg?x=242&y=313&w=181&h=235&r=0"/>

<!-- Media -->

竞赛任务与评估指标

竞赛伊始需先研究目标指标。理解模型错误的评估方式，是每场竞赛取得高分的关键。当预测结果提交至Kaggle平台时，系统会根据目标指标将其与基准真相数据进行比对。

例如在泰坦尼克号竞赛(https://www.kaggle.com/c/titanic/)中，所有提交均按准确率（正确预测乘客生还的百分比）评估。组织方选择该指标，是因为竞赛目标是寻找能估算类似情境下乘客生还概率的模型。而在"房价预测-高级回归技术"(https://www.kaggle.com/c/house-prices-advanced-regression-techniques)竞赛中，评估标准则是预测值与真实值的平均差异，涉及对数运算、平方及开方处理，因为模型需要尽可能准确地量化待售房屋的价格排序。

现实数据科学中，目标指标同样是项目成功关键，尽管实际场景与Kaggle竞赛存在差异。简言之，现实世界更为复杂。实际项目中，模型常需面对多重评估指标，其中某些指标甚至与预测性能无关。例如专业领域知识、项目范围、模型特征数量、内存占用、特殊硬件需求（如GPU）、预测延迟、模型复杂度等因素，其重要性可能远超单纯预测性能。现实问题往往受商业和技术基础设施制约的程度，远超未涉足者的想象。

但核心原则始终如一：无论是实际项目还是Kaggle竞赛，你的工作都将根据特定标准被评估。深入理解这些标准细节、智能优化模型适配度、或依据标准选择参数，都将助你成功。若能在Kaggle中精通模型评估之道，现实数据科学工作亦将受益。

本章将详细阐述在某些类型问题中，评估指标如何深刻影响数据科学竞赛中构建模型解决方案的操作方式。我们同时探讨Kaggle竞赛中各类评估指标的多样性，帮助您理解最关键的因素，并在边缘讨论不同指标对预测性能的差异化影响及其在项目中的正确转化方法。本章涵盖以下主题：

- 评估指标与目标函数

- 基础任务类型：回归、分类与序数问题

- Meta Kaggle数据集

- 处理未见指标的方法

- 回归任务指标（标准型与序数型）

- 二分类指标（标签预测与概率）

- 多类别分类指标

- 目标检测问题指标

- 多标签分类与推荐问题指标

- 评估指标优化策略

## 评估指标与目标函数

在Kaggle竞赛中，您可在竞赛概述页面的左侧菜单找到评估指标。通过选择"评估"标签页，将获取关于评估指标的详细信息，包括可能出现的指标公式、复现代码及相关讨论。该页面还会说明提交文件格式，提供文件标题及示例行。评估指标与提交文件的关联至关重要，因为指标运算发生在模型训练完成并生成预测之后。因此首要步骤是理解评估指标与目标函数的区别。

从根本上说，目标函数在模型训练阶段发挥作用，参与误差最小化（或分数最大化，视问题类型而定）的过程；而评估指标则是在训练完成后为模型提供评分。因此评估指标虽不能直接影响模型拟合数据的方式，但能通过帮助选择最优超参数配置及最佳模型产生间接影响。在继续探讨该差异如何影响Kaggle竞赛、以及为何分析评估指标应作为竞赛首要步骤之前，我们先解析讨论区常见术语。

您会频繁听到目标函数、代价函数与损失函数被交替使用，但它们存在细微差别：

- 损失函数作用于单个数据点，根据模型预测值与真实值计算惩罚值

- 成本函数会考虑用于训练的整个数据集（或其批次），计算各数据点损失惩罚的总和或平均值。它可能包含其他约束条件，例如L1或L2惩罚项。成本函数直接影响训练过程。

- 目标函数是机器学习训练优化范畴中最通用（且安全）的术语：它包含成本函数，但不仅限于此。事实上，目标函数还能考虑与预测目标无关的其他目标：例如要求估计模型的系数具有稀疏性，或最小化系数值（如L1和L2正则化）。此外，损失函数和成本函数意味着基于最小化的优化，而目标函数是中性的，可能表示学习算法执行的最大化或最小化操作。

同理，在评估指标方面，你会遇到评分函数和误差函数。区分它们很简单：评分函数的值越大表示预测结果越好，意味着最大化过程；误差函数的值越小则预测越好，意味着最小化过程。

## 任务基本类型

并非所有目标函数都适用于所有问题。从广义上看，Kaggle竞赛主要包含两类问题：回归任务和分类任务。近期也出现了强化学习（RL）任务，但RL不使用评估指标，而是通过与其他假定性能相当的解决方案进行直接对决来生成排名（对决表现优于同行则排名上升，反之下降）。由于RL不涉及指标，我们将继续讨论回归-分类二分法，不过预测整数表示有序标签的序数任务可能超出这种分类范畴，既可采用回归也可用分类方法处理。

## 回归

回归任务需要构建能预测实数的模型（通常为正数，但也有负数预测案例）。经典案例是"房价-高级回归技术"竞赛，因为需要预测房屋价值。回归任务的评估涉及计算预测值与真实值之间的距离，可通过平方误差惩罚较大偏差，或采用对数尺度惩罚错误量级。

## 分类

Kaggle中的分类任务更具复杂性，可分为二分类、多类别分类和多标签分类。

二分类问题需要判断样本是否属于特定类别（通常称为正类，与负类相对）。评估可能直接预测类别归属，或估计归属概率。典型如泰坦尼克号竞赛需预测二元结果：生存/死亡。虽然统计正确匹配数量看似可行，但当正负类别样本数量不平衡时，这种方法会失效。基于类别不平衡分布的分类需要采用考虑失衡的评估指标，才能准确追踪模型改进。

超过两个类别时即多类别预测问题，需使用特定评估函数跟踪模型整体性能，并确保各类别性能可比（例如某些类别可能存在欠拟合）。每个样本仅属于唯一类别，典型案例是叶片分类竞赛，需要将叶片图像对应到正确植物物种。

当类别预测非互斥且每个样本可预测多个类别时，即为多标签问题，需额外评估模型是否能预测正确类别及其数量组合。例如在希腊媒体多标签分类竞赛中，需将每篇文章与其涉及的所有主题相关联。

## 序数尺度

在处理序数尺度预测问题时，需要预测具有自然顺序的整数标签。例如地震震级就属于序数尺度。此外，市场调研问卷数据也常采用序数尺度记录（如消费者偏好或意见认同度）。由于序数尺度由有序数值构成，这类任务可视为回归与分类的中间形态，可通过两种方式解决。

最常见的方法是将其视为多分类问题。此时虽能获得整数值（类别标签）的预测，但模型不会考虑类别间的顺序关系。观察各类别的预测概率分布时，常会发现概率值分散在所有可能取值上，呈现多峰且非对称的分布（理论上应呈现以最大概率类别为中心的正态分布），这暗示了多分类方法的局限性。

另一种解决思路是将其视为回归问题后进行后处理。这种方法能考虑类别顺序，但原始回归输出（浮点数而非序数类别整数）不能直接用于评估指标。通过截断输出值并进行单位舍入虽可转换，但可能引入误差，需要更复杂的后处理（本章后续将详细讨论）。

要在Kaggle比赛中获胜，必须精通竞赛指定的评估指标。不过某些指标更为常见，掌握这些指标能带来优势。如何快速了解高频指标？如何借鉴使用相似评估指标的往期比赛经验？答案是利用Meta Kaggle数据集。

## Meta Kaggle数据集

Meta Kaggle数据集(https://www.kaggle.com/kaggle/meta-kaggle)是Kaggle官方发布的社区活动数据集合，包含竞赛、数据集、笔记本和讨论区的公开记录。只需创建Kaggle笔记本（如第2、3章所述），加载该数据集即可开始分析。这些CSV表格每日更新，虽需定期刷新分析结果，但其蕴含的洞察价值非凡。

本书将多次引用Meta Kaggle数据集，既为展示竞赛动态的典型案例，也为提炼学习策略的实用范例。此处我们将用它统计近七年竞赛中最常用的评估指标。通过本章学习，你能夯实基础快速投入新比赛，再结合论坛讨论掌握特定指标的细微差别。下文代码可直接在Kaggle平台运行，用于生成按年度统计的指标频率表：

---

import numpy as np

导入 pandas 库并简写为 pd

comps = pd.read_csv("/kaggle/input/meta-kaggle/Competitions.csv")

评估指标 = ['评估算法缩写',

'评估算法名称',

'评估算法描述']

竞赛字段 = ['标题', '启用日期', '主办方类别']

df = comps[竞赛字段 + 评估指标].copy(   )

df['年份'] = pd.to_datetime(df.启用日期).dt.year.values

df['竞赛数'] = 1

时间筛选 = df.年份 >= 2015

竞赛类型筛选 = df.主办方类别.isin(   )

['精选', '研究'])

pd.pivot_table(df[时间筛选&竞赛类型筛选],

values='竞赛数',

index=['评估算法缩写'],

columns=['年份'],

填充值=0.0,

聚合函数=np求和,

显示总计=True

).排序值(   )

按=('总计'), 升序=False).行切片[1:,:].头部(20)

---

本代码中，我们读取包含竞赛相关数据的CSV表格，重点关注代表评估指标的列以及记录竞赛名称、开始日期和类型的列。我们将数据限定为2015年后举办且类型为Featured或Research（最常见类型）的竞赛。通过创建pandas数据透视表，将评估算法与年份结合，并统计使用该算法的竞赛数量来完成分析。仅显示前20个算法。

<!-- Media -->

以下是生成的结果表（截至撰写时）：

<table><tbody><tr><td>年份</td><td rowspan="2">2015</td><td rowspan="2">2016</td><td rowspan="2">2017</td><td rowspan="2">2018</td><td rowspan="2">2019</td><td rowspan="2">2020</td><td rowspan="2">2021</td><td rowspan="2">总计</td></tr><tr><td>评估算法</td></tr><tr><td>AUC（曲线下面积）</td><td>4</td><td>4</td><td>1</td><td>3</td><td>3</td><td>2</td><td>0</td><td>17</td></tr><tr><td>对数损失</td><td>2</td><td>2</td><td>5</td><td>2</td><td>3</td><td>2</td><td>0</td><td>16</td></tr><tr><td>平均准确率@\{K\}</td><td>1</td><td>3</td><td>0</td><td>4</td><td>1</td><td>0</td><td>1</td><td>10</td></tr><tr><td>分类准确率</td><td>1</td><td>0</td><td>4</td><td>0</td><td>1</td><td>2</td><td>0</td><td>8</td></tr><tr><td>多类别损失</td><td>2</td><td>3</td><td>2</td><td>0</td><td>1</td><td>0</td><td>0</td><td>8</td></tr><tr><td>均方根对数误差</td><td>2</td><td>1</td><td>3</td><td>1</td><td>1</td><td>0</td><td>0</td><td>8</td></tr><tr><td>二次加权卡帕系数</td><td>3</td><td>0</td><td>0</td><td>1</td><td>2</td><td>1</td><td>0</td><td>7</td></tr><tr><td>平均F分数Beta</td><td>1</td><td>0</td><td>1</td><td>2</td><td>1</td><td>2</td><td>0</td><td>7</td></tr><tr><td>K最佳误差均值</td><td>0</td><td>0</td><td>2</td><td>2</td><td>1</td><td>1</td><td>0</td><td>6</td></tr><tr><td>多类别均方根对数误差</td><td>0</td><td>0</td><td>1</td><td>0</td><td>0</td><td>5</td><td>0</td><td>6</td></tr><tr><td>多类别AUC</td><td>1</td><td>0</td><td>1</td><td>0</td><td>0</td><td>3</td><td>0</td><td>5</td></tr><tr><td>均方根误差</td><td>1</td><td>1</td><td>0</td><td>3</td><td>0</td><td>0</td><td>0</td><td>5</td></tr><tr><td>Dice系数</td><td>0</td><td>1</td><td>1</td><td>0</td><td>2</td><td>1</td><td>0</td><td>5</td></tr><tr><td>谷歌全局平均精度</td><td>0</td><td>0</td><td>1</td><td>2</td><td>1</td><td>1</td><td>0</td><td>5</td></tr><tr><td>宏平均F分数</td><td>0</td><td>0</td><td>0</td><td>1</td><td>0</td><td>2</td><td>1</td><td>4</td></tr><tr><td>得分</td><td>0</td><td>0</td><td>3</td><td>0</td><td>0</td><td>0</td><td>0</td><td>3</td></tr><tr><td>连续分级概率评分</td><td>2</td><td>0</td><td>0</td><td>0</td><td>1</td><td>0</td><td>0</td><td>3</td></tr><tr><td>OpenImages目标检测平均精度</td><td>0</td><td>0</td><td>0</td><td>1</td><td>1</td><td>1</td><td>0</td><td>3</td></tr><tr><td>平均F分数</td><td>0</td><td>0</td><td>1</td><td>0</td><td>0</td><td>0</td><td>2</td><td>3</td></tr><tr><td>RSNA目标检测平均精度</td><td>0</td><td>0</td><td>0</td><td>1</td><td>0</td><td>1</td><td>0</td><td>2</td></tr></tbody></table>

<!-- Media -->

利用我们刚才实例化的相同变量来生成表格，您还可以检查数据以找出采用了所选指标的竞赛：

---

metric = 'AUC'

metric_select = df['EvaluationAlgorithmAbbreviation']==metric

print(df[time_select&competition_type_select&metric_select]

[['Title', 'year']])

---

上述代码片段展示了采用AUC指标的竞赛。只需修改代表所选指标的字符串，结果列表将相应更新。回到生成的表格，我们可以研究Kaggle竞赛中最常用的评估指标：

- 前两名指标密切相关且均针对二分类概率问题。AUC指标用于衡量模型预测阳性案例的概率倾向，而Log Loss则衡量预测概率与真实值的偏差程度（优化Log Loss的同时也会优化AUC指标）。

- 第\( {3}^{\text{rd }} \)位是MAP@\( \{ \mathrm{K}\} \)，这是推荐系统和搜索引擎的常用指标。在Kaggle竞赛中，该指标主要用于信息检索评估，例如座头鲸识别竞赛（https://www.kaggle.com/c/humpback-whale-identification）要求从五个猜测中精确识别鲸鱼；Quick, Draw!涂鸦识别挑战赛（https://www.kaggle.com/c/quickdraw-doodle-recognition/）允许三次尝试猜测草图内容。本质上，当\( \operatorname{MAP}@\{ K\} \)作为评估指标时，只要正确猜测位于函数名中"\( \mathrm{K} \)"指定的错误预测数量范围内，即可得分。

- 仅在\( {6}^{\text{th }} \)位出现回归指标RMSLE（均方根对数误差），\( {7}^{\text{th }} \)位则是适用于序数尺度问题的二次加权Kappa系数。

浏览顶级指标列表时，您会不断发现机器学习教材中常讨论的指标。接下来几节中，我们将先探讨遇到未见过的指标时的应对策略（这在Kaggle竞赛中比预期更常见），然后回顾回归和分类竞赛中最常见的指标。

## 处理未见过的指标

首先需注意，前20名表格并未涵盖所有竞赛指标。近年来有些指标仅被使用过一次。

让我们继续使用之前代码的结果来找出这些指标：

---

counts = (df[time_select&competition_type_select]

.groupby('EvaluationAlgorithmAbbreviation'))

total_comps_per_year = (df[time_select&competition_type_select]

.groupby('年份').sum(   ))

年度单一指标 = (counts.sum(   )[counts.sum(   ).竞赛数==1]

.groupby('年份').sum(   ))

年度单一指标

数据表 = (年度总竞赛数.rename(columns=\{'竞赛数': '总竞赛数'\})

.join(年度单一指标 / 年度总竞赛数)

.rename(columns=\{'竞赛数': '占比'\}))

打印(数据表)

---

最终我们得到这张表格，按年份显示：有多少竞赛使用了后来再未出现的指标（总竞赛数），以及这类竞赛占当年竞赛的比例（占比）：

<!-- Media -->

<!-- figureText: year 2015 28 0.179 2016 19 0.158 2017 34 0.177 2018 35 0.229 2019 36 0.278 2020 43 0.302 2021 8 0.250 -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_130.jpg?x=247&y=1043&w=1396&h=476&r=0"/>

<!-- Media -->

观察这些使用"昙花一现"指标的竞赛占比，我们明显发现其逐年增长的趋势——近年来已达到25%-30%的水平，这意味着平均每三到四个竞赛中就有一个要求参赛者从零开始研究理解新指标。

通过简单代码即可获取历史上出现过的这类指标列表：

---

打印(counts.sum(   )[counts.sum(   ).竞赛数==1].index.values)

---

<!-- Media -->

执行代码后将获得类似这样的列表：['AHD@{Type}' 'CVPRAutoDrivingAveragePrecision' 'CernWeightedAuc' 'FScore_1' 'GroupMeanLogMAE' 'ImageNetObjectLocalization' 'IndoorLocalization' 'IntersectionOverUnionObjectSegmentationBeta' 'IntersectionOverUnionObjectSegmentationWithClassification' 'IntersectionOverUnionObjectSegmentationWithF1' 'Jaccard' 'JaccardDSTLParallel' 'JigsawBiasAUC' 'LaplaceLogLikelihood' 'LevenshteinMean' 'Lyft3DObjectDetectionAP' 'M5_WRMSSE' 'MASpearmanR' 'MCRMSE' 'MCSpearmanR' 'MWCRMSE' 'MeanColumnwiseLogLoss' 'MulticlassLossOld' 'NDCG@{K}' 'NQMicroF1' 'NWRMSLE' 'PKUAutoDrivingAP' 'R2Score' 'RValue' 'RootMeanSquarePercentageError' 'SIIMDice' 'SMAPE' 'SantaResident' 'SantaRideShare' 'SantaWorkshopSchedule2019' 'TrackML' 'TravelingSanta2' 'TwoSigmaNews' 'WeightedAUC' 'WeightedMulticlassLoss' 'WeightedPinballLoss' 'WeightedRowwisePinballLoss' 'YT8M_MeanAveragePrecisionAtK' 'ZillowMAE' 'football' 'halite' 'mab']

仔细检视可以发现，许多指标与深度学习和强化学习竞赛相关

<!-- Media -->

。

当遇到从未见过的新指标时该怎么办？当然可以依靠Kaggle讨论区的交流，那里总能获得灵感和热心用户的帮助。但若想建立自己的知识体系，除了谷歌搜索外，我们建议通过编写评估函数进行实验——哪怕方式不够完美，模拟该指标对模型各类错误的反应。也可以直接在竞赛训练数据样本或自制的合成数据上测试其功能。以下是Kaggle用户采用此方法的几个实例：

- Carlo Lepelaars关于斯皮尔曼等级相关系数(Spearman's Rho)的解析：https://www.kaggle.com/carlolepelaars/understanding-the-metric-spearman-s-rho

- Carlo Lepelaars关于二次加权卡帕系数(Quadratic Weighted Kappa)的解析：https://www.kaggle.com/carlolepelaars/understanding-the-metric-quadratic-weighted-kappa

- Rohan Rao关于拉普拉斯对数似然(Laplace Log Likelihood)的解析：https://www.kaggle.com/rohanrao/osic-understanding-laplace-log-likelihood

这将使您更深入地理解评估标准，相比仅依赖谷歌搜索和Kaggle论坛答案的竞争对手更具优势。

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_132.jpg?x=246&y=237&w=350&h=353&r=0"/>

<!-- Media -->

## Rohan Rao专访

https://www.kaggle.com/rohanrao

在探讨不同评估指标之前，让我们先听听四重特级大师、H20.ai高级数据科学家Rohan Rao（又名Vopani）分享他在Kaggle的成功经验与智慧。

## 您最青睐哪类竞赛？为什么？在技术方法和解决思路上，您在Kaggle的专长是什么？

我喜欢尝试各类竞赛，但最钟情的当属时间序列比赛。我对工业界常规的时间序列处理方式不太认同，因此常以非传统方法构建解决方案，这种创新思维最终为我带来了巨大成功。

## 您如何规划Kaggle竞赛策略？这与日常工作方法有何不同？

对于任何Kaggle竞赛，我的标准工作流程如下：

- 理解问题陈述，研读所有关于规则、格式、时间线、数据集、评估指标和交付成果的说明

- 深度分析数据。多维度拆解数据并通过探索性分析可视化，确保能解答任何相关疑问

- 建立包含基线模型的简易流程，提交结果以验证流程有效性

- 进行特征工程、超参数调优，通过多模型实验判断有效方案

- 持续回溯数据分析，研讨论坛观点，极致优化特征与模型。适时组建团队

- 集成多模型结果，确定最终提交版本

在我的数据科学日常工作中，大部分情况也是如此。但还有两个额外不可或缺的关键要素：

- 根据问题陈述筛选和准备数据集

- 将最终模型或解决方案部署到生产环境

过去参与的大部分项目中，我的时间主要都投入在这两项工作上。

## Kaggle对你的职业发展有帮助吗？具体体现在哪些方面？

我在机器学习领域的知识几乎都源自Kaggle。这个社区、平台及其内容堪称无价之宝，你能从中汲取海量知识。

对我助益最大的是参加Kaggle竞赛的经历，这让我在跨领域理解、架构和解决问题方面建立了强大信心，这些能力已成功应用于我在Kaggle之外的多个企业和项目。

许多招聘方因看到我在\( {myKaggle} \)竞赛中的成就而联系我。这能有效证明候选人解决数据科学问题的能力，因此是展示技能和构建作品集的绝佳平台。

## 你在过往竞赛中犯过哪些错误？

每场比赛我都会犯错！这正是学习和进步的方式。有时是代码漏洞，有时是验证设置缺陷，有时是错误提交选择！

关键是从中吸取教训避免重蹈覆辙。这个迭代过程自然能提升你在Kaggle的整体表现。

## 有哪些特别推荐的数据分析/机器学习工具或库？

我坚信不该固守某项技术。选择最高效趁手的工具，同时保持学习新工具库的开放心态。

## 回归问题的评估指标（标准与序数）

处理回归问题（即预测从负无穷到正无穷连续值的问题）时，最常用的误差指标是均方根误差(RMSE)和平均绝对误差(MAE)，但相对对数均方根误差(RMSLE)或修正均方根误差(MCRMSLE)等变体指标也可能适用。

## 均方误差(MSE)与R平方

均方根误差是均方误差(MSE)的平方根，而MSE正是您在回归分析中学过的经典误差平方和(SSE)的平均值。其计算公式如下：

\[{MSE} = \frac{1}{n}{SSE} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{\left( \widehat{{y}_{i}} - {y}_{i}\right) }^{2}\]

首先解析公式原理：\( n \)表示样本数量，\( {y}_{i} \)代表真实值，\( {\widehat{y}}_{\iota } \)为预测值。先计算预测值与真实值的差值，平方后求和得到SSE，再除以预测次数即得MSE。通常回归模型都会最小化SSE，因此最小化MSE或其派生指标（如决定系数R平方）也不成问题，R平方公式为：

\[{R}^{2} = \frac{SSE}{SST} = \mathop{\sum }\limits_{{i = 1}}^{n}\frac{{\left( {\widehat{y}}_{i} - {y}_{i}\right) }^{2}}{{\left( {y}_{i} - \bar{y}\right) }^{2}}\]

此处将SSE（误差平方和）与总平方和(SST)比较，后者即响应变量的方差。统计中SST定义为目标值与其均值的平方差：

\[{SST} = \mathop{\sum }\limits_{{i = 1}}^{n}{\left( {y}_{i} - \bar{y}\right) }^{2}\]

换言之，R平方将模型误差与最简模型（响应变量均值）的误差进行对比。由于SSE和SST量纲相同，R平方可帮助判断目标变量变换是否能改善预测效果。

请注意：minmax标准化或Z-score标准化等线性变换不会改变回归器性能（因其属于目标变量的线性变换）。而非线性变换（如平方根、立方根、对数、指数及其组合）则能显著改变模型在评估指标上的表现（若选择得当可提升效果）。MSE是横向比较同问题回归模型的利器，但Kaggle竞赛中更常用RMSE——取平方根后其值更接近目标变量原量纲，便于直观评估模型表现。当跨数据集比较时，R平方更优：其与MSE完全相关且取值在0-1之间，更便于比较。

## 均方根误差(RMSE)

RMSE即MSE的平方根，但蕴含微妙差异。其公式为：

\[{RMSE} = \sqrt{\mathop{\sum }\limits_{{i = 1}}^{n}\frac{{\left( {\widehat{y}}_{i} - {y}_{i}\right) }^{2}}{n}}\]

公式中\( n \)为样本数，\( {y}_{i} \)是真实值，\( {\widehat{y}}_{l} \)为预测值。MSE因平方运算会放大较大误差，而RMSE通过开方减弱这种效应（但异常值仍需警惕，无论使用MSE还是RMSE评估，它们都会显著影响模型表现）。

因此针对特定问题，可先对目标变量取平方根（需正值），再用MSE作为目标函数进行拟合。Scikit-learn的TransformedTargetRegressor能自动完成这种变换，使模型更适配评估指标。

近期使用RMSE的竞赛包括：

- Avito需求预测挑战赛：https://www.kaggle.com/c/avito-demand-prediction

- 谷歌分析客户收入预测：https://www.kaggle.com/c/ga-customer-revenue-prediction

- Elo商家类别推荐：https://www.kaggle.com/c/elo-merchant-category-recommendation

## 均方根对数误差(RMSLE)

MSE另一常见变体是均方根对数误差(RMSLE)。MCRMSLE则是COVID-19预测竞赛推广的多目标评估指标，即各目标RMSLE的列向平均值。RMSLE公式如下：

\[{RMSLE} = \sqrt{\frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}{\left( \log \left( {\widehat{y}}_{i} + 1\right)  - \log \left( {y}_{i} + 1\right) \right) }^{2}}\]

在该公式中，\( n \)表示案例数量，\( {y}_{i} \)代表真实值，\( {\widehat{y}}_{i} \)为预测值。由于在对预测值和真实值进行平方、平均及开方运算前先进行了对数转换，因此不会对预测值与实际值之间的巨大差异（尤其是两者均为大数值时）施加过度惩罚。换言之，使用RMSLE时最关注的是预测值相对于真实值的量级关系。与RMSE类似，若在拟合前对目标变量进行对数转换（随后通过指数函数还原效果），回归类机器学习算法能更好地优化RMSLE指标。

近期采用RMSLE作为评估指标的竞赛包括：

- ASHRAE能源预测大赛III：https://www.kaggle.com/c/ashrae-energy-prediction

- 桑坦德银行价值预测挑战赛：https://www.kaggle.com/c/ santander-value-prediction-challenge

- Mercari商品价格建议挑战赛：https://www.kaggle.com/c/mercari-price-suggestion-challenge

- 俄罗斯联邦储蓄银行住房市场分析：https://www.kaggle.com/ olgabelitskaya/sberbank-russian-housing-market

- Recruit餐厅客流量预测：https://www.kaggle.com/c/ recruit-restaurant-visitor-forecasting

截至目前，RMSLE仍是Kaggle竞赛中最常用的回归评估指标。

## 平均绝对误差(MAE)

MAE（平均绝对误差）评估指标是预测值与目标值之差的绝对值。其计算公式如下：

\[{MAE} = \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}\left| {{\widehat{y}}_{i} - {y}_{i}}\right| \]

公式中\( n \)代表案例数量，\( {y}_{i} \)为真实值，\( {\widehat{y}}_{i} \)为预测值。MAE对异常值不敏感（不同于平方误差的MSE），因此在包含异常值数据集的竞赛中常见此评估指标。此外，许多算法可直接将其作为目标函数使用；也可通过对目标变量取平方根训练后对预测值平方，间接优化该指标。

MAE作为目标函数的缺陷在于收敛速度较慢——因其实际优化的是目标变量的中位数（L1范数）而非均值（L2范数），这导致优化器计算复杂度增加，训练时间可能随训练案例数量呈指数级增长（参见Stack Overflow讨论：https:// stackoverflow.com/questions/57243267/why-is-training-a-random-forest-regressor-with-mae-criterion-so-slow-compared-to）。

近期采用MAE评估指标的知名竞赛包括：

- LANL地震预测：https://www.kaggle.com/c/LANL-Earthquake-Prediction

- 降水量预测II：https://www.kaggle.com/c/how-much-did-it-rain-ii

前文提及ASHRAE竞赛时，需说明回归评估指标与预测类竞赛密切相关。例如近期举办的M5预测大赛（https://mofc.unic.ac.cy/m5-competition/）及其它M系列竞赛数据均开放获取。对预测类竞赛感兴趣者可参阅https://robjhyndman.com/hyndsight/forecasting-competitions/了解M系列竞赛概况及Kaggle对提升实践与理论成果的价值。本质上，预测竞赛的评估方式与回归竞赛差异不大，虽会出现加权均方根缩放误差（https://www.kaggle.com/c/m5-forecasting-accuracy/overview/evaluation）或对称平均绝对百分比误差（sMAPE，https://www.kaggle.com/c/demand-forecasting-kernels-only/overview/evaluation）等特殊指标，但这些均可视为RMSE或MAE的变体，通过适当的目标变量转换即可处理。

## 分类指标（标签预测与概率）

在探讨完回归问题的评估指标后，我们现在将阐述分类问题的度量标准——从二分类问题（需在两个类别间进行预测）开始，延伸到多分类问题（存在两个以上类别），再到多标签分类（类别存在重叠的情况）。

## 准确率

分析二分类器性能时，最常用且直观的指标是准确率。当模型对样本做出错误类别预测时，称为误分类错误。准确率即是误分类错误的补集，计算公式为正确预测数量与总预测数量的比值：

\[\text{ Accuracy } = \frac{\text{ correct answers }}{\text{ total answers }}\]

该指标曾应用于木薯叶病害分类（https://www.kaggle.com/c/cassava-leaf-disease-classification）和英语文本规范化挑战赛（https://www.kaggle.com/c/text-normalization-challenge-english-language），这些场景中仅当预测文本与实际字符串完全匹配时才计为正确预测。

作为指标，准确率强烈聚焦于模型在真实场景中的有效性能：它能告诉你模型是否如预期工作。但若目的是评估比较并清晰了解方法的真实有效性，使用准确率时需格外谨慎——当类别不平衡（频率差异显著）时可能导致错误结论。例如某类别仅占数据10%，仅预测多数类的分类器就能达到90%准确率，这种高准确率实则毫无用处。如何识别此类问题？通过混淆矩阵可轻松实现：该双向表格将真实类别（行）与预测类别（列）进行对比，使用Scikit-learn的confusion_matrix函数即可生成基础矩阵：

---

sklearn.metrics.confusion_matrix(   )

y_true, y_pred, *, labels=None, sample_weight=None,

normalize=None

)

---

提供y_true和y_pred向量即可生成有效表格，亦可添加行列标签、样本权重，并选择对真实样本（行）、预测样本（列）或全体样本进行归一化（使边际总和为1）。完美分类器的矩阵主对角线将包含全部案例，若对角线单元格出现空或少量案例，则预示预测器存在严重效度问题。

为更好理解其工作原理，可参考Scikit-learn提供的图形示例（https://scikit-learn.org/stable/auto_examples/model_selection/plot_confusion_matrix.html#sphx-glr-auto-examples-model-selection-plot-confusion-matrix-py）。虽然可通过计算各类别相对准确率并取平均值来提升指标实用性，但更推荐使用精确率、召回率和F1分数等其他指标。

<!-- Media -->

<!-- figureText: setosa 1.00 0.00 0.00 0.62 0.38 0.00 1.00 versicolor virginica Predicted label True label versicolor 0.00 virginica 0.00 setosa -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_139.jpg?x=525&y=1241&w=819&h=750&r=0"/>

图5.1：混淆矩阵（各单元格归一化为1.00以表示匹配占比）

<!-- Media -->

## 精确率与召回率

要计算精确率和召回率，我们再次从混淆矩阵出发。首先需为矩阵各单元格命名，定义方式如下：

<!-- Media -->

<table><tbody><tr><td colspan="2" rowspan="2"></td><td colspan="2">预测值</td></tr><tr><td>阴性</td><td>阳性</td></tr><tr><td rowspan="2">实际值</td><td>阴性</td><td>真阴性</td><td>假阳性</td></tr><tr><td>阳性</td><td>假阴性</td><td>真阳性</td></tr></tbody></table>

表5.1：带有单元格名称的混淆矩阵

<!-- Media -->

- TP（真阳性）：位于左上角单元格，包含被正确预测为阳性的样本。

- FP（假阳性）：位于右上角单元格，包含被预测为阳性但实际为阴性的样本。

- FN（假阴性）：位于左下角单元格，包含被预测为阴性但实际为阳性的样本。

- TN（真阴性）：位于右下角单元格，包含被正确预测为阴性的样本。

利用这些单元格，您可以更精确地了解分类器的工作机制及优化模型的方法。首先，我们可以轻松修正准确率公式：

\[\text{ Accuracy } = \frac{\left( TP + TN\right) }{\left( TP + TN + FP + FN\right) }\]

第一个关键指标称为精确率（或称特异度），它本质上是阳性案例的准确率：

\[\text{ Precision } = \frac{TP}{{TP} + {FP}}\]

计算时仅涉及真阳性数和假阳性数。该指标实质上反映了当预测为阳性时的正确频率。

显然，模型可以通过仅对高置信度样本预测阳性来获得高分。这正是该指标的初衷：迫使模型仅在确信且安全的情况下才预测阳性类别。

但若需尽可能多地预测阳性案例，则还需关注召回率（或称覆盖率/敏感度/真阳性率）：

\[\text{ Recall } = \frac{TP}{{TP} + {FN}}\]

此时还需考虑假阴性。这两个指标的微妙之处在于：由于它们基于样本分类（而分类本质是基于概率，通常以0.5为阈值划分正负类），调整阈值会以牺牲其中一个指标为代价提升另一个。

例如提高阈值会提升精确率（分类器预测更确信）但降低召回率；降低阈值则效果相反。这种现象称为精确率-召回率权衡。Scikit-learn官网对此有简明实用的解读（https://scikit-learn.org/stable/auto_examples/model_selection/plot_precision_recall.html），通过绘制PR曲线帮助理解如何平衡这两个指标以获得理想结果：

<!-- Media -->

<!-- figureText: Recall (positive label) -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_142.jpg?x=252&y=439&w=1375&h=950&r=0"/>

图5.2：具有阶梯特征的双类别精确率-召回率曲线

<!-- Media -->

与PR权衡相关的指标是平均精确率（Average Precision），它计算召回率从0到1时的平均精确率（本质是阈值从1到0变化时的均值）。该指标在目标检测任务中广受欢迎（后文将讨论），对表格数据分类也极具价值。当需要更精准地监测模型在稀有类别（数据极度不平衡时，如欺诈检测场景）的表现时尤为实用。

详见Gael Varoquaux的论述：http://gael-varoquaux.info/interpreting_ml_tuto/content/01_how_well/01_metrics.html#average-precision

## F1分数

至此，您可能已经意识到仅使用精确率(precision)或召回率(recall)作为评估指标并非理想选择，因为优化其中一个指标必然以牺牲另一个为代价。因此，Kaggle竞赛从不单独使用这两个指标，而是采用组合指标（如平均精确率）。F1分数作为精确率和召回率的调和平均数，被广泛认为是最佳解决方案：

\[{F1} = 2 * \frac{\text{ precision } * \text{ recall }}{\text{ precision } + \text{ recall }}\]

若\( {F1} \)分数较高，说明模型在精确率或召回率或两者上均有提升。Quora虚假问题分类竞赛(https://www.kaggle.com/c/quora-insincere-questions-classification)提供了该指标的经典应用案例。

部分竞赛会采用F-beta分数，这是精确率与召回率的加权调和平均数，其中beta参数决定召回率在综合分数中的权重：

\[{F}_{\beta } = \frac{\left( {1 + {\beta }^{2}}\right)  * \left( {\text{ precision } * \text{ recall }}\right) }{\left( {\beta }^{2} * \text{ precision } + \text{ recall }\right) }\]

既然已介绍过阈值和分类概率的概念，现在可以探讨两种常见分类指标：对数损失(log loss)和ROC-AUC。

## 对数损失与ROC-AUC

首先介绍对数损失（深度学习模型中称为交叉熵）。\( \log \)损失衡量预测概率与真实概率之间的差异：

\[\operatorname{LogLoss} =  - \frac{1}{n}\mathop{\sum }\limits_{{i = 1}}^{n}\left\lbrack  {{y}_{i}\log \left( {\widehat{y}}_{i}\right)  + \left( {1 - {y}_{i}}\right) \log \left( {1 - {\widehat{y}}_{i}}\right) }\right\rbrack  \]

公式中\( n \)表示样本数量，\( {y}_{i} \)代表第\( {i}^{\text{th }} \)个样本的真实标签，\( \widehat{{y}_{l}} \)为预测值。

采用对数损失的竞赛意味着核心目标是尽可能准确地估计样本属于正类的概率。该指标在众多竞赛中广泛应用。

例如可参考近期举办的Deepfake检测挑战赛(https://www.kaggle.com/c/deepfake-detection-challenge)或较早的Quora问题对竞赛(https://www.kaggle.com/c/quora-question-pairs)。

ROC曲线（接收者操作特征曲线）是评估二分类器性能及比较不同分类器的图示工具，也是ROC-AUC指标的基础——该指标即ROC曲线下面积。ROC曲线以真正例率（召回率）为纵轴，假正例率（被误判为正例的负例比例）为横轴绘制，其数值等于1减去真负例率（正确识别的负例比例）。示例如下：

<!-- Media -->

<!-- figureText: 100% 100% True positive rate AUC=50% 0% False positive rate 100% 100% True positive rate AUC=65% 0% False positive rate 100% True positive rate AUC=100% 0% False positive rate 100% 100% True positive rate AUC=90% 0% False positive rate 100% -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_144.jpg?x=237&y=616&w=1390&h=1177&r=0"/>

图5.3：不同ROC曲线及其AUC值

<!-- Media -->

理想情况下，优秀分类器的ROC曲线应在假正例率较低时快速爬升真正例率（召回率）。ROC-AUC值在0.9至1.0区间视为极佳。劣质分类器的ROC曲线会接近图表对角线（如左上图所示），代表与随机分类器相当的性能——接近0.5的ROC-AUC分数意味着预测结果近乎随机。当比较不同分类器时，曲线下面积(AUC)越大者性能越优。

当类别平衡或轻度不平衡时，AUC提升与模型效果成正比，可直观理解为模型对正例输出更高概率的能力，也可视为样本从正到负的排序能力。但当正类样本稀少时，初始高AUC值的微小提升可能对稀有类预测改善有限，此时平均精确率是更有效的指标。

近期多项竞赛采用AUC指标，推荐参考以下三例：

- IEEE-CIS欺诈检测：https://www.kaggle.com/c/ieee-fraud-detection

- Riiid答题正确率预测：https://www.kaggle.com/c/riiid-test-answer-prediction

- Jigsaw多语言毒性评论分类挑战赛：https://www.kaggle.com/c/jigsaw-multilingual-toxic-comment-classification/

您可在以下论文中查阅详细论述：苏伟、袁野、朱明。《平均精确率与ROC曲线下面积的关系》。《2015年国际信息检索理论会议论文集》。2015年。

## 马修斯相关系数(MCC)

我们以马修斯相关系数(MCC)作为二元分类指标的综述收尾，该指标曾出现在VSB输电线故障检测(https://www.kaggle.com/c/vsb-power-line-fault-detection)和博世生产线效能(https://www.kaggle.com/c/bosch-production-line-performance)竞赛中。

MCC的计算公式为：

\[{MCC} = \frac{\left( {{TP} * {TN}}\right)  - \left( {{FP} * {FN}}\right) }{\sqrt{\left( {{TP} + {FP}}\right)  * \left( {{TP} + {FN}}\right)  * \left( {{TN} + {FP}}\right)  * \left( {{TN} + {FN}}\right) }}\]

上述公式中，\( {TP} \)代表真正例，\( {TN} \)代表真负例，\( {FP} \)代表假正例，\( {FN} \)代表假负例。这与我们讨论精确率和召回率时使用的术语体系一致。

作为相关系数，该指标取值区间为+1(完美预测)到-1(完全反向预测)，即使在类别严重不平衡时，仍可视为分类质量的可靠度量。

尽管公式复杂，但如Neuron Engineer(https://www.kaggle.com/ratthachat)在其笔记中演示的：www.kaggle.com/ratthachat/demythifying-matthew-correlation-coefficients-mcc，该公式可被重构简化。

Neuron Engineer对评估指标比率的解析工作堪称典范。经其重构后的MCC公式变为：

\[{MCC} = \left( {{\text{ Pos }}_{\text{precision }} + {\text{ Neg }}_{\text{precision }} - 1}\right)  * \text{ PosNegRatio }\]

公式中各元素定义如下：

\[{\text{ Pos }}_{\text{precision }} = \frac{TP}{{TP} + {FP}}\]

\[{\text{ Neg }}_{\text{precision }} = \frac{TN}{{TN} + {FN}}\]

\[\text{ PosNegRatio } = \sqrt{\frac{\text{ PosPredictionCount } * \text{ NegPredictionCoun }}{\text{ PosLabelCount } * \text{ NegLabelCount }}}\]

\[\text{PosPredictionCount} = {TP} + {FP}\]

\[\text{NegPredictionCount} = {TN} + {FN}\]

重构公式以比原式更清晰的方式阐明：仅提升正负类精确率不足以保证高性能，预测结果还必须与真实分布保持比例一致，否则将遭受严重惩罚。

## 多类别分类指标

处理多类别分类时，只需将前述二元分类指标分别应用于每个类别，再通过常用聚合策略进行汇总。例如基于\( {F1} \)分数评估方案时，有三种平均策略可选：

- 宏平均：分别计算每个类别的\( {F1} \)分数后取算术平均。该方法平等对待所有类别，无论其正例频率或重要性，因此模型在任何类别表现不佳时都将受到同等惩罚。

\[\text{macro} = \frac{F{1}_{\text{class }1} + F{1}_{\text{class }2} + \cdots  + F{1}_{\text{class }N}}{N}\]

- 微平均：汇总所有类别的贡献计算综合\( {F1} \)分数。由于计算过程忽略类别差异，不会特别偏袒或惩罚任何类别，能更准确反映类别不平衡情况。

\[\text{ micro } = F{1}_{\text{class }1 + \text{ class }2 + \cdots \text{ class }N}\]

- 加权平均：类似宏平均先计算各类别\( {F1} \)分数，但采用基于类别真实标签数量的加权平均。通过权重设置，可体现各类别正例频率或问题相关性，该方法明显有利于占多数的类别。

\[\text{weighted} = F{1}_{\text{class1 }} * {W}_{1} + F{1}_{\text{class2 }} * {W}_{2} + \cdots  + F{1}_{\text{classN }} * {W}_{n}\]

\[{W}_{1} + {W}_{2} + \cdots  + {W}_{N} = {1.0}\]

在Kaggle竞赛中常见的多分类评估指标包括：

- 多分类准确率（加权）：孟加拉语AI手写字符分类（https://www.kaggle.com/c/bengaliai-cv19）

- 多分类对数损失（MeanColumnwiseLogLoss）：作用机制预测（https://www.kaggle.com/c/lish-moa/）

- 宏平均F1与微平均F1（NQMicroF1）：利物浦大学离子通道研究（https://www.kaggle.com/c/liverpool-ion-switching）、人类蛋白质图谱图像分类（https://www.kaggle.com/c/human-protein-atlas-image-classification/）、TensorFlow 2.0问答系统（https://www.kaggle.com/c/tensorflow2-question-answering）

- 平均F1值：Shopee价格匹配担保（https://www.kaggle.com/c/shopee-product-matching/）。此处对每行预测结果计算\( {F1} \)分数后取平均，而宏平均F1则是各类别\( {F1} \)分数的算术平均值。

此外还有二次加权卡帕系数，我们后续将探讨其作为序数预测问题的智能评估指标。其基础形式科恩卡帕系数仅衡量预测值与真实值的一致性。该指标最初用于评估标注者间一致性，但其通用性使其衍生出更广泛的应用。

什么是标注者间一致性？假设你有个标注任务：根据照片内容标记"猫"、"狗"或"无"。若让多人执行该任务，可能出现误标——某个评判者可能将狗误认为猫。正确做法是让多名评判者对相同照片独立标注，再通过科恩卡帕系数衡量其一致性程度。

因此，科恩卡帕系数被设计为反映两名标注者在分类问题上一致程度的指标：

\[k = \left( {{p}_{0} - {p}_{e}}\right) /\left( {1 - {p}_{e}}\right) \]

公式中\( {p}_{\mathrm{o}} \)表示评判者间实际观测到的一致率，\( {p}_{\mathrm{e}} \)代表随机达成一致的理论概率。使用混淆矩阵术语可改写为：

\[k = \frac{2 * \left( {{TP} * {TN} - {FN} * {FP}}\right) }{\left( {{TP} + {FP}}\right)  * \left( {{FP} + {TN}}\right)  + \left( {{TP} + {FN}}\right)  * \left( {{FN} + {TN}}\right) }\]

该公式的精妙之处在于：分数会扣除随机达成一致的经验概率，从而对所有最可能分类进行校正。指标范围从1（完全一致）到-1（完全对立），

接近0的值表示评判者间的一致或分歧纯属随机。这有助于判断模型是否确实比随机猜测表现更好。

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_149.jpg?x=242&y=229&w=365&h=364&r=0"/>

<!-- Media -->

## 安德烈·卢基扬年科专访

https://www.kaggle.com/artgor

本章第二位访谈对象是Notebooks与讨论区双料大师、竞赛专家安德烈·卢基扬年科。他现任MTS集团机器学习工程师与技术主管，分享了精彩的Kaggle参赛心得。

## 您最青睐哪类竞赛？在技术方案和解决路径方面，您的Kaggle专长是什么？

我偏好解决方案具备通用性、可迁移至其他数据集/领域的竞赛。热衷于尝试各种神经网络架构、前沿方法和后处理技巧。不倾向需要逆向工程或构造"黄金特征"的比赛，这类方法通常缺乏普适性。

## 您在参与竞赛期间还斩获了Notebooks（并登顶榜首）和讨论区双料大师称号。这是您刻意规划的目标吗？

我在撰写Notebooks上投入了大量时间和精力，但Discussion Grandmaster（讨论大师）的排名却像是自然而然获得的。

让我们先从Notebook排名说起。

2018年有个名为DonorsChoose.org申请筛选的特殊比赛。DonorsChoose是一个资助基金，帮助全美公立学校教师为学生申请急需的教学物资和实践机会。该比赛不以排行榜分数定胜负，而是根据Notebook获得的点赞数来评选优胜方案。这很有趣，我便为比赛写了篇Notebook。许多参赛者在社交媒体上推广自己的分析，我也照做了。最终我获得第二名，赢了一台Pixelbook（至今仍在用！）

这次成功极大地激励了我继续撰写Notebooks。最初我只是想分享分析成果并获得反馈，因为想通过与他人比较分析能力和可视化技巧来检验自己的水平。当人们开始喜欢我的内核时，我便想进一步提升技能。另一个动力是希望提高快速制作MVP（最小可行产品）的能力。新比赛开始时，很多人会立即撰写Notebooks，要想成为首批发布者，就必须在保证质量的前提下快速完成。这很有挑战性，但也充满乐趣和回报。2019年2月我获得Notebook Grandmaster（笔记本大师）称号，后来一度稳居榜首超过一年。现在虽然写得少了，但我依然乐在其中。

至于讨论排名，我觉得是水到渠成的事。我回复Notebooks下的评论，分享并讨论参与比赛的想法，排名就逐渐上升了。

## 请分享你参加过最具挑战性的比赛，以及你用来解决任务的洞见。

那是在"预测分子特性"比赛中。我写过详细博客(https://towardsdatascience.com/a-story-of-my-first-gold-medal-in-one-kaggle-competition-things-done-and-lessons-learned-c269d9c233d1)。这是专业领域赛事，目标是预测分子中原子间的相互作用。核磁共振(NMR)是与MRI原理相似的技术，用于解析蛋白质和分子结构。全球研究者通过NMR实验推进分子结构研究，涉及环境科学、制药科学和材料科学等领域。比赛中我们尝试预测分子内两个原子的磁相互作用（标量耦合常数）。量子力学前沿方法仅需输入\( {3D} \)分子结构即可计算这些耦合常数，但计算资源消耗极大。若机器学习能预测这些值，将极大帮助药物化学家更快、更经济地获取结构洞见。

我通常为新Kaggle比赛撰写EDA（探索性数据分析）内核，这次也不例外。Kaggle表格数据比赛的常见方法是大量特征工程和使用梯度提升模型。早期尝试中我也用了LGBM，但意识到处理图数据应有更好方法。我明白领域专业知识会带来巨大优势，因此搜集了所有相关资料。当然，我注意到论坛里有几位活跃专家发表文章和内核，便研读了他们所有内容。某天我收到该领域专家的邮件，认为我们可以优势互补。通常我喜欢独自参赛一段时间，但这次组队似乎是好主意。这个决定后来被证明非常正确！我们逐渐组建了强大团队。

一段时间后，我们注意到神经网络在比赛中的潜力：知名Kaggle选手Heng发布了MPNN（消息传递神经网络）模型示例。后来我成功运行了它，但效果不如我们的模型。不过团队明白，要想取得好成绩就必须研究这些神经网络。Christof以惊人速度构建新神经网络的能力令人赞叹。很快我们全力投入神经网络开发，之后我的角色转为辅助支持。我做了大量神经网络实验：尝试不同超参数、架构、训练方案微调等。有时还对预测结果做EDA分析，找出有趣或错误案例，这些信息后来都用于进一步优化模型。

我们赢得了\( {8}^{\text{th }} \)名次，在这次比赛中我收获颇丰。

## Kaggle是否对你的职业生涯有所帮助？如果有，具体体现在哪些方面？

Kaggle确实给予我极大帮助，特别是在技能提升和个人品牌建设方面。撰写和发布Kaggle Notebook不仅教会了我EDA（探索性数据分析）和机器学习技能，更迫使我培养适应能力——快速理解新课题任务、在不同方法间高效迭代。同时，它为我提供了可见度，因为我的工作得到了同行认可。

我的第一个作品集(https://erlemar.github.io/)包含大量Notebook，其中半数基于往届Kaggle竞赛。这对获得第一份工作至关重要。我的Kaggle成就还吸引了优质企业招聘官的关注，有时甚至能跳过面试环节，更促成了多次咨询合作机会。

## 根据你的经验，新手Kagglers常会忽视什么？你现在掌握的哪些知识希望当初刚开始时就了解？

我认为需要将新手Kagglers分为两类：数据科学领域的新手和Kaggle平台的新手。

数据科学新手常犯以下错误（这很正常，所有人都有起步阶段）：

- 最严重的问题之一：缺乏批判性思维，不懂如何自主研究；

- 不清楚何时使用何种工具/方法；

- 盲目套用公开Notebook却不理解其原理；

- 固执坚持某个无效想法并耗费过多时间；- 实验失败时陷入绝望丧失动力

对于有数据科学经验但缺乏Kaggle经验的人，他们最严重的误判是低估了Kaggle的难度。没预料到平台竞争如此激烈：需要尝试多种方案才能成功，存在仅适用于比赛的技巧，还有职业竞赛选手。此外，人们常高估领域专业知识的作用。虽然确实有专业团队斩获金牌的案例，但多数情况下经验丰富的Kagglers更胜一筹。

我还多次目睹这种情况：有人宣称赢得Kaggle很容易，他（或其团队）短期内将获得金牌。结果往往悄无声息地失败。

## 你在过往比赛中犯过哪些错误？

- 数据探索不足。有时因此无法生成更优特征或应用更好的后处理方法。而逆向工程和"黄金特征"本身就是一个复杂课题。

- 在单一想法上耗费过多时间，寄望于其终会奏效。这属于沉没成本谬误。

- 实验不足。付出终有回报——若在竞赛中投入的时间和资源不够，就无法在排行榜上取得高位。

- 参加了"错误"的竞赛。有些竞赛存在数据泄露、逆向工程等问题；有些竞赛的公开测试数据与私有测试数据划分不合理导致排名震荡；还有些竞赛本身缺乏吸引力，本不该参与。

- 与不合适的队友组队。曾多次遇到队友活跃度不如预期，最终拖累团队成绩的情况。

## 参加竞赛时最需要牢记或做到的关键事项是什么？

我认为关键在于明确目标、清楚自己愿意投入的资源，并预判可能的结果。参赛动机多种多样：- 赢取奖金或奖牌；- 获取新技能或提升现有能力；- 接触新任务/领域；- 拓展人脉；- \( {PR} \)；- 等等

当然可能存在多重动机。关于资源投入，通常涉及你愿意花费的时间精力以及现有硬件条件。

所谓预判结果，是指要考虑竞赛结束时的各种可能性。你可能投入大量资源并获胜，也可能铩羽而归。能否接受这种现实？赢得特定竞赛对你是否至关重要？也许你需要准备投入更多努力；反过来说，若你怀揣长期目标，一次失败或许无伤大雅。

目标检测问题的评估指标

近年来，Kaggle平台上深度学习竞赛日益增多。这些竞赛大多聚焦图像识别或自然语言处理任务，其评估指标与目前探讨的差异不大。但目标检测与图像分割这类特殊问题，需要采用特定的评估指标才能准确衡量模型性能。

<!-- Media -->

<!-- figureText: Classification + localization (cat) Object detection (dog, cat) -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_153.jpg?x=252&y=1022&w=1384&h=588&r=0"/>

图5.4：计算机视觉任务示例。（数据源：https://cocodataset.org/#explore?id=38282，https://cocodataset.org/#explore?id=68717）

<!-- Media -->

目标检测任务并非对整幅图像分类，而是定位画面中的相关区域并加以标注。如图5.4所示，目标检测分类器需在照片中定位猫狗所在区域，并用对应标签进行分类。左例通过矩形框（称为边界框）标定猫的位置，右例则展示如何用边界框检测多只猫狗并进行正确分类（蓝色框标注狗，红色框标注猫）。在目标检测中，我们使用边界框来描述物体的空间位置，即用矩形区域框定物体范围。通常用两组(x,y)坐标（左上角与右下角）来定义边界框。从机器学习算法角度看，确定边界框坐标相当于对多个目标进行回归预测。实际应用中，开发者通常会直接采用预构建模型（如Mask R-CNN、RetinaNet、FPN、YOLO、Faster R-CNN或SSD），而非从头构建。

图像分割则需进行像素级分类。对于\( {320} \times  {200} \)尺寸的图像，实际需要进行64,000次像素分类。根据任务类型，可分为需对照片所有像素分类的语义分割，以及仅对特定目标像素分类的实例分割（例如下图5.5中的猫）：

<!-- Media -->

<!-- figureText: Semantic segmentation (cat, sofa) Instance segmentation (cat) -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_154.jpg?x=423&y=1165&w=1042&h=485&r=0"/>

图5.5：同一图像的语义分割与实例分割对比（数据源：https://cocodataset.org/#explore?id=338091）

<!-- Media -->

首先概述适用于这两类任务的专用指标。由于两者都需要预测画面中的连续区域（目标检测为矩形区域，分割为多边形区域），并与同样以区域形式表示的真实标注进行比较。分割任务中最简单的指标是像素精度，即像素分类的正确率。但该指标存在明显缺陷：当目标像素占比较低时（类似二分类或多分类中的样本不均衡问题），仅预测背景类别就能获得虚高的分数，这实际上等同于未进行有效分割。

因此竞赛中最常采用两个更具代表性的指标：交并比(IoU)和戴斯系数(Dice coefficient)。

## 交并比(IoU)

交并比(IoU)又称杰卡德指数(Jaccard index)。在分割任务中应用IoU时，需比较预测图像与真实标注掩膜——后者通常是二进制矩阵，值1表示目标区域，0表示背景。对于多目标场景，每个类别都有对应的标注掩膜。

在目标检测任务中，IoU通过比较预测边界框与真实边界框的顶点坐标来计算。针对每个分类类别，先计算预测区域与真实区域的交集面积，再除以二者的并集面积（该并集已自动包含重叠部分）。这种计算方式能均衡惩罚两种错误：预测区域过大（导致分母增大）或过小（导致分子减小）。

<!-- Media -->

<!-- figureText: Area of overlap Area of union -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_155.jpg?x=535&y=1284&w=811&h=426&r=0"/>

图5.6：IoU计算的可视化说明

<!-- Media -->

图5.6直观展示了计算所涉及的区域。通过想象正方形重叠部分增大，可以理解该度量标准如何有效惩罚预测范围超出真实值的情况（即使覆盖了真实值，联合区域变大会导致指标下降）。以下是使用交并比(IoU)的竞赛示例：

- TGS盐体识别挑战赛(https://www.kaggle.com/c/tgs-salt-identification-challenge/) 采用交并比目标分割

- FGVC6时尚材料识别2019(https://www.kaggle.com/c/imaterialist-fashion-2019-FGVC6) 采用带分类的交并比目标分割

- 空客船舶检测挑战赛(https://www.kaggle.com/c/airbus-ship-detection) 采用交并比目标分割测试版

## Dice系数

另一个重要指标是Dice系数，其计算方式是将预测与真实值的重叠区域面积翻倍后，除以两者面积之和：

<!-- Media -->

<!-- figureText: Area of overlap Sum of areas -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_156.jpg?x=339&y=1026&w=1201&h=370&r=0"/>

图5.7：Dice计算的可视化示意

<!-- Media -->

与杰卡德指数不同，该指标分母不考虑预测与真实值的重叠部分。其核心思想是通过最大化重叠区域来确保预测范围准确。若预测范围过大仍会受惩罚。实际上这两个指标呈正相关，在单分类问题中结果几乎一致。

差异主要体现在多类别场景。使用IoU和Dice系数时需对所有类别结果取平均，但IoU对单类别预测错误惩罚更严厉，而Dice系数更宽容，能更好反映整体性能。采用Dice系数的Kaggle竞赛案例（常见于医疗领域，但也适用于云层、车辆等场景）：

- HuBMAP肾脏破解挑战：https://www.kaggle.com/c/hubmap-kidney-segmentation

- 超声神经分割：https://www.kaggle.com/c/ultrasound-nerve-segmentation

- 卫星图像云层识别：https://www.kaggle.com/c/understanding_cloud_organization

- Carvana车辆图像掩膜挑战：https://www.kaggle.com/c/carvana-image-masking-challenge

IoU和Dice系数构成了分割与目标检测领域更复杂指标的基础。通过设定合适阈值（通常为0.5），可判定是否确认检测结果（即分类）。此时可采用前文讨论的分类指标，如精确率、召回率和\( {F1} \)，正如PASCAL VOC(http://host.robots.ox.ac.uk/pascal/VOC/voc2012)和COCO(https://cocodataset.org)等经典目标检测挑战赛所做的那样。

## 多标签分类与推荐系统的评估指标

推荐系统是数据分析和机器学习最热门的应用之一，Kaggle上举办过多个相关竞赛。例如"快画！涂鸦识别挑战"就采用推荐系统式评估。而Expedia酒店推荐(https://www.kaggle.com/c/expedia-hotel-recommendations)等竞赛则真正致力于构建推荐系统。推荐系统会议RecSYS(https://recsys.acm.org/)甚至曾在Kaggle举办年度赛事（RecSYS 2013：https://www.kaggle.com/c/yelp-recsys-2013）。

在\( K \)处的平均精度均值(MAP@K)通常是评估推荐系统性能的首选指标，也是Kaggle平台上所有试图将问题构建或视为推荐系统的竞赛中最常见的衡量标准。还存在其他指标如k处精度(P@K)和\( \mathbf{k} \)处的平均精度(\( \mathbf{{AP}}@\mathbf{K} \))，这些损失函数本质上是针对每个单独预测计算的。理解其运作原理有助于更深入把握MAP@K在推荐系统和多标签分类中的表现机制。

实际上，与推荐系统类似，多标签分类意味着模型会输出一系列类别预测。这类结果既可通过二元分类指标的平均值来评估（例如希腊媒体监控多标签分类比赛(WISE 2014)采用的平均F1分数：https://www.kaggle.com/c/wise-2014），也可使用更典型的推荐系统指标如MAP@K。本质上，无论是推荐还是多标签预测，都可视为排序任务——前者生成有序推荐列表，后者产生无序标签集合。

## MAP@{K}

\( \mathrm{{MAP}}@\mathrm{K} \)是个复合指标，由多重计算得出。要透彻理解MAP@K，需从其最基础的组件——\( \mathbf{k} \)处精度(P@K)开始。当模型对样本的预测结果为概率降序排列时，该函数仅考量前\( k \)个预测，计算其与真实标签的匹配数量后除以\( k \)。简言之，这类似于对前\( k \)个预测取平均的准确率衡量方式。

计算稍复杂但概念简单的\( k \)处平均精度(AP@K)，是对1到\( k \)范围内所有\( \mathrm{P}@\mathrm{K} \)取均值。该指标通过依次评估前1个、前2个直至前\( k \)个预测，全面衡量预测系统的整体表现。

最终MAP@K是整个预测样本AP@K的平均值，作为综合性指标涵盖所有预测评估。Expedia酒店推荐竞赛(https://www.kaggle.com/c/expedia-hotel-recommendations)中MAP@5的公式定义如下：

\[{MAP}@5 = \frac{1}{\left| U\right| }\mathop{\sum }\limits_{{u = 1}}^{\left| U\right| }\mathop{\sum }\limits_{{k = 1}}^{{\min \left( {5,n}\right) }}P\left( k\right) \]

公式中\( \left| U\right| \)表示用户推荐数量，\( P\left( k\right) \)代表截止点\( k \)处的精度，\( n \)是预测酒店集群数（每次推荐最多预测5家酒店）。虽然比我们的解释更复杂，但公式本质上表示\( \mathrm{{MAP}}@\mathrm{K} \)是所有预测\( \mathrm{{AP}}@\mathrm{K} \)评估结果的均值。

在完成对不同回归和分类指标的专项梳理后，我们接下来探讨如何在Kaggle竞赛中处理评估指标。

## 优化评估指标

综上所述，目标函数是学习算法内部用于衡量模型拟合数据优劣的函数，并通过反馈指导算法迭代优化。显然，当Kaggle评估指标与算法目标函数完全匹配时，模型能获得最佳表现。

但现实往往不尽如人意。常见的困境是现有目标函数只能近似评估指标。在目标函数与评估指标不匹配时，您有以下选择：

1. 修改学习算法使其包含与评估指标匹配的目标函数（但并非所有算法都支持，如LightGBM和XGBoost允许自定义目标函数，而多数Scikit-learn模型则不行）。

2. 调整模型超参数，选择那些能最大化评估指标表现的组合。

3. 对结果进行后处理，使其更贴近评估标准。例如，可以编写一个优化器对预测结果进行转换（概率校准算法就是一个例子，我们将在本章末尾讨论这类方法）。

将竞赛指标融入机器学习算法是实现更好预测效果的最有效方法，尽管只有少数算法能通过改造将竞赛指标作为目标函数。因此第二种方法更为常见，许多竞赛最终都演变为围绕评估指标寻找最佳模型超参数的较量。若已编写好评估函数，那么选择合适的交叉验证方法或测试集就至关重要。若手头没有现成的评估函数，则需要根据Kaggle提供的公式进行适当编码。

以下方法往往能带来显著提升：

- 通过搜索引擎查找与评估指标及其编码函数相关的所有信息

- 浏览常用工具包（如Scikit-learn：https://scikit-learn.org/stable/modules/model_evaluation.html#model-evaluation 或 TensorFlow：https://www.tensorflow.org/api_docs/python/tf/keras/losses）

- 查阅GitHub项目（例如Ben Hammer的Metrics项目：https://github.com/benhamner/Metrics）

- 在论坛和现有Kaggle笔记本中提问或查找（包括当前竞赛及类似竞赛）

- 此外，如前所述，查询Meta Kaggle数据集（https://www.kaggle.com/kaggle/meta-kaggle）并查看竞赛表，可快速找到使用相同评估指标的其他Kaggle竞赛，直接获取可借鉴的代码和思路

我们将详细探讨当评估指标与算法目标函数不匹配时的解决方案。首先从自定义指标开始分析。

## 自定义指标与目标函数

当目标函数与评估指标不一致时，前文提到可通过创建自定义目标函数解决，但仅有少数算法能方便地改造以适配特定目标函数。

值得庆幸的是，这些支持改造的算法恰是Kaggle竞赛和数据科学项目中最有效的工具。虽然创建自定义目标函数看似复杂，但这确实是提升竞赛得分的绝佳途径。例如XGBoost、CatBoost、LightGBM等梯度提升算法，以及基于TensorFlow或PyTorch的深度学习模型都支持此类操作。

以下资源提供TensorFlow和PyTorch自定义指标与目标函数的优质教程：

- https://towardsdatascience.com/custom-metrics-in-keras-and-how-simple-they-are-to-use-in-tensorflow2-2-6d079c2ca279

- https://petamind.com/advanced-keras-custom-loss-functions/

- https://kevinmusgrave.github.io/pytorch-metric-learning/extend/losses/

这些将为您提供基础函数模板及关于如何编写自定义目标函数或评估函数的有用建议。

若您想直接获取所需的自定义目标函数，可尝试RNA的这份Notebook（https://www.kaggle.com/bigironsphere）：https://www.kaggle.com/bigironsphere/loss-function-library-keras-pytorch/notebook。其中包含适用于TensorFlow和PyTorch的各类竞赛中出现过的自定义损失函数。

如需在LightGBM、XGBoost或CatBoost中创建自定义损失函数，根据其官方文档要求，您需要编写一个以预测值和真实值为输入，并返回梯度（gradient）和海森矩阵（hessian）的函数。

您可参考Stack Overflow上的这篇帖子来深入理解梯度与海森矩阵的概念：https://stats.stackexchange.com/questions/231220/how-to-compute-the-gradient-and-hessian-of-logarithmic-loss-question-is-based。

从代码实现角度看，您只需创建一个函数（若需传递预测标签向量和真实标签之外的参数，可使用闭包）。以下是一个焦点损失函数（Focal Loss，该损失函数在计算时会大幅加权少数类，详见Lin, T-Y.等人的论文《Focal Loss for Dense Object Detection》：https://arxiv.org/abs/1708.02002）的简单示例，可作为自定义函数的模板：

---

from scipy.misc import derivative

import xgboost as xgb

def focal_loss(alpha, gamma):

def loss_func(y_pred, y_true):

a, \( \mathrm{g} = \) alpha,gamma

def get_loss(y_pred, y_true):

p = 1 / (1 + np.exp(-y_pred))

loss = (-(a * y_true + (1 - a)*(1 - y_true)) *

((1 - (y_true * p + (1 - y_true) *

(1 - p)))**g) * (y_true * np.log(p) +

(1 - y_true) * np.log(1 - p)))

返回损失值

partial_focal = lambda y_pred: 获取损失值(y_pred, y_true)

梯度 = 求导(partial_focal, y_pred, n=1, dx=1e-6)

海森矩阵 = 求导(partial_focal, y_pred, n=2, dx=1e-6)

返回 梯度, 海森矩阵

返回损失函数

xgb = xgb.XGBClassifier(目标函数=焦点损失函数(alpha=0.25, gamma=1))

---

上述代码片段定义了一个新的代价函数——焦点损失函数(focal_loss)，并将其传入XGBoost实例的目标参数。这个示例很有价值，因为焦点损失函数需要配置特定参数(alpha和gamma)才能在你的问题上有效工作。直接将参数值硬编码到函数中的简易方案并不理想，因为在模型调优时可能需要系统性地调整这些参数。而在我们实现的函数中，当参数传入焦点损失函数后会被存储在内存中，并通过返回给XGBoost的loss_func函数进行引用。因此最终返回的代价函数会正确引用你初始设定的alpha和gamma值。

这个示例另一个亮点是，借助SciPy的求导函数可以轻松计算代价函数的梯度和海森矩阵。只要你的代价函数可微，就无需手动计算。但构建自定义目标函数需要一定的数学知识，并需投入大量精力确保其适用性。Max Halford在LightGBM算法中实现焦点损失函数时遇到的困难及解决方案，可参阅：https://maxhalford.github.io/blog/lightgbm-focal-loss/。尽管实现难度大，但在Kaggle竞赛中定制损失函数往往能成为制胜关键——它能帮你从模型中榨取极致性能。

若自定义目标函数失败，可退而求其次将其编码为评估指标。虽然模型不会直接针对该函数优化，但基于此进行超参数调优仍能提升预测性能——这正是前文提到的第二方案。需注意，从头编写评估指标时需遵循特定编码规范。例如在Scikit-learn中，需使用make_scorer函数进行封装。该包装器会适配评估函数使其符合Scikit-learn API规范，处理包括：是否使用概率估计而非预测值、是否需要设定预测阈值、以及最重要的优化方向（最大化或最小化评分指标）：

---

from sklearn.metrics import make_scorer

from sklearn.metrics import 平均精确率得分

评分器 = make_scorer(平均精确率得分,

average='加权', greater_is_better=True, needs_proba=False)

---

本示例创建了基于平均精确率的评分器，指定在多分类问题中采用加权计算方式。

针对评估指标进行优化时，可应用网格搜索、随机搜索或贝叶斯优化等高级方法，找出使算法在该指标下表现最优的参数组合——即使模型使用不同代价函数。我们将在讨论完模型验证（特别是涉及表格数据问题的章节）后，详细探讨如何在Kaggle竞赛中最佳配置参数优化以获得最优结果。

## 预测结果的后处理

后处理调优意味着通过特定函数对预测结果进行转换，以获得更优的评估效果。在构建自定义损失函数或针对评估指标优化后，您还可以通过对预测结果施加特定函数来利用评估指标的特性提升模型表现。以二次加权卡帕（Quadratic Weighted Kappa）为例，前文提到该指标适用于序数值预测场景。简言之，原始卡帕系数是算法预测与真实值之间经过机会校正的一致性指标，本质上是扣除偶然匹配概率后的准确度度量。其原始计算公式如下所示：

\[k = \left( {{p}_{0} - {p}_{e}}\right) /\left( {1 - {p}_{e}}\right) \]

公式中\( {p}_{0} \)表示评估者间相对观测一致性，\( {p}_{e} \)代表随机一致性的理论概率。此处仅需两个矩阵：观测分数矩阵和基于随机一致性的期望分数矩阵。当采用加权卡帕系数时，还需引入权重矩阵，公式演变为：

\[k = \left( {{p}_{0} - {p}_{e}}\right) /\left( {1 - {p}_{p}}\right) \]

矩阵\( {p}_{p} \)包含差异化误差惩罚权重，这对序数预测尤为重要——当预测值与真实值偏差越大时惩罚越重。采用二次形式（即对\( k \)进行平方运算）会进一步加剧惩罚力度。但由于该指标难以实现为损失函数，直接优化颇具挑战性，此时后处理技术便能发挥作用。

PetFinder.my宠物领养预测大赛（https://www.kaggle.com/c/petfinder-adoption-prediction）提供了典型范例。该赛事结果采用5级评分制（0-4分），参赛者既可采用分类也可选择回归方法。若使用回归模型，对回归输出进行后处理转换可显著提升模型在二次加权卡帕指标上的表现，效果优于直接输出离散预测的分类方法。

该赛事中的后处理流程包含优化步骤：先将回归结果通过初始阈值[0.5, \( {1.5},{2.5},{3.5}\rbrack \)]转为整数，再经迭代微调寻找使性能最大化的最优阈值组。阈值优化需借助SciPy的optimize.minimize（基于Nelder-Mead算法）等优化器实现，并通过交叉验证验证最优阈值组的有效性。详情可参阅Abhishek Thakur在赛事期间的技术帖：https://www.kaggle.com/c/petfinder-adoption-prediction/discussion/76107。除该赛事外，众多竞赛案例证明智能后处理能有效提升成绩与排名，例如：

- https://www.kaggle.com/khoongweihao/post-processing-technique-c-f-1st-place-jigsaw

- https://www.kaggle.com/tomooinubushi/postprocessing-based-on-leakage

- https://www.kaggle.com/saitodevel01/indoor-post-processing-by-cost-minimization

遗憾的是，后处理通常高度依赖于所使用的评估指标（理解指标对设计优质后处理至关重要），且往往具有数据特异性——例如时间序列数据与数据泄漏的情况。因此很难总结出适用于所有比赛的通用后处理方案。但务必保持警觉，在竞赛中时刻留意后处理可能提升效果的蛛丝马迹。参考往届类似竞赛的讨论帖总能获得启发——最终总会有人提出这个话题。

## 预测概率及其调整

为完善前述关于指标优化（预测后处理）的讨论，我们将探讨需要精准预测概率但不确定所用算法表现的情况。如前所述，分类概率问题存在于二分类与多分类场景，通常通过二元或多元对数损失（又称交叉熵损失）来评估（详见前文"分类指标：标签预测与概率"及"多分类指标"章节）。

但仅评估或优化对数损失可能不够。在追求概率预测准确性时需警惕以下核心问题：

- 模型未输出真实概率估计

- 类别分布不均衡

- 训练集与测试集（包括公开/私有排行榜）的类别分布差异。仅第一点就足以要求我们从建模不确定性角度检验分类预测质量。事实上，即便Scikit-learn中许多算法都提供predict_proba方法，这远不能保证其输出的是真实概率。

以决策树为例（它是众多表格数据建模方法的基础）。分类决策树(https://scikit-learn.org/stable/modules/generated/sklearn.tree.DecisionTreeClassifier.html)输出的概率基于终端叶节点——即取决于包含预测样本的叶节点类别分布。若树完全生长，该样本很可能位于仅含少量样本的叶节点中，导致预测概率虚高。调整max_depth、max_leaf_nodes或min_samples_leaf等参数时，随着树结构变化，输出概率会在高低值间剧烈波动。

决策树是集成方法（如装袋模型、随机森林）和提升方法（如梯度提升树及其高效实现XGBoost/LightGBM/CatBoost）最常见的基模型。但同样由于缺乏坚实概率估计基础，该问题也影响支持向量机、\( k \)近邻等常用模型。在Otto集团产品分类挑战赛(https://www.kaggle.com/c/otto-group-product-classification-challenge/overview/)前，这些隐患鲜为人知，直到Christophe Bourguignat等人提出(参见https://www.kaggle.com/cbourguignat/why-calibration-works)，当时利用Scikit-learn新增的校准函数便轻松解决了问题。

除模型因素外，类别不平衡也会导致模型不可靠。处理非平衡分类问题时，可采用欠采样/过采样策略，或在算法计算损失时为不同类别设置自定义权重。这些策略虽能提升模型性能，但必然扭曲概率估计——可能需进一步调整才能在排行榜上获得更好分数。

最后，第三个关注点与测试集的分布方式有关。这类信息通常被隐藏，但往往有方法可以估算出来（例如，基于公开排行榜结果通过试错法推断，如我们在第1章《Kaggle与其他数据科学竞赛介绍》中所述）。比如，iMaterialist家具挑战赛（https://www.kaggle.com/c/imaterialist-challenge-furniture-2018/）和更知名的Quora问题对比赛（https://www.kaggle.com/c/quora-question-pairs）都引发了关于如何通过后处理调整概率以匹配测试预期的广泛讨论（具体方法可参阅https://swarbrickjones.wordpress.com/2017/03/28/cross-entropy-and-training-test-class-imbalance/ 和 https://www.kaggle.com/dowakin/probability-calibration-0-005-to-1b）。从全局来看，即使不了解待预测类别的测试分布，基于训练数据先验信息正确预测概率仍非常有益（在获得反证前，这就是模型应模拟的概率分布）。事实上，若预测概率分布与训练集一致，后续修正将容易得多。

当预测概率与目标变量的训练分布不匹配时，解决方案是使用Scikit-learn提供的校准函数CalibratedClassifierCV：

---

sklearn.calibration.CalibratedClassifierCV(base_estimator=None, *,

method='sigmoid', cv=None, n_jobs=None, ensemble=True)

---

该校准函数的作用是对预测概率施加后处理函数，使其更贴近真实观测到的经验概率。只要模型是Scikit-learn模型或具有类似行为，该函数将作为模型包装器，直接将预测结果导入后处理函数。有两种后处理方法可选：其一是sigmoid法（又称Plat缩放），本质上是逻辑回归；其二是保序回归——一种非参数回归方法，需注意样本较少时易过拟合。

还需选择校准器的拟合方式。记住这是应用于模型结果的次级模型，必须通过系统化重构预测来避免过拟合。可采用交叉验证（下章《设计优质验证》将详述）生成多个模型，取其平均值作为最终预测（ensemble=True）。或者采用我们惯用的留出法预测（后续章节详述），基于全量数据进行校准（ensemble=False）。尽管CalibratedClassifierCV能应对多数情况，也可探索经验性方法优化概率估计以获得最佳测试表现。任何转换函数皆可尝试，从手工构建到遗传算法推导的复杂函数均可。唯一限制是必须进行交叉验证，且最好在公开排行榜取得良好结果（但非必需，因更应信任本地交叉验证分数，下章将讨论）。Silogram（https://www.kaggle.com/psilogram）在微软恶意软件分类挑战中通过网格搜索确定指数，将随机森林不可靠概率输出转化为可靠概率的策略便是典型案例（参见https://www.kaggle.com/c/malware-classification/discussion/13509）。

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_168.jpg?x=241&y=819&w=359&h=361&r=0"/>

<!-- Media -->

## 苏达莱·拉吉库马尔

https://www.kaggle.com/sudalairajkumar

本章最后访谈中，我们对话了竞赛、数据集和笔记本领域的大师级人物苏达莱·拉吉库马尔（SRK），他同时是讨论大师。这位Analytics Vidhya数据科学平台排名第一的专家，现任初创企业AI/ML顾问。

## 您最青睐哪类竞赛？原因是什么？在技术方法和解决策略方面，您在Kaggle上的专长是什么？

我最钟爱需要大量特征工程的竞赛，这恰是我的强项。我通常热衷于通过数据探索深入理解数据（可从我的简单探索笔记本系列https://www.kaggle.com/sudalairajkumar/code 看出），继而基于洞察构建特征。

您如何着手应对Kaggle竞赛？这种方式与日常工作有何不同？

竞赛框架涵盖数据探索、寻找合适的验证方法、特征工程、模型构建以及集成/堆叠。这些同样是我日常工作的一部分。但除此之外，我的日常工作中还涉及大量利益相关方讨论、数据收集、数据标注、模型部署、模型监控和数据故事讲述。

## 请分享一次你参与的特别具有挑战性的竞赛，以及你用来解决任务的见解。

桑坦德产品推荐赛是我们参与过的一场难忘的竞赛。罗翰和我进行了大量特征工程并构建了多个模型。在最终集成时，我们为不同产品设置了不同权重，其中部分权重之和并未等于1。通过数据探索和理解，我们手工挑选了这些权重，这为我们提供了帮助。这让我们意识到领域知识/数据在解决问题中的重要性，以及数据科学既是科学也是艺术。

## Kaggle对你的职业生涯有帮助吗？如果有，是怎样的？

Kaggle在我的职业生涯中起到了非常重要的作用。我能够获得最近两份工作主要归功于Kaggle。此外，在Kaggle上的成功让我更容易与数据科学领域的其他佼佼者建立联系并向他们学习。它对我目前担任初创公司AI/ML顾问的角色也大有裨益，因为它提供了可信度。

## 根据你的经验，缺乏经验的Kaggle用户常常忽视什么？你现在知道的哪些事情是你希望刚开始时就了解的？

深入理解数据。这一点经常被忽视，人们会直接开始构建模型。数据探索在任何Kaggle竞赛的成功中都扮演着非常重要的角色。这有助于建立适当的交叉验证，创建更好的特征，并从数据中提取更多价值。

## 你在过去的竞赛中犯过哪些错误？

这是个很长的清单，我会说这些都是学习机会。在每场竞赛中，我尝试的20-30个想法里可能只有1个有效。这些错误/失败带来的学习远比实际成功或有效的方法要多。例如，我在最早期的某次竞赛中通过从最高分位跌至最低分位的惨痛经历，才真正理解了过拟合。但那次教训从此永远铭记于心。

有没有特别推荐用于数据分析/机器学习的工具或库？

对于表格数据，我主要使用XGBoost/LightGBM。如今我也会使用开源AutoML库和Driverless AI来获取早期基准。在深度学习模型方面，我使用Keras、Transformers和PyTorch。

# 参加竞赛时，最重要的注意事项或行动是什么？

持之以恒是关键。每场竞赛都会有起伏。会有很多天毫无进展，但我们不应放弃，要不断尝试。我认为这不仅适用于Kaggle竞赛，也适用于任何事情。

## 你使用其他竞赛平台吗？它们与Kaggle相比如何？

我也参加过Analytics Vidhya的DataHack平台、Driven Data、CrowdAnalytix等其他平台。它们也不错，但Kaggle应用更广泛且具有全球性，因此Kaggle上的竞争激烈程度远高于其他平台。

## 总结

本章我们探讨了Kaggle竞赛中的评估指标。首先阐述了评估指标与目标函数的区别，并对比了回归问题与分类问题的差异。针对每类问题，我们分析了Kaggle竞赛中最常见的评估指标。

随后讨论了那些竞赛中罕见且可能不再出现的特殊指标。最后通过解析往届赛事案例，深入研究了多种常见指标的应用场景，并提出若干优化评估指标的策略。特别建议尝试编写自定义损失函数，并就后处理步骤提供了实用建议。

现在您应当理解评估指标在Kaggle竞赛中的作用，并掌握应对常见与非常见指标的方法——通过复盘历史赛事及透彻理解指标运作机制。下一章我们将讨论如何运用评估指标，并通过验证策略准确评估您的竞赛方案表现。

## 加入本书Discord空间

加入本书Discord工作区，每月参与作者问答会：

https://packt.link/KaggleDiscord

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_173.jpg?x=247&y=311&w=178&h=237&r=0"/>

<!-- Media -->

## 设计优质验证方案

在Kaggle竞赛中，当沉浸于建模与提交结果时，人们容易轻信排行榜显示的表面成绩。您可能认为竞赛排名就是一切——这是赛事中反复出现的认知误区。实际上，在比赛结束前您无法得知真实排行榜（私有榜单）情况，盲目信任公开榜单并不可取，因其往往具有误导性。

本章将阐述数据竞赛中验证机制的重要性，您将学习：

- 过拟合现象及公开榜单的误导性

- 可怕的排名震荡

- 各类验证策略

- 对抗性验证

- 如何发现并利用数据泄漏

- 最终提交时的策略选择

监控建模表现并识别过拟合时机，不仅是数据科学竞赛更是所有数据项目的核心能力。掌握正确的模型验证方法，既是Kaggle赛事中最值得学习的技能，也是职场中极具价值的核心竞争力。

## 排行榜窥探现象

如前所述，在每场竞赛中，Kaggle将测试集划分为公开部分（显示于实时排行榜）和私有部分（用于计算最终得分）。这些测试部分通常随机确定（时序竞赛中按时间划分），且整个测试集发布时未区分公开与私有部分。

近期为避免特定竞赛中测试数据被过度分析，Kaggle甚至暂缓发布完整测试数据，仅提供示例样本，待提交时替换为真实测试集。这类竞赛称为代码竞赛，因为参赛者实际提交的是生成预测的代码笔记本（Notebook），而非预测结果本身。

因此，模型生成的提交会覆盖整个测试集，但仅公开部分会即时评分，私有部分评分需待竞赛结束后进行。

由此产生三个关键考量：

- 为确保竞赛有效性，训练数据与测试数据应同源分布，且测试数据的公开与私有部分在分布上应相似。

- 即使训练与测试数据表面同源，若任一组样本不足，都可能导致训练数据与公开/私有测试数据的结果难以对齐。

- 应将公开测试数据视为数据科学项目中的保留测试集：仅用于最终验证。故应减少对其频繁查询，避免产生适应性过拟合——即模型在特定测试集表现优异却在其他集表现不佳的现象。

牢记这三项对理解竞赛机制至关重要。多数竞赛论坛中，关于训练数据与公开/私有测试数据关系的讨论层出不穷，常见数百个仅基于公开排行榜效果提交的解决方案。排名剧烈变动的"震荡"现象也常引发热议——这种最终排名的重组常使公开排行榜领先者大失所望。经验表明，震荡多源于训练集与测试集、或测试数据公开/私有部分间的差异。其评估方式包括：参赛者预期本地分数与排行榜反馈的事前相关性分析，以及基于两项指标的事后分析：

- 总体震荡指数：均值（绝对私有排名-公开排名）/参赛队伍总数

- 头部震荡指数：仅考量公开排名前10%的变动

这些事后指标由Steve Donoho（https://www.kaggle.com/breakfastpirate）首创，他编制了Kaggle最严重震荡排行榜（参见https://www.kaggle.com/c/recruit-restaurant-visitor-forecasting/discussion/49106#278831）。如今这些指标可通过第五章"竞赛任务与指标"讨论的Meta Kaggle数据集（见https://www.kaggle.com/jtrotman/meta-kaggle-competition-shake-up）轻松复现。例如查阅这些指标可知，RSNA颅内出血检测竞赛因剧烈震荡（尤其是头部排名）令众多参赛者叫苦不迭。

除事后评估外，过往震荡现象可为我们提供诸多Kaggle竞赛经验。加州大学伯克利分校的研究者也持此观点。在2019年NIPS会议上，Roelofs、Fridovich-Keil等学者通过分析数千场Kaggle竞赛，深入探究了公开-私有排行榜动态机制。尽管研究聚焦特定竞赛子集（120场，参与人数达标且专注二分类），但仍获得重要发现：

- 适应性过拟合现象较少：公开排名通常在私有排行榜揭晓后仍保持稳定

- 多数震荡源于随机波动及排名密集区：当竞争者分数接近时，私有测试集的微小性能变化会导致排名大幅变动

- 当训练集规模过小或数据非独立同分布（i.i.d.）时，易发生震荡现象

完整论文《机器学习中的过拟合问题元分析》（Roelofs, R., Fridovich-Keil, S. 等作者）发表于2019年\( {33}^{\mathrm{{rd}}} \)国际神经信息处理系统大会论文集，可通过此链接获取：https://papers.nips.cc/paper/2019/file/ee39e503b6bedf0c98c388b7e8589aca-Paper.pdf。

然而根据我们在Kaggle竞赛中的长期观察，自适应过拟合问题自始就屡见不鲜。例如可参阅Greg Park对我们早期参赛项目的分析报告：http://gregpark.io/blog/Kaggle-Psychopathy-Postmortem/。鉴于这是多数参赛者面临的普遍难题，我们建议采取比盲目跟随公开排行榜更精细的策略：

- 始终构建可靠的交叉验证系统进行本地评分

- 根据实际情况采用最佳验证方案控制非独立同分布数据。除非竞赛说明明确标注，识别非独立同分布特征并非易事，但可通过讨论或分层验证实验获取线索（例如当按特定特征分层时，结果显著改善）

- 对比本地评分与公开排行榜趋势的一致性

- 运用对抗性验证检测测试数据分布是否与训练数据相似

- 通过集成学习增强方案鲁棒性，尤其适用于小数据集场景

后续章节将逐一探讨这些方法（集成学习除外，该主题将在未来章节专述），并提供最优工具与策略以获取最佳结果，特别是在私有数据集上

## 竞赛中验证机制的重要性

若深入思考竞赛本质，可将其视为庞大的实验系统。谁能建立最系统高效的实验流程，谁就能胜出

事实上，尽管具备理论知识，你仍需与数百名实力相当的数据从业者竞争

他们使用相同的数据集和类似的学习工具（TensorFlow/PyTorch/Scikit-learn等）。虽然计算资源差异因Kaggle Notebooks和云计算成本下降而缩小，但在知识储备、数据模型和硬件设备方面已难形成显著优势。然而某些选手总能持续领先，暗示存在关键成功要素

访谈中，顶尖选手将其归因为"毅力"、"穷举尝试"或"全情投入"。这些说法看似玄妙，我们称之为系统化实验——成功关键取决于实验数量与执行方式。实验越多，解决方案越可能优于他人。这取决于可用时间、计算资源（虽非决定性因素）、团队规模及投入程度，印证了毅力与专注的成功法则

但实验方式同样影响结果。"快速失败并吸取教训"是竞赛要诀。无论成败都需深入反思，否则竞赛将沦为随机尝试

因此，在同等条件下，完善的验证策略是区分优秀选手与过拟合排行榜者的关键因素

验证是通过量化模型误差、评估实验效果改进的核心方法论

通常，选择适当验证方法的影响往往被忽视，人们更倾向于关注更具量化性的因素，比如拥有最新、最强大的GPU或更大的团队来提交成果。

然而，如果仅仅依赖实验的火力及其在排行榜上的结果，那就像是"往墙上扔泥巴，希望有些能粘住"（参见http://gregpark.io/blog/Kaggle-Psychopathy-Postmortem/）。有时这种策略会奏效，但大多数时候不会，因为你会错过在正确方向上进行实验的重要机会，甚至无法在那一团泥巴中发现你创造出的闪亮宝石。例如，如果过于专注于在公共排行榜上使用随机、非系统性的策略碰运气，即使你提出了出色的解决方案，最终也可能无法正确选择最终提交，从而在私有排行榜上错过得分最高的那个。

拥有适当的验证策略可以帮助你决定哪些模型应该提交以在私有测试集上排名。尽管提交在公共排行榜上表现最好的模型的诱惑可能很大，但始终要考虑你自己的验证分数。对于最终提交，根据具体情况以及你是否信任排行榜，选择基于排行榜的最佳模型和基于本地验证结果的最佳模型。如果你不信任排行榜（特别是当训练样本较小或样本非独立同分布时），提交具有两个最佳验证分数的模型，选择两个非常不同的模型或集成模型。这样，你将降低选择在私有测试集上表现不佳的解决方案的风险。

在指出了拥有实验方法的重要性之后，剩下的就是验证的实际操作问题了。事实上，当你建模一个解决方案时，你需要做出一系列相互关联的决策：

1. 如何处理你的数据

2. 应用什么模型

3. 如何改变模型的架构（尤其适用于深度学习模型）

4. 如何设置模型的超参数

5. 如何对预测进行后处理 即使公共排行榜与私有排行榜完全相关，每日提交次数的限制（所有比赛中都存在的限制）也会阻止你在上述所有领域进行可能的测试，甚至连皮毛都触及不到。拥有一个适当的验证系统可以事先告诉你你所做的是否可能在排行榜上有效。

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_179.jpg?x=245&y=469&w=355&h=358&r=0"/>

<!-- Media -->

## 德米特里·拉尔科

https://www.kaggle.com/dmitrylarko

德米特里·拉尔科（Dmitry Larko）是Kaggle竞赛特级大师，现任H2O.ai首席数据科学家。他拥有十余年机器学习和数据科学领域经验，于2012年12月发现Kaggle平台并在数月后参与首次竞赛。正如他在访谈中所言，他是Kaggle竞赛中验证机制的坚定倡导者。

您最青睐哪类竞赛？原因何在？就技术方法和解决路径而言，您在Kaggle平台的专业优势是什么？

我主要参与表格数据类竞赛，同时也热衷计算机视觉领域的赛事。

## 您如何规划Kaggle竞赛策略？这种策略与日常工作有何差异？

我总是从简单模型入手，先构建小型/简易模型的提交管道。关键步骤是建立恰当的验证方案，确保能稳健地验证各项设想。此外，投入充足时间进行数据检视与分析始终是明智之举。

在日常工作中，我负责构建AutoML平台，因此许多在Kaggle尝试的技术最终都会集成到这个平台中。

## 请分享您参与过最具挑战性的竞赛，以及攻克该任务的关键洞见

一时难以列举具体案例，但这并不重要——对我构成技术挑战的任务，对他人可能易如反掌。技术难度并非关键，重要的是理解竞赛如同马拉松而非短跑，或者您也可以视之为系列冲刺的马拉松。因此保持精力充沛、睡眠充足、坚持锻炼、通过公园散步激发新思路都至关重要。要赢得Kaggle竞赛，需要调动全部创造力与专业知识，有时还需要些许运气。

# Kaggle是否对您的职业发展有所助益？具体体现在哪些方面？

我现任职位正是得益于Kaggle竞赛特级大师的身份。对我的雇主而言，这个头衔足以证明我在该领域的专业造诣。

# 根据您的观察，新手Kaggle用户常忽视哪些要点？您希望初入行时了解哪些现在掌握的经验？

他们大多忽视正确验证方案的建立，盲目追随公开排行榜反馈。这往往导致糟糕结果，即Kaggle上所谓的"排名震荡"现象。

此外，他们常急于跳过探索性数据分析直接建模，致使解决方案流于表面，排行榜成绩平平。

## 您过往竞赛中曾犯过哪些错误？

我的主要错误与新手如出一辙——过度关注排行榜分数而忽略内部验证。每次做出这种选择，都导致我的排名下滑数位。

# 在数据分析或机器学习领域，您有哪些特别推荐的工具或库？

这些通常是首选工具。处理表格数据：LightGBM、XGBoost、CatBoost；深度学习领域：PyTorch、PyTorch-Lightning、timm；而Scikit-learn则是通用选择。

参加竞赛时最需要牢记或做到的关键事项是什么？

从简单开始，持续验证；相信你的验证分数而非排行榜分数。

## 偏差与方差

良好的验证系统能提供比训练集误差指标更可靠的评估标准。实际上，训练集获得的指标受每个模型的容量和复杂度影响。你可以将模型容量视为其从数据中学习的内存空间。每个模型都有帮助记录数据模式的内在参数集，不同模型提取模式的能力各异——有些能识别特定规则或关联，而另一些则发现其他规律。当模型从数据中提取模式时，会将其存储在"记忆"中。

模型的容量或表达能力常被表述为偏差与方差问题。此处模型的偏差和方差虽指向预测结果，但其核心原理与模型表达能力密切相关。模型可简化为将输入（观测数据）映射到结果（预测）的数学函数。不同数学函数的复杂度体现在参数数量和使用方式上：

- 当模型的数学函数不够复杂或缺乏足够表达能力来捕捉问题的复杂性时，就会出现偏差问题，因为预测结果会被模型自身的局限性所"偏倚"。

- 若模型核心数学函数对当前问题过于复杂，则会产生方差问题——模型会记录训练数据中过多不必要的细节和噪声，导致预测结果受其过度影响而变得不稳定。

当今机器学习技术发展和计算资源支持下，问题往往源于方差。因为最常用的深度神经网络和梯度提升方法，其数学表达能力通常远超解决大多数实际问题所需。

当模型提取完所有有用模式后若仍有剩余容量，就会开始记忆与预测无关的数据特征和信号（通常称为噪声）。虽然初始提取的模式有助于模型泛化到测试数据集并提升预测准确性，但专门针对训练集学习的非泛化性内容反而可能损害性能。这种学习无泛化价值训练集元素的过程被称为过拟合。

验证的核心目的是明确定义一个分数或损失值，将可泛化部分与过拟合训练集特性导致的部分区分开来。

这就是验证损失。通过下图学习曲线可以直观理解这种情况：

<!-- Media -->

<!-- figureText: Overfitting starts from here Training loss Iterations -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_182.jpg?x=353&y=347&w=1173&h=917&r=0"/>

图6.1：从训练数据中学到更多并不总意味着学会预测

<!-- Media -->

若以\( y \)轴表示损失度量，\( x \)轴表示模型学习程度（神经网络中的epoch或梯度提升中的轮次），你会观察到训练数据集上学习似乎持续进行，但其他数据上并非如此。

即使改变超参数、处理数据或完全更换模型，这种现象依然存在。曲线形态会变化，但总会存在过拟合开始的临界点。该点位置因模型选择和处理方式而异。若通过正确验证策略准确计算出过拟合起始点，模型表现必与排行榜结果（公开和私有）相关，且验证指标能让你无需提交即可评估工作成效。

过拟合可能发生在不同层面：

- 在训练数据层面，当你使用的模型对问题而言过于复杂时

- 在验证集本身层面，当你针对特定验证集过度调整模型时

- 在公开排行榜层面，当结果与训练预期相差甚远时

- 在私有排行榜层面，尽管公开排行榜成绩优异，私有评分却令人失望时

虽然具体含义略有差异，但都同样意味着模型缺乏泛化能力，正如本节所述。

## 尝试不同的划分策略

如前所述，验证损失基于训练集之外的数据样本。这个经验性指标能反映模型的预测能力，相比训练得分更能说明问题——后者主要体现模型对训练数据模式的记忆程度。正确选择验证数据样本构成了验证策略的核心。

总结正确验证模型和评估性能的策略，你有几种选择：

- 第一种是采用保留集方法，但存在未能正确选择代表性数据样本或对验证集过拟合的风险

- 第二种是采用概率方法，通过系列样本来评估模型。概率方法包括交叉验证、留一法(LOO)和自助法。交叉验证策略中，根据数据特性（简单随机抽样、分层抽样、分组抽样、时间抽样）又存在不同变体

这些策略的共同点在于都是抽样策略。它们帮助基于随机选取的小部分数据来推断总体指标（模型性能）。抽样是统计学基础，并非精确过程——根据抽样方法、可用数据及选取特定案例的随机性，总会存在一定误差。例如依赖有偏样本可能导致评估指标被高估或低估。但若设计实施得当，抽样策略通常能提供良好的总体估计

另一个共同点是它们都采用互斥划分，将案例严格归入训练集或验证集。由于多数模型具有记忆能力，在训练和验证中使用相同案例会导致评估虚高——我们真正需要评估的是模型对未见样本的规律推导能力

## 基础训练-测试划分

我们将分析的第一种策略是训练-测试划分。该策略从训练集中抽样部分数据（称为保留集），将其作为测试集来评估所有使用剩余数据训练的模型

该策略的最大优势是简单直接：选取部分数据作为检验标准。通常按80/20比例划分训练集，Scikit-learn中通过train_test_split函数实现。需要注意几个关键点：

- 当数据量充足时，抽取的测试数据通常能代表整体分布。但由于抽取过程具有随机性，仍可能获得非代表性样本——尤其当初始训练样本较小时。通过对抗性验证比较划分结果（后续章节详述），可确保评估方式正确

此外，为确保测试抽样具有代表性（特别是训练数据与目标变量的关联性），可采用分层抽样技术。该技术能保证抽样数据中特定特征的比例与原数据集一致。在train_test_split函数中，可通过stratify参数传入类别分布数组来实现这一目标。

需要特别指出的是，即使拥有代表性保留集，单纯使用训练-测试分割仍可能无法确保竞赛中成果评估的准确性。事实上，频繁在该测试集上验证会导致"适应性过拟合"（即错误地将训练集噪声误判为有效信号），这与在公开排行榜持续评估时出现的问题类似。因此，虽然计算成本更高，但概率性评估方法更适合竞赛场景。

## 概率性评估方法

机器学习模型的概率性评估基于分布样本的统计特性。抽样过程会生成一个保持原数据特征的小型数据集，而未参与抽样的部分本身也构成具有相同统计特性的样本。通过在抽样数据上反复训练测试模型，本质上是在构建衡量模型性能的统计估计量。每个样本都可能存在"误差"（即不能完全代表原始数据的真实分布），但随着抽样次数增加，多个样本估计量的均值将收敛于待估量的真实均值（这种现象在概率论中由大数定律解释）。

虽然概率性估计量比简单训练-测试分割需要更多计算资源，但能提供更可靠的模型泛化性能评估。

## K折交叉验证

最常用的概率性验证方法是\( k \)折交叉验证，该方法能准确评估模型在相同分布未见过测试数据上的表现。

这一观点在Bates、Hastie和Tibshirani的论文《Cross-validation: what does it estimate and how well does it do it?》（arXiv预印本arXiv:2104.00673，2021年）中有详细阐述。

\( k \)折交叉验证既能有效比较预测模型，也可用于选择测试集表现最优的模型超参数。

虽然存在多种\( k \)折交叉验证变体，但Scikit-learn中KFold函数实现的最简版本会将训练数据划分为\( k \)个子集。经过\( k \)轮迭代，每轮取一个子集作为测试集，其余用于训练。最终将\( k \)个验证分数取平均，所得\( k \)折验证分数即模型在未知数据上的预估平均性能，其标准差则反映估计的不确定性。图6.2展示了5折交叉验证的结构：

<!-- Media -->

<!-- figureText: Fold 1 validation train train validation train validation train validation Fold 2 train validation Fold 3 train Fold 4 train Fold 5 train -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_186.jpg?x=364&y=448&w=1143&h=546&r=0"/>

图6.2：5折验证方案结构示意图

<!-- Media -->

需注意\( k \)折交叉验证分数的重要特性：它估计的是基于\( k \)-1折数据训练的模型平均性能。若后续使用全量数据训练模型，该验证估计将失效。当\( k \)接近样本数量\( n \)时，虽能获得基于完整训练集的更准确估计，但由于各折估计值间相关性增强，将丧失所有概率性验证意义。此时得到的仅是模型在训练数据上的表现指标（虽可用于比较，但无法有效评估模型泛化能力）。

当采用\( k = n \)时，您将使用留一法（LOO）验证方法，该方法在样本量较少时尤为实用。该方法基本是无偏拟合度量，因为它使用几乎所有可用数据训练而仅用一个样本测试。但它并不能有效评估模型在未知数据上的预期表现。其在整个数据集上的重复测试结果高度相关，因此LOO指标更多反映模型在当前数据集上的性能，而非在未知数据上的表现。

选择正确的\( k \)分区数量需基于现有数据的几个关键维度：

- \( k \)值越小（最小为2），每个折叠集规模越小，导致基于\( k - 1 \)折训练模型的偏差越大：相较于更大\( k \)训练的模型，在小\( k \)上验证的模型性能会有所下降。

- \( k \)值越大，数据量虽增加但验证评估相关性越强：您将丧失\( k \)折交叉验证在预测未知数据性能时的优势特性。

通常\( k \)设为5、7或10折，极少采用20折。竞赛中一般选择\( k = 5 \)或\( k = {10} \)折（后者每次训练使用\( ({90}\% \)比例数据），更适用于评估模型在全量数据重训练时的表现。

在竞赛中为特定数据集选择\( k \)值时，建议从两个维度考量：

首先，折数选择应匹配目标需求：

- 若为性能评估，需低偏差估计模型（避免系统性估计失真）。建议采用较高折数（通常10-20折）。

- 若为参数调优，需平衡偏差方差，推荐中等折数（通常5-7折）。

- 若仅需变量筛选简化数据，低方差估计模型即可（避免结果分歧），3-5折足够。

当数据量较大时，可酌情选择建议范围中的较小值。

其次，若专注性能评估需注意：折数越多验证集样本越少，各折评估结果相关性越强。超过临界点后，增加\( k \)会使交叉验证结果更反映训练集表现而非测试集预测能力。这也意味着更多折数能获得完美的堆叠（stacking）用折外预测（详见第9章《混合与堆叠集成方案》）。在Kaggle竞赛中，\( k \)折交叉验证不仅用于验证方案和评估模型，还能生成预测结果。交叉验证本质是子采样，对多个子模型结果取平均是降低方差的有效策略（常优于全量数据训练，第9章将详述）。因此许多选手直接使用交叉验证生成的模型对测试集进行预测并集成。

## k折变体

由于基于随机采样，\( k \)折在以下场景可能产生不理想分割：

- 需保持小类样本比例（目标变量或特征层面）。常见于目标变量高度不平衡场景，如垃圾邮件数据集（垃圾邮件占比极小）或需预测低频违约事件的信贷风险数据。

- 需保持数值变量分布（目标变量或特征层面）。多见于存在严重偏态或长尾分布的回归问题，如房价预测中总有少量远高于均价的在售房源。

- 您的案例属于非独立同分布(non-i.i.d)情况，特别是在处理时间序列预测时。

前两种场景的解决方案是分层\( k \)折交叉验证，通过受控采样保持需要保留的数据分布。若需保持单一类别的分布，可使用Scikit-learn的StratifiedKFold，通常以目标变量或需要保持分布的特征作为分层变量。该函数将生成索引集帮助数据分区。对连续变量，可先使用pandas.cut或Scikit-learn的KBinsDiscretizer进行离散化处理。

当涉及多变量分层或重叠标签（如多标签分类）时更为复杂。Scikit-multilearn包(http://scikit.ml/)中的IterativeStratification命令可解决此问题，它能控制需要保留的多变量组合比例顺序(http://scikit.ml/api/skmultilearn.model_selection.iterative_stratification.html)。该算法基于以下论文：

- Sechidis, K., Tsoumakas, G., 和 Vlahavas, I. (2011). 《多标签数据分层方法》. 《机器学习与知识发现在数据库中》, 145-158. http://lpis.csd.auth.gr/publications/sechidis-ecmlpkdd-2011.pdf

- Szymański, P. 和 Kajdanowicz, T.; 《第一届不平衡领域学习国际研讨会论文集》, PMLR 74:22-35, 2017. http://proceedings.mlr.press/v74/szyma%C5%84ski17a.html

即使处理回归问题，分层仍大有可为。回归问题中使用分层能确保交叉验证时拟合的目标变量（或预测变量）分布与整体样本相似。此时需将连续目标变量转换为离散代理变量才能使StratifiedKFold正常工作。

最简单的方法是使用pandas.cut函数将目标变量划分为足够数量的区间（如10或20个）：

---

import pandas as pd

y_proxy = pd.cut(y_train, bins=10, labels=False)

---

Abhishek Thakur推荐根据样本量采用Sturges规则确定分箱数量，再传入pandas.cut函数(参见https://www.kaggle.com/abhishek/step-1-create-folds)：

---

import numpy as np

bins = int(np.floor(1 + np.log2(len(X_train))))

---

另一种方法是聚焦训练集特征分布，通过聚类分析（无监督方法）对排除目标变量和标识符后的特征进行聚类，将预测簇作为分层依据。参考该Notebook示例(https://www.kaggle.com/lucamassaron/are-you-doing-cross-validation-the-best-way)：先进行PCA主成分分析消除相关性，再执行\( k \)均值聚类分析。可通过实验确定最佳聚类数。对于\( k \)折交叉验证不适用的情况——第三种非独立同分布(non-i.i.d)数据场景（如样本存在分组关联时）尤为棘手。非独立同分布样本的特征和目标存在组内相关性（已知组内某个样本即可较易预测组内其他样本）。若同一组被分割到训练集和验证集，模型可能学会区分组别而非目标本身，导致验证分数虚高而实际预测效果差。此时应使用GroupKFold：通过指定分组变量，确保每个组完整出现在训练折或验证折中。

发现导致数据非独立同分布(non-i.i.d.)的分组结构并非易事。除非竞赛题目明确说明，否则您需要依靠自身能力来探查数据（使用无监督学习技术，如聚类分析）并结合问题领域知识。例如，若数据涉及移动电话使用情况，您可能通过特征中连续出现的相似值意识到某些样本来自同一用户。时间序列分析面临同样问题，由于数据非独立同分布，您无法通过随机抽样进行验证——这会混淆不同时间段的数据，且后期时间帧可能包含前期痕迹（统计学中称为自相关特征）。最基本的时间序列验证方法是基于时间划分训练集与验证集，如图6.3所示：

<!-- Media -->

<!-- figureText: train validation test test public private time -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_190.jpg?x=306&y=1395&w=1274&h=274&r=0"/>

图6.3：训练集与验证集基于时间划分

<!-- Media -->

但您的验证能力将受限制，因为验证会固定在特定时间段。更复杂的方法是使用时序分割验证TimeSeriesSplit，如Scikit-learn包提供的sklearn.model_selection.TimeSeriesSplit。该功能可帮助设定时间序列中训练与测试部分的时间范围：对于训练时段，您可选择包含测试时段前所有历史数据，或限定固定回溯期（例如始终使用测试时段前三个月的数据进行训练）。

图6.4展示了基于时间的验证策略结构，包含逐步扩大的训练集和移动验证集：

<!-- Media -->

<!-- figureText: Fold 1 train validation test test public private validation test test public private validation test test public private time Fold 2 train Fold 3 train -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_191.jpg?x=292&y=577&w=1278&h=510&r=0"/>

图6.4：训练集随时间推移逐步扩大

<!-- Media -->

而在图6.5中，您可以看到当规定训练集采用固定回溯期时策略的变化：

<!-- Media -->

<!-- figureText: Fold 1 train validation test test public private validation test test public private validation test test public private time Fold 2 train Fold 3 train -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_191.jpg?x=292&y=1308&w=1283&h=537&r=0"/>

图6.5：训练集与验证集随时间推移移动

<!-- Media -->

根据我们的经验，采用固定回溯期能更公平评估时间序列模型，因为始终依赖相同规模的训练集。若随时间推移扩大训练集规模，会将模型性能随时间切片的变化与模型偏差减少（样本越多偏差越小）的影响混为一谈。

最后请记住，可以设置TimeSeriesSplit来保持训练与测试时间的预设间隔。当测试集位于未来特定时段时（例如训练数据后一个月），这非常有用——它能验证模型是否具备足够鲁棒性进行远期预测。

## 嵌套交叉验证

此处需要引入嵌套交叉验证。此前我们仅讨论了模型最终性能测试，但调参过程中常需评估中间性能。实际上，不能先用测试集验证特定参数效果，又用相同数据评估最终性能——因为针对该测试集优化的参数会使评估结果过于乐观，换用其他测试集很可能得不到相同结果。此时必须区分验证集（用于评估不同模型及超参数性能）和测试集（用于估计模型最终性能）。

若采用训练-测试分割，需将测试部分再分为两部分。典型比例为\( {70}/{20}/{10} \)分别用于训练、验证和测试（可自定义）。若使用交叉验证，则需嵌套交叉验证——即在另一个交叉验证的分割基础上再进行交叉验证。本质上，常规交叉验证运行时，当需要评估不同模型或参数时，需基于该折数分割再次运行交叉验证。

图6.6示例展示了这种内外交叉验证结构。外部循环确定用于测试评估指标的数据部分；内部循环则基于外部循环的训练数据，通过训练/验证分割来评估和优化特定模型选择（如决定采用哪种模型或超参数值）：

<!-- Media -->

<!-- figureText: Fold 1 validation train train dool AD (eu：03 kg train validation train validation train doo| AJ |euuә:u| validation Fold 2 train validation Fold 3 train validation Fold 4 train Fold 5 train validation train train validation train -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_193.jpg?x=239&y=208&w=1401&h=1163&r=0"/>

图6.6：嵌套交叉验证在外部循环与内部循环中的结构

<!-- Media -->

这种方法能确保测试和参数搜索完全可靠，但会带来两个问题：

- 训练集规模缩减，因为先进行交叉验证分割，然后再次分割

- 更重要的是需要大量建模工作：若运行两层10折交叉验证，需训练100个模型。因此部分Kaggle选手会忽略嵌套交叉验证，冒险用相同交叉验证既搜索模型/参数又评估性能，或固定测试样本进行最终评估。根据经验，这种方法虽可行，但若将折外预测用于后续建模（下节将讨论），可能导致高估性能及过拟合。我们建议根据情况选择最佳方法——若要准确评估模型性能并将其预测用于其他模型，请记住嵌套交叉验证能提供过拟合更少的解决方案，在某些比赛中可能成为制胜关键。

## 生成折外预测(OOF)

交叉验证除评估指标性能外，还有个妙用是生成测试预测和折外预测。实际上，当在部分训练数据上训练并对剩余部分预测时，你可以：

- 对测试集预测：所有预测的平均值通常比在全量数据上重新训练相同模型更有效——这是与混搭(blending)相关的集成技术，第9章《混搭与堆叠解决方案的集成》将详细讨论

- 对验证集预测：最终会获得完整训练集的预测，可按原始训练数据顺序重组。这些预测通常称为折外(OOF)预测，极具实用价值

OOF预测的首要用途是评估性能——可直接在其上计算评估指标。该性能不同于交叉验证估计值（基于抽样），不具备相同概率特性，不能作为泛化性能的有效度量，但能反映模型在特定训练集上的表现。

第二个用途是生成预测结果与真实值或其他模型预测的对比图表，这有助于理解各模型的工作原理及其预测相关性。

最终用途是创建元特征或元预测器。虽然第九章将深入探讨，但需特别指出：袋外预测是交叉验证的副产品，其有效性源于模型在验证阶段始终预测训练时未接触的样本。由于每个袋外预测均由不同数据子集训练的模型生成，这些预测不存在偏差且无需担心过拟合（但下章将讨论某些注意事项）。

生成袋外预测有两种方法：

- 编写程序将验证预测存入向量，并确保其索引位置与训练数据样本严格对应

- 使用Scikit-learn的cross_val_predict函数自动生成袋外预测

本章后续探讨对抗验证时，将实际演示第二种技术。

## 子抽样法

除\( k \)折交叉验证外，还有其它验证策略但泛化性能不同。前文讨论的LOO（留一法）即\( k = \)\( n \)（\( n \)为样本量）的特例。另一种选择是子抽样：类似\( k \)折交叉但无固定折数，根据经验设定抽样次数，每次用抽样数据训练、未抽样数据验证，通过平均各次评估指标获得模型性能估计。

由于需系统性覆盖所有样本（如\( k \)折交叉），实际需要大量试验才能充分测试。若抽样不足，某些样本可能被重复测试。可通过Scikit-learn的ShuffleSplit实现此类验证。

## 自助法

最后还可采用统计学中的自助法，该方法本用于估计统计量的误差分布，同样适用于性能评估。自助法要求进行有放回抽样且样本量与原数据相同，具体有两种应用方式：

- 统计传统用法：多次自助抽样后，在抽样数据上训练模型并计算训练集评估指标，最终取多次结果的平均值

- 类子抽样法：用自助样本训练，未抽样部分作为测试集

实践中，第一种方法（常用于线性模型系数估计）对机器学习效果有限，因多数算法易过拟合训练数据。为此Efron与Tibshirani（参见《交叉验证改进：632+自助法》）提出632+估计量作为最终验证指标。

最初他们提出简化版632自助法：

\[{\text{ Err }}_{.632} = {0.368} * {\text{ err }}_{\text{fit }} + {0.632} * {\text{ err }}_{\text{bootstrap }}\]

该公式中err表示评估指标，err\( {}_{fit} \)为训练数据指标，\( {\text{err}}_{\text{bootstrap }} \)为自助数据指标。但当训练模型过拟合时err\( {}_{fit} \)趋近零导致估计失效，因此改进推出632+自助法：

\[{\operatorname{Err}}_{.632} + \left( {1 - w}\right)  * {\operatorname{err}}_{\text{fit }} + w * {\operatorname{err}}_{\text{bootstrap }}\]

其中 \( w \) 为：

\[w = \frac{0.632}{1 - {0.632R}}\]

\[R = \frac{{\text{ err }}_{\text{bootstrap }} - {\text{ err }}_{\text{fit }}}{\gamma  - {\text{ err }}_{\text{fit }}}\]

此处引入新参数\( \gamma \)，即无信息错误率，通过评估预测模型在所有目标变量与预测变量组合上的表现得出。如Scikit-learn开发团队所述(https://github.com/scikit-learn/scikit-learn/issues/9153)，计算\( \gamma \)确实存在计算复杂度问题。鉴于传统统计学的bootstrap方法在机器学习应用中的局限性和计算不可行性，可采用第二种方法——通过bootstrap未采样的剩余样本进行评估。

这种形式的bootstrap可作为交叉验证的替代方案，但与子采样类似，其需要构建和测试的模型数量远超交叉验证。然而当交叉验证显示评估指标方差过高时，了解此类替代方案仍有价值，以便通过反复测试进行更严格的验证。

该方法曾实现在Scikit-learn中(https://github.com/scikit-learn/scikit-learn/blob/0.16.X/sklearn/cross_validation.py#L613)但后续被移除。鉴于Scikit-learn中已无bootstrap功能且其原实现会对测试数据也进行重采样，可采用我们自定义的实现方案。示例如下：

<!-- Media -->

---

import random

def Bootstrap(n, n_iter=3, random_state=None):

	"""

带替换的随机抽样交叉验证生成器

每次迭代生成索引\( \lbrack 0,\mathrm{\;n}) \)的bootstrap样本

函数返回获得的样本

及所有被排除索引的列表

	"""

if random_state:

random.seed(random_state)

for j in range(n_iter):

bs = [random.randint(0, n-1) for i in range(n)]

out_bs = list(\{i for i in range(n)\} - set(bs))

yield bs, out_bs

---

<!-- Media -->

总之，自助法（bootstrap）确实是交叉验证的有效替代方案。它在统计学和金融领域应用更为广泛。在机器学习中，黄金法则是采用\( k \)折交叉验证法。但我们建议，当遇到异常值或样本异质性过高导致交叉验证的评估指标标准误差过大时，不应忽视自助法的价值——这种情况下，自助法在模型验证中将展现出更大的实用性。

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_198.jpg?x=249&y=233&w=355&h=357&r=0"/>

<!-- Media -->

## 瑞恩·切斯勒

https://www.kaggle.com/ryches

本章第二位访谈对象是瑞恩·切斯勒，他是Kaggle论坛特级大师、笔记本与竞赛专家，现任H2O.ai数据科学家，同时担任圣地亚哥机器学习Meetup小组（https://www.meetup.com/San-Diego-Machine-Learning/）的组织者之一。在他的多个回答中都强调了验证环节的重要性。

## 您最青睐哪种类型的竞赛？为什么？在技术方法和解决思路上，您在Kaggle的专长是什么？

我倾向于涉猎各类竞赛。比起专攻计算机视觉或自然语言处理等特定领域，接触多样化的问题更有趣。最吸引我的是那些能从数据和预测误差中挖掘深层洞见的竞赛。对我而言，误差分析是最具启发性的过程——通过理解模型失败的原因，尝试改进模型或输入数据表征来弥补缺陷。

## 您如何着手应对Kaggle竞赛？这与日常工作方法有何不同？

我的方法论在两者间是相通的。许多人喜欢在建模前进行探索性数据分析，但我发现数据预处理过程通常已足够。我的典型做法是人工检视数据，初步判断最佳建模方向及可探索选项，随后构建模型评估性能，最后聚焦分析误差并根据模型弱点规划后续改进步骤。

## Kaggle对您的职业发展有帮助吗？具体体现在？

是的，它助我获得了现职。H2O非常看重Kaggle成就，我前雇主也曾因我的竞赛表现而青睐于我。

## 您还组织着圣地亚哥两千多人参与的Meetup活动，这与Kaggle经历有关吗？

当然密切相关。我最初知识匮乏，首次参赛成绩惨淡。后来通过本地Meetup结识队友并向他们学习，当时与水平远超我的伙伴合作取得了4500多支队伍中第三名的佳绩。原小组解散后，为延续社区活力我自立门户组织活动，四年来角色转变为教学指导。我们最初专注Kaggle组队参赛，现已拓展至读书会和主题讲座。每周固定研究机器学习的时间，是我成功的重要基石。

## 据您观察，新手常忽视哪些要点？哪些经验您希望初学时就知道？

许多人过度强调偏差-方差权衡和过拟合问题，这其实是被过分担忧的。重点不应追求训练集与验证集表现相近，而应全力优化验证集性能。

## 您过去在竞赛中犯过哪些错误？

我的通病是探索不足。有时过早否定某些想法，后来却发现它们对提升性能至关重要。往往首次尝试就能接近竞争力水平，但持续迭代改进需要另一种我正在磨练的技能。

## 有哪些特别推荐的数据分析或机器学习工具/库？

我常用标准工具：XGBoost、Light GBM、PyTorch、TensorFlow和Scikit-learn。对特定工具或库没有特别偏好，只选择适合解决问题的方案。

## 参加竞赛时最需要牢记的关键事项是什么？

我认为最重要的是保持清醒的验证意识。常见情况是，人们误以为模型性能在提升，但提交排行榜后才发现实际效果与预期不符。关键技能在于理解如何让假设适配新数据，并构建能适应新环境的稳健模型。

## 优化模型验证系统

此时你应已掌握所有可能的验证策略全景。参赛时需设计并实施验证方案，随后检验所选策略的正确性。

黄金法则是：设计验证策略时，必须模拟竞赛主办方划分训练集、私有测试集和公开测试集的方法。思考主办方如何进行数据分割——是随机抽样？还是保持特定数据分布？测试集是否与训练数据同分布？

这些问题在真实项目中不会出现。与不惜代价追求泛化能力的实际项目不同，竞赛更聚焦模型在给定测试集（尤其是私有集）的表现。若从一开始就专注于此，就更可能找到最佳验证策略，从而提升竞赛排名。

这是个试错过程。寻找最佳验证策略时，可系统应用以下两项一致性检验来判断方向是否正确：

1. 首先检查本地测试的一致性：交叉验证各折误差不应差异过大；若采用简单训练-测试分割，不同分割应能复现相同结果

2. 其次确认本地验证误差与公开排行榜结果是否一致

若首项检验未通过，可根据问题根源选择以下方案：

- 训练数据不足

- 数据过于分散且各训练分区差异显著（如存在高基数特征——像邮政编码这类多层级特征，或存在多元离群值）。这两种情况本质都是数据量不足以支撑目标模型。即使问题看似仅是数据过于分散，绘制学习曲线也会清晰表明模型需要更多数据。

此时，除非发现改用简单算法能提升评估指标（但用偏差替代方差可能降低模型性能，并非总是如此），最佳选择是采用扩展验证方案：

- 增大\( k \)值（当\( k = n \)时接近留一法）。虽然这会降低模型在未见数据上的表现评估，但通过使用更大训练集可获得更稳定的评估结果

- 对多次\( k \)折验证结果取平均（基于不同随机种子初始化的数据分区）

- 使用重复自举法。

请注意，当您发现不稳定的本地验证结果时，您并非唯一遭遇此问题的人。通常这是由于数据来源和特性导致的共性问题。持续关注讨论论坛，您可能获得解决方案的线索。例如针对高基数特征可采用目标编码；分层抽样有助于处理异常值等。

若您通过首次检验却未通过二次验证——即本地交叉验证结果稳定但与排行榜表现不符——则需另当别论。为发现该问题，必须详细记录所有实验、验证测试类型、使用的随机种子及提交预测后的排行榜结果。通过绘制散点图并尝试线性回归拟合，或更简单地计算本地结果与公开排行榜得分的相关性，您能进行关键性的竞赛表现元分析。尽管标注分析工作耗时，这却是追踪竞赛表现最重要的方法。

当验证分数持续低于或高于排行榜分数时，这强烈暗示您的验证策略存在缺失，但该问题不妨碍模型优化。您可继续改进模型并期待排行榜反映进展（尽管非线性相关）。但系统性差异始终是危险信号，意味着您的操作与主办方的测试设计存在根本差异。更糟糕的是本地交叉验证与排行榜反馈完全无关的情况——这必须立即触发系列测试调查。无论是否普遍问题，该状况都会严重威胁最终排名。可能原因包括：

- 测试集与训练集分布不同。对抗性验证测试（下节讨论）能有效应对此情况。

- 数据非独立同分布但未明示。例如在自然保护协会渔业监测竞赛中，训练集图像均取自渔船相似场景，需自行设计方法避免模型误学目标标识而非图像上下文（参见Anokas的方案）。

- 特征多元分布相同但测试集中某些组别分布有异。若能识别差异并相应调整训练集与验证策略，即可获得优势。这需要通过对公开排行榜的探测分析来实现。

- 测试数据存在漂移或趋势（时序预测常见）。同样需探测公开排行榜，通过后处理手段（如预测值乘数调整）模拟测试数据的递减/递增趋势来提升分数。

如前所述，排行榜探测是通过特殊设计的提交来推断公开测试集构成的技术。当私有测试集与公开集相似时效果尤佳。探测方法需根据竞赛类型具体设计，不存在通用方案。

例如Jacob在论文《利用对数损失预言攀登Kaggle排行榜》中阐述了如何在不下载训练数据的情况下获得竞赛第四名。

针对回归问题，在Kaggle近期举办的"30天机器学习"活动中，Hung Khoi演示了如何通过排行榜探测理解训练集与公开测试集目标列均值及标准差的差异。

他使用以下方程：

\[{RMS}{E}^{2} = {MSE} = \text{ variance } + {\left( \text{ mean } - {\text{ guessed }}_{\text{value }}\right) }^{2}\]

由于仅有两个未知项（方差与均值），理论上只需两次提交即可求解测试目标的均值与方差。

您还可以从Chris Deotte（https://www.kaggle.com/cdeotte）的这篇文章中获取关于排行榜探测的其他思路，该文与Don't Overfit II竞赛（https://www.kaggle.com/c/dont-overfit-ii）相关：https://www.kaggle.com/cdeotte/lb-probing-strategies-0-890-2nd-place。

若想了解从排行榜探测信息如何成为一把双刃剑，您可以阅读Zahar Chikishev如何在LANL地震预测竞赛中实施探测策略——他在公开排行榜领先却最终在私有排行榜跌至\( {87}^{\text{th }} \)名的案例：https://towardsdatascience.com/how-to-lb-probe-on-kaggle-c0aa21458bfe

## 使用对抗性验证

如前所述，交叉验证能测试模型对与训练数据同分布未见数据集的泛化能力。理论上，Kaggle竞赛要求构建的模型需在公开和私有数据集上预测，因此测试数据应与训练数据同分布。但实际情况往往并非如此。

即便您没有过度拟合测试数据——因为决策依据不仅包含排行榜结果，还考虑了交叉验证——结果仍可能出人意料。当测试集与建模所用的训练集存在细微差异时，这种情况就会发生。事实上，目标概率及其分布、以及预测变量与它的关联方式，会在训练过程中向模型传递某些预期；若测试数据与训练数据不同，这些预期将无法满足。

因此，仅避免前文讨论的排行榜过拟合并不足够。首要任务是确认测试数据是否与训练数据具有可比性。若存在差异，则需评估能否通过某种方法缓解训练与测试数据间的分布差异，从而构建适用于该测试集的模型。

对抗性验证(Adversarial validation)正是为此而生。这项技术能便捷评估训练与测试数据的差异程度，曾在Kaggle参赛者间秘密流传，直至Zygmunt Zajqc（https://www.kaggle.com/zygmunt）在其FastML博客公开。

原理很简单：移除训练数据的目标变量，将其与测试数据合并，新建二元分类目标（测试数据标记为正例）。运行机器学习分类器后，用ROC-AUC指标评估（该指标在前文"竞赛任务与指标详解"章节已讨论）。

若ROC-AUC约0.5，表明训练与测试数据难以区分，应属同分布。当数值高于0.5趋近1.0时，意味着算法能轻易区分数据来源——此时别指望模型能良好泛化，因为测试集显然来自不同分布。

Sberbank俄罗斯房产大赛（https://www.kaggle.com/c/sberbank-russian-housing-market）的示例Notebook（https://www.kaggle.com/konradb/adversarial-validation-and-other-scary-terms）演示了对抗性验证的实战应用。

由于数据类型可能不同（数值型/字符串型）且存在缺失值，运行分类器前需进行数据处理。建议使用随机森林分类器，原因如下：

- 它不输出真实概率，但结果天然有序，与ROC-AUC评分完美适配。

- 这种基于决策树的灵活算法能自主特征选择，无需预处理即可处理混合特征类型（同时将数据数值化），且抗过拟合性强，无需过多调整超参数。

- 基于树结构的特性使其对数据处理需求较低：缺失值可用-999等异常值替代；字符串变量通过标签编码器（如Scikit-learn的LabelEncoder）转为数值。虽效果不及独热编码，但速度快且能可靠解决问题。

除分类模型外，亦可采用其他方法。例如NanoMathias（https://www.kaggle.com/nanomathias）提出的方案（https://www.kaggle.com/nanomathias/distribution-of-test-vs-training-data）——通过t-SNE和PCA将数据映射到低维空间。虽需更多调参，但能生成直观的可视化图表。

请记住：人脑对视觉模式的识别能力远胜数值分析（关于人类视觉能力的深入探讨参见https://onlinelibrary.wiley.com/doi/full/10.1002/qua.24480）。

PCA和t-SNE并非唯一能帮助降低数据维度并实现可视化的工具。UMAP（https://github.com/1mcinnes/umap）常能提供更快速的低维解决方案，并呈现清晰的数据聚类。变分自编码器（详见第7章《表格竞赛建模》）则能处理非线性降维，提供比PCA更具实用性的表征方式，但其配置和调参过程更为复杂。

## 示例实现

虽然您可以在Zygmunt的原始文章和我们链接的Notebook中找到对抗性验证的案例，但我们基于Kaggle竞赛"Tabular Playground Series - Jan 2021"（https://www.kaggle.com/c/tabular-playground-series-jan-2021）为您创建了新示例。

首先导入Python包并获取竞赛的训练数据与测试数据：

---

import numpy as np

import pandas as pd

from sklearn.ensemble import RandomForestClassifier

from sklearn.model_selection import cross_val_predict

from sklearn.metrics import roc_auc_score

train = pd.read_csv("../input/tabular-playground-series-jan-2021/train.csv")

test = pd.read_csv("../input/tabular-playground-series-jan-2021/test.csv")

---

数据准备过程简洁明了：所有特征均为数值型，无需标签编码，但需用负数（通常取-1）填充缺失值，并移除目标列及标识列——当标识列为递增值时，对抗性验证可能返回较高的ROC-AUC分数：

---

train = train.fillna(-1).drop(["id", "target"], axis=1)

test = test.fillna(-1).drop(["id", axis=1])

X = train.append(test)

y = [0] * len(train) + [1] * len(test)

---

此时，您只需使用cross_val_predict函数为数据生成RandomForestClassifier预测，该函数会自动创建交叉验证方案并存储验证折叠上的预测结果：

---

model = RandomForestClassifier(   )

cv_preds = cross_val_predict(model, X, y, cv=5, n_jobs=-1,

method='predict_proba')

---

最终您将获得无偏预测（由于未在训练数据上预测，故不存在过拟合），这些预测可用于误差估计。请注意cross_val_predict不会拟合您实例化的模型，因此无法从中获取诸如模型重要特征等信息。如需此类信息，需先通过model.fit(X,y)进行拟合。

最后可查询预测结果的ROC-AUC分数：

---

print(roc_auc_score(y_true=y, y_score=cv_preds[:,1]))

---

您将获得约0.49-0.50的值（除非使用固定random_seed的交叉验证，否则cross_val_predict结果非确定性）。这表明难以区分训练数据与测试数据，二者源自相同分布。

## 处理训练数据与测试数据的不同分布

当ROC-AUC分数达到0.8或更高时，意味着测试集存在特殊性且与训练数据明显可区分。此时可采取以下策略：

- 特征抑制

- 选择与测试集最相似的样本进行训练

- 通过模拟测试集进行验证

特征抑制需迭代移除对抗性测试集中影响最大的变量，直至分布重新一致。具体流程：拟合全量数据→检查特征重要性（如Scikit-learn的feature_importances_method）和ROC-AUC拟合分数→移除最重要变量→重复该循环，直至拟合ROC-AUC分数降至0.5左右。

此方法的局限在于可能被迫移除大部分重要变量，导致基于筛选后数据构建的模型因信息特征缺失而预测失准。

选择相似样本训练时，策略转为聚焦训练样本而非变量：仅选取符合测试分布的训练样本。这样训练的模型虽适配测试分布（但泛化性受限），能在竞赛问题上取得最佳测试效果。该方法的局限性在于会缩减数据集规模——若符合测试分布的样本过少，可能因训练样本不足导致模型严重偏差。前例中仅筛选概率超过0.5的对抗性预测样本，最终仅获得1,495个案例（数量极少说明测试集与训练集差异不大）：

---

打印(np.sum(cv_preds[:len(X), 1] > 0.5))

---

最终，通过模拟测试集进行验证的策略是：持续使用全部数据进行训练，但验证时仅选取训练集中预测概率超过0.5（或更高阈值如0.9）的对抗性预测样本。这种与测试集匹配的验证集设置，能帮助你选择所有可能提升排行榜成绩的超参数和模型方案。

在本例中，通过以下代码输出可发现feature_19和feature_54在训练集/测试集划分中差异最为显著：

---

model.fit(X, y)

ranks = sorted(list(zip(X.columns, model.feature_importances_)),

key=lambda x: x[1], reverse=True)

for feature, score in ranks:

print(f"\{feature:10\} : \{score:0.4f\}")

---

总结对抗性验证时需注意：该方法通常能提升竞赛表现，但并非万能。在Kaggle代码竞赛等无法完全访问测试集的场景中无法应用。此外，该方法虽能揭示测试数据整体特征，却无法区分私有/公开测试集的划分——这正是导致公开排行榜过拟合和后续排名震荡的主因。

尽管对抗性验证是专为竞赛设计的特殊方法，但在实际应用中颇具价值：你是否常因选错测试集导致模型验证失效？该方法能有效判断项目中测试数据与验证数据的使用合理性。更重要的是，生产环境中的数据变化可能导致模型预测失真（概念漂移），通过对抗性验证可快速判断是否需要重新训练部署模型。

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_208.jpg?x=239&y=1563&w=361&h=367&r=0"/>

<!-- Media -->

## Giuliano Janson

https://www.kaggle.com/adjgiulio

Giuliano Janson是Zillow集团的机器学习与自然语言处理高级应用科学家，同时保持Kaggle竞赛大师头衔。他向我们分享了夺冠经验、交叉验证的重要性，以及接下来章节重点探讨的数据泄露问题。

## 您最青睐哪种竞赛类型？原因是什么？在Kaggle平台上，您的技术专长和解题方法论有何独到之处？

我理想的竞赛包含三大要素：a) 具有研究价值的课题；b) 中等规模数据集（既能内存加载又避免过拟合困扰）；c) 特征工程层面的创新空间。当三者兼备时，\( {I}^{\prime }m \)就能在竞技机器学习中全力施展——既保持严谨方法论，又能自由发挥创造力，无需受工程限制束缚。

## 您如何规划Kaggle竞赛策略？这与日常工作方法有何不同？

Kaggle竞赛是场马拉松。投入初期用几天时间就能达到最终得分的90%-95%，剩余阶段需要持续精进。这里唯一的成功标准就是分数，其他因素皆无关紧要。

我的日常工作更像是一连串冲刺。模型性能只是我需考虑的冰山一角。上线日期可能同样重要，而可解释性、扩展性和可维护性等因素，完全可能让天平倾向截然不同的方向。每次冲刺后重新评估优先级，最终成品往往与最初设想大相径庭。况且建模只占我日常的小部分时间，更多精力花在与人沟通、优先级管理、构建用例、清洗数据，以及思考如何将原型模型转化为成功的生产解决方案。

## 请分享您参加过最具挑战性的竞赛，以及您用来解决任务的关键洞察

我赢得的两次竞赛之一——基因泰克癌症预测大赛（Genentech Cancer competition）是仅限硕士参加的赛事。提供的原始交易数据没有现成的结构化数据集，这正是我钟爱的类型，因为特征工程本就是我机器学习工作中最享受的环节。参赛时我已具备十年医疗行业经验，对数据有着商业和临床层面的理解，但最重要的是，我深刻理解正确处理此类数据的工程复杂度，以及处理这类原始交易数据时可能出现的各种问题。这些认知最终成为制胜关键——关于数据泄露源的初始假设之一被证实成立，由此产生的"黄金特征"为模型提供了最终助力。这次竞赛让我明白：进行特征工程或建立验证方法时务必格外谨慎。数据泄露往往难以察觉，常规的训练/验证/测试方法在多数情况下无法识别泄露风险，这会导致模型在生产环境中表现不佳。

## Kaggle对您的职业发展有何帮助？

Kaggle从两方面助益我的发展：首先，它为我提供了接触现代机器学习的低门槛入口，大量接触前沿建模技术的机会，并迫使我真正掌握专业级模型验证技术的艺术与科学；其次，Kaggle让我得以结识应用机器学习领域最杰出的头脑。与顶尖Kaggle选手组队获得的经验，成为我每日与团队分享的宝贵财富。

## 您如何通过Kaggle构建个人作品集？

我的职业生涯并未因Kaggle简历直接获益——我的意思是并未因此获得工作邀约或面试机会。开始参与Kaggle时，我已担任高级数据科学家职位，尽管当时工作不侧重机器学习。得益于在Kaggle所学，我成功推动职业转型，转向以机器学习为核心的岗位。

至今，许多同事仍热衷讨论竞技机器学习，对我的Kaggle经验技巧充满好奇。但不可否认，机器学习领域仍有大量从业者可能从未听说过Kaggle。

## 根据您的经验，新手Kaggle选手常忽视哪些要点？您希望初入行时就知道的认知是什么？

规范的交叉验证重要性常被竞技机器学习新手忽视。稳健的交叉验证框架能可靠客观地衡量改进效果。在长达六个月的竞赛中，最终胜出的模型往往不属于最初点子最妙的人，而属于那些愿意根据数据反馈持续迭代调整的选手。优秀的验证框架正是这一切的基础。

## 您过去在竞赛中犯过哪些错误？

我给机器学习新手的忠告是："切勿过度迷恋复杂方案"。面对复杂新问题时，人们容易倾向于构建复杂解决方案，但这通常耗时良久。关键在于：在已有稳健基线的前提下，复杂方案往往边际效益有限。例如设想建立选举预测模型时，若耗费数周设计复杂特征来捕捉地理、社会经济和时间维度间的潜在关联，可能收效甚微——当简单特征组合已能通过数据驱动深度交互实现高度优化时，精心构建的复杂特征可能几乎不带来提升。我的建议是遵循奥卡姆剃刀原则：在尝试复杂方法前，先验证简单方案。

## 您会推荐哪些特别适合数据分析或机器学习的工具或库？

我是Pandas和Scikit-learn的忠实用户。钟爱Pandas便捷的数据处理与探索能力，也欣赏Scikit-learn让我能在几分钟内快速构建模型原型。我的大部分原型工作都依赖这两个库。不过最终模型通常基于XGBoost实现。至于深度学习，我偏好使用Keras。

## 数据泄露处理

Kaggle竞赛中常见的影响比赛结果的问题是数据泄露。数据泄露（常简称为leakage或冠以"黄金特征"等花哨名称）指训练阶段存在预测时无法获取的信息。这类信息会导致模型在训练和测试阶段表现虚高，虽能提升竞赛排名，但从主办方角度看，基于此构建的解决方案要么完全无效，要么至多只是次优选择。

正如Michael Kim(https://www.kaggle.com/mikeskim)在2019年Kaggle旧金山日活动演讲中所定义：数据泄露是"当涉及真实标签的信息被人为或无意地混入训练特征数据或训练元数据时发生的现象"。

尽管主办方和Kaggle团队会严格核查，数据泄露仍频繁出现在竞赛中。这源于其隐蔽性——Kaggle选手们为提升成绩不遗余力地搜寻任何可能线索时，往往意外触发这种微妙问题。

切勿将数据泄露与存在漏洞的验证策略混淆。后者指因训练数据信息渗入验证集而导致验证分数虚高的情况。这与竞赛本身无关，而是源于验证流程设计缺陷——常见于未划分训练/验证集前就进行数据预处理（如标准化、降维、缺失值填补）。

防范验证漏洞的关键在于：使用Scikit-learn处理数据时，必须确保验证集不参与任何拟合操作。推荐采用Scikit-learn管道(https://scikit-learn.org/stable/modules/generated/sklearn.pipeline.Pipeline.html)，将数据处理与建模封装为统一流程，杜绝数据泄露风险。

数据泄露虽与验证操作无直接关联，却会深刻影响验证效果。本章虽聚焦验证策略，但必须探讨此议题——它直接关系到模型评估效果及在竞赛测试集之外的泛化能力。

泄露通常发生在特征或样本层面，其中特征泄露最为常见。成因包括：存在目标变量的代理特征，或使用了时间上晚于目标本身的特征。代理目标可能源自标签处理过程（如特定编号规则与响应值的隐性关联）。更隐蔽的情况是主办方在划分数据前对训练/测试集进行了联合处理。Kaggle史上著名泄露案例包括：

1. 主办方数据处理不当，特别是对训练/测试集进行联合操作时（如"贷款违约预测"竞赛中，主办方最初使用的聚合历史特征泄露了未来信息）。

2. 与时间索引或特定数据组相关的行序问题（如"Telstra网络中断"竞赛中，某特征的记录顺序暗示了未公开但极具预测力的位置信息）。

3. 与时间索引相关的列序问题（通过行列转换可获取线索）。

4. 连续行间的特征重复（如"博世生产线效能"竞赛中，这暗示了响应相关性，详见Beluga的冠军方案https://www.kaggle.com/c/bosch-production-line-performance/discussion/25434）。

5. 图像元数据泄露（参见"Two Sigma租房询价预测"竞赛案例）。

6. 哈希编码或简单匿名化处理的标识符存在可破解风险。

后验信息的问题源于我们在处理信息时未考虑时间因素及跨时间维度的因果序列效应。由于我们回望过去时，常会忽略当下有意义的变量在过去并不具备价值。例如，在评估新公司贷款信用评分时，得知借款经常逾期是判断债务人可靠性低、风险高的关键指标——但这只能在放贷后获知。这也是分析企业数据库时的常见问题：查询数据反映的是现状而非历史。若无法明确限定只提取特定时间点的信息，重构历史数据将极为困难。因此建模前必须投入大量精力识别这些泄露特征并予以剔除或调整。

同类问题在基于银行保险等数据的Kaggle竞赛中也很常见，但由于赛事数据经过严格处理，泄露特征会以更隐蔽的形式出现。通常这些特征会与目标变量高度相关，领域专家能识别其成因（比如数据录入数据库的阶段）。因此竞赛中不会出现明显的泄露特征，而是经过转换处理、脱离主办方控制的衍生特征。由于特征常被匿名化以保护商业机密，它们往往隐匿在其他特征中。这催生了寻找"黄金/魔法特征"的热潮——通过组合现有特征使数据泄露显性化。Corey Levison在领英的精彩文章（链接略）讲述了桑坦德客户交易预测竞赛如何演变为他们团队的魔法特征搜寻之旅。

dune_dweller提供的另一个典型案例（链接略）中，通过观察数据排序方式，他发现数据可能按时间顺序排列。将此信息转化为新特征后显著提升了评分。

另一种泄露形式是训练样本泄露，常见于非独立同分布数据。这意味着某些案例因处于相同时段（或相邻时段）、同一组别而产生关联。若这些案例未全部集中在训练集或测试集，而是分散在两者中，机器学习算法很可能学会识别特定案例（而非运用通用规则）进行预测。吴恩达教授团队的案例常被引用（链接略）：2017年他们使用3万名患者的10万张X光片撰写论文时，采用随机划分训练测试集，未意识到同一患者的X光片可能同时存在于两个集合中。Nick Roberts等从业者指出这种泄露可能虚增模型表现，最终导致论文重大修订。

Kaggle竞赛出现数据泄露时会如何处理？平台有明确政策：

- 维持竞赛现状（尤其当泄露影响较小时）

- 剔除泄露数据后重新竞赛

- 生成不含泄露的新测试集

特别值得注意的是，Kaggle建议公开任何被发现的数据泄露（leakage），尽管不强制要求或惩罚未公开行为。但根据我们的经验，比赛中一旦存在数据泄露，很快就会变得显而易见——论坛讨论区将迅速涌现关于"魔法特征"（magic features）等话题的热议。只要密切关注论坛动态并整合各位Kagglers提供的线索，你很快就能察觉异常。但需警惕，某些选手可能故意炒作"魔法特征"话题来误导竞争对手偏离有效建模。例如在桑坦德客户交易预测赛中，就发生过知名案例：部分参赛者通过鼓吹华而不实的"魔法特征"，诱使他人研究方向出现偏差（详见讨论链：https://www.kaggle.com/c/santander-customer-transaction-prediction/discussion/87057#502362）。

我们建议仔细研读比赛论坛中关于数据泄露和魔法特征的讨论，根据个人参赛兴趣和目标，自主决定是否利用已发现的泄露信息。

刻意回避数据泄露可能严重影响最终排名，但确实会损害学习价值（因为泄露属于数据失真，基于此构建的模型不具备参考意义）。若参赛目的并非建立声誉或争取赞助商雇佣机会，利用泄露信息无可厚非；否则请坚持踏实建模（说不定Kaggle最终会重置或修复比赛，让那些依赖泄露信息者空欢喜一场）。

数据泄露形态因赛事而异。若想了解Kaggle历史上的典型泄露案例，可参考以下三个经典案例：

- 红帽商业价值预测赛（https://www.kaggle.com/c/predicting-red-hat-business-value）中，由于训练集/测试集划分方法缺陷引发的泄露（讨论链：https://www.kaggle.com/c/predicting-red-hat-business-value/discussion/22807）

- TalkingData移动用户画像赛（https://www.kaggle.com/c/talkingdata-mobile-user-demographics）中，非独立同分布数据导致划分失效的案例（讨论链：https://www.kaggle.com/c/talkingdata-mobile-user-demographics/discussion/23403）

- Two Sigma租房询价预测赛（https://www.kaggle.com/c/two-sigma-connect-rental-listing-inquiries）中，元数据（文件夹创建时间）引发的泄露（讨论链：https://www.kaggle.com/c/two-sigma-connect-rental-listing-inquiries/discussion/31870）

## 本章总结

在本章结尾，我们将梳理全程讨论的关键建议，助你构建有效的验证策略，并筛选出最终提交的优质模型。

本章首先解析了公开排行榜的动态特性，探讨了适应性过拟合（adaptive overfitting）和排名震荡（shake-ups）等问题。继而论述了数据科学竞赛中验证体系的重要性，包括构建可靠验证系统、对标排行榜优化以及过程追踪。

在探讨多种验证策略后，我们介绍了超参数调优的最佳实践，以及通过对抗性验证（adversarial validation）检测测试数据/验证集划分的方法。最后分析了Kaggle赛事中的典型数据泄露案例及应对策略。

最终建议如下：

- 赛事初期优先构建可靠验证方案，采用\( k \)折交叉验证而非简单训练集-测试集划分，因其概率特性更能泛化至未知数据。

- 若验证方案不稳定，可增加折数或多次运行不同数据划分。务必使用对抗性验证检测测试集。

- 同步追踪验证方案与排行榜结果。在探索潜在优化（如魔法特征或泄露）时，优先采信验证分数。

- 如开篇所述，最终提交选择应基于验证分数。根据对排行榜可信度的判断，在最优交叉验证模型与排行榜高分提交间抉择时，建议优先选择前者。

在旅程的这一阶段，我们将探讨如何利用表格数据（即按矩阵排列的数值型或类别型数据，其中行代表样本，列代表特征）应对竞赛。下一章将介绍Kaggle组织的月度比赛"表格游乐场系列"（由Inversion策划：https://www.kaggle.com/inversion）。此外，我们将分享提升竞赛表现的关键技术，包括特征工程、目标编码、降噪自编码器，以及针对表格数据的神经网络方案——这些都可作为当前公认最优算法（如XGBoost、LightGBM或CatBoost等梯度提升算法）的替代选择。

## 加入本书的Discord空间

加入本书的Discord工作区，每月参与作者问答会：

https://packt.link/KaggleDiscord

## 表格竞赛建模

2017年之前，竞赛类型无需过多区分，由于绝大多数比赛基于表格数据，甚至在Kaggle论坛都难觅"表格竞赛"的提法。但形势骤变。经历赛事空窗期（参见https://www.kaggle.com/general/49904）后，深度学习竞赛占据主导，表格竞赛日渐式微，令许多人失望。其稀缺程度迫使Kaggle近期不得不推出基于合成数据的表格竞赛系列。何以至此？

2017-2018年间，数据科学已发展成熟，众多企业开启数据化进程。这门学科虽仍是热点，却不再新奇。当年Kaggle上反复出现的各类问题解决方案，已成为许多企业的标准实践。在此背景下，主办方缺乏举办外部表格竞赛的动力——因为他们内部已在处理相同问题。反观深度学习领域仍存在大量未知，长期内都将如此，因此举办竞赛挑战技术前沿、探索创新方案显得更有意义。

本章将探讨表格竞赛，回顾经典赛事并聚焦近期的"表格游乐场系列"。鉴于表格问题仍是全球数据科学家的主流实践，Kaggle平台蕴含丰富学习资源。我们将从探索性数据分析（EDA）和特征工程这两项常规工作切入，在阐述特征工程核心策略后，延伸至类别编码、特征选择、目标变换及伪标签等技术。最后探讨针对表格数据的深度学习方法，介绍TabNet等专用神经网络架构，并解析降噪自编码器——这种在近期Kaggle竞赛中大放异彩却尚未广泛应用于现实场景的技术。

本章涵盖：

- 表格游乐场系列

- 设置随机种子保证可复现性

- EDA的重要性

- 数据降维

- 实施特征工程

- 伪标签技术

- 自编码器降噪

- 表格竞赛专用神经网络

本章不会涵盖表格竞赛的所有相关主题，但这些内容作为数据科学的核心，你可以在许多其他书籍中轻松找到。本章的重点是介绍一系列特殊技术和策略，这些是Kaggle表格竞赛的独特之处，除了Kaggle论坛外，其他地方很难见到。

## 表格游乐场系列

鉴于对表格问题的巨大需求，Kaggle团队在2021年启动了一项实验，推出了名为"表格游乐场系列"的月度比赛。这些比赛基于合成数据集，这些数据复制了公开数据或以往竞赛的数据。合成数据的生成得益于名为CTGAN的深度学习生成网络。

你可以在https://github.com/sdv-dev/CTGAN找到CTGAN代码。还有一篇相关论文解释了其工作原理：通过建模表格数据行的概率分布来生成逼真的合成数据（参见https://arxiv.org/pdf/1907.00503v2.pdf）。

由麻省理工学院发起的"合成数据保险库"(https://sdv.dev/)开发了CTGAN背后的技术及一系列配套工具。其成果是一套开源软件系统，旨在帮助企业生成模拟真实数据的合成数据；它可以帮助数据科学家基于真实数据创建匿名数据集，并为建模目的扩展现有数据集。

Kaggle在2021年成功举办了13场竞赛，尽管没有积分、奖牌或奖金（仅有一些周边商品），仍吸引了许多Kaggle用户。以下是2021年的竞赛列表，你可以按类型或指标查找特定问题，并寻找相关资源如专题讨论或Notebook：

<!-- Media -->

<table><tbody><tr><td>月份</td><td>\( \mathbf{{Problem}} \)</td><td>变量</td><td>\( \mathbf{{Metric}} \)</td><td>缺失数据</td></tr><tr><td>2021年1月</td><td>未指定问题的回归分析</td><td>数值型</td><td>均方根误差(RMSE)</td><td>否</td></tr><tr><td>2021年2月</td><td>预测保险索赔金额的回归分析</td><td>数值型和分类型</td><td>均方根误差(RMSE)</td><td>否</td></tr><tr><td>2021年3月</td><td>预测保险索赔的二元分类</td><td>数值型和分类型</td><td>曲线下面积(AUC)</td><td>否</td></tr><tr><td>2021年4月</td><td>基于泰坦尼克号原始数据集高度复刻的二元分类</td><td>数值型和分类型</td><td>准确率</td><td>是</td></tr></tbody></table>

<table><tbody><tr><td>2021年5月</td><td>多类别分类：根据商品列表的多种属性预测电商产品类别</td><td>分类变量</td><td>多类别对数损失(Multiclass LogLoss)</td><td>否</td></tr><tr><td>2021年6月</td><td>多类别分类：根据商品列表的多种属性预测电商产品类别</td><td>数值型与分类型</td><td>多类别对数损失(Multiclass LogLoss)</td><td>否</td></tr><tr><td>2021年7月</td><td>多元回归：通过各类输入传感器数值（如时间序列）预测城市空气污染</td><td>数值型，时间型</td><td>均方根对数误差(RMSLE)</td><td>是</td></tr><tr><td>2021年8月</td><td>回归计算：评估贷款违约相关损失</td><td>数值型</td><td>均方根误差(RMSE)</td><td>否</td></tr><tr><td>30天机器学习挑战</td><td>保险理赔金额回归分析</td><td>数值型与分类型</td><td>均方根误差(RMSE)</td><td>否</td></tr></tbody></table>

<table><tbody><tr><td>2021年9月</td><td>二元分类预测保险单是否会产生索赔</td><td>数值型</td><td>AUC（曲线下面积）</td><td>是</td></tr><tr><td>2021年10月</td><td>二元分类预测给定多种化学特性后分子的生物反应</td><td>数值型与分类型</td><td>AUC（曲线下面积）</td><td>否</td></tr><tr><td>2021年11月</td><td>二元分类通过从电子邮件中提取的各种特征识别垃圾邮件</td><td>数值型</td><td>AUC（曲线下面积）</td><td>否</td></tr><tr><td>2021年12月</td><td>基于原始森林覆盖类型预测竞赛的多类别分类</td><td>数值型与分类型</td><td>多类别分类准确率</td><td>否</td></tr></tbody></table>

表7.1：2021年表格游乐场系列竞赛

2022年表格游乐场竞赛持续举办，推出了更加复杂且具有挑战性的赛题：

<table><tbody><tr><td>2022年1月</td><td>预测两家虚构独立连锁店的Kaggle周边商品销售额</td><td>日期与分类数据</td><td>对称平均绝对百分比误差(SMAPE)</td><td>否</td></tr><tr><td>2022年2月</td><td>利用包含数据压缩和丢失的基因组分析技术数据，对10种不同细菌种类进行分类</td><td>数值型</td><td>分类准确率</td><td>否</td></tr></tbody></table>

表7.2：2022年表格数据竞赛系列赛事

<!-- Media -->

本章大部分内容是通过观察这些竞赛中产生的代码与讨论撰写而成，而非分析过去更辉煌的赛事。正如我们所述，鉴于专业环境的变化，表格竞赛确实已永久消失，因此阅读与当下相关的建议提示会比研究历史资料更具实用价值。

与其他完整的Kaggle积分奖牌赛事相同，在表格竞赛中我们建议遵循本书其他章节讨论过的高效基础流程：

- 探索性数据分析（EDA）

- 数据预处理

- 建模（采用交叉验证策略进行模型验证）

- 后处理

- 结果提交

原则上还需注意保持实验可复现性，保存所有模型（包括每折验证模型）、参数列表、各折验证预测结果、袋外预测数据以及全量数据训练模型的全部预测结果。

存储这些信息时应确保易于检索重建，例如采用规范标签系统、记录MD5哈希值（具体方法可参考Stack Overflow解答：https://stackoverflow.com/questions/16874598/how-do-i-calculate-the-md5-checksum-of-a-file-in-python），并追踪每次实验的交叉验证分数和排行榜成绩。多数Kaggle选手使用.txt文件或Excel表格等简单工具管理，但也可采用更专业的方案如：

- DVC（https://dvc.org/）

- Weights and Biases（https://wandb.ai/site）

- MLflow（https://mlflow.org/）

- Neptune（https://neptune.ai/experiment-tracking）

最终关键的是结果而非工具，即便在竞赛白热化阶段也应尽力保持实验与模型的有序性。

在继续之前，建议思考Kaggle生成竞赛数据的技术原理；若能准确理解数据生成机制，将获得显著优势。此外，掌握合成数据的工作原理能切实影响现实中的数据科学实践——这为你提供了轻松获取多样化训练数据的途径。

例如，以谷歌大脑(Google Brain)举办的呼吸机压力预测竞赛(https://www.kaggle.com/c/ventilator-pressure-prediction)为例。该竞赛要求开发用于机械通气控制的机器学习模型。虽然通过深度学习对提供的数据建模可获得不错结果，但鉴于数据是合成生成的，参赛者亦可逆向工程其生成过程来获得排行榜顶尖成绩——正如Jun Koda(https://www.kaggle.com/junkoda)在其帖子(https://www.kaggle.com/c/ventilator-pressure-prediction/discussion/285278)中所述及实践的那样。如今生成人工数据并理解合成数据变得前所未有的简单，这一点你可通过本笔记(https://www.kaggle.com/lucamassaron/how-to-use-ctgan-to-generate-more-data)验证，该笔记源自Dariush Bahrami(https://www.kaggle.com/dariushbahrami)最初编写测试的代码。

## 设置随机状态以确保可复现性

在开始探讨表格类竞赛可能用到的步骤和模型前，有必要重申前文提及的可复现性主题。

在Kaggle笔记代码中，多数命令都包含一个声明数字种子(seed)作为随机状态的参数。该设置对结果可复现性至关重要。由于许多算法并非确定性而是基于随机性，设置种子可影响随机数生成器行为，使其随机性可预测：相同随机种子对应相同随机数序列。换言之，这能确保每次运行相同代码都获得一致结果。

正因如此，Scikit-learn所有机器学习算法及兼容模型（如最流行的XGBoost、LightGBM和CatBoost）都设有随机种子参数。

结果可复现性在实际项目和Kaggle竞赛中同等重要。现实中，可复现模型有助于更好追踪开发过程并保持一致性。在Kaggle竞赛中，可复现性能更有效验证假设，因为你控制了模型中所有变异来源。例如，若创建新特征，将其纳入可复现流程可明确判断该特征是否有效——你能确信模型表现的任何提升或退化仅源于该特征，而非上次运行后某些随机过程的变化所致。

处理公开笔记时，可复现性亦可成为优势。这些笔记通常使用固定种子（0、1或42）。42这个值尤为常见，源自道格拉斯·亚当斯《银河系漫游指南》中超级计算机"深思"花费750万年计算得出的"生命、宇宙及万物的终极答案"。当竞赛中所有人都使用相同随机种子时，会产生双重效应：

- 该随机种子可能在公开排行榜表现过优，意味着过拟合

- 大量参赛者将产生相似结果，导致他们在最终排行榜的名次变化趋同

改变随机种子既能避免过拟合，又可打破排名趋同——即获得与他人不同的结果，这可能最终使你占据优势。此外，若赢得Kaggle竞赛，需证明获胜模型如何生成提交结果，因此要快速获奖就必须确保所有环节完全可复现。

TensorFlow和PyTorch模型未显式使用随机种子参数，因此确保其完全可复现更具挑战性。以下代码片段可为两者设置相同随机种子：

<!-- Media -->

---

def seed_everything(seed,

tensorflow_init=True,

pytorch_init=True):

	...

为结果可复现性设置基础参数

	"""

random.seed(seed)

os.environ["PYTHONHASHSEED"] = str(seed)

np.random.seed(seed)

if tensorflow_init is True:

tf.random.set_seed(seed)

if pytorch_init is True:

torch.manual_seed(seed)

torch.cuda.manual_seed(seed)

torch.backends.cudnn.deterministic \( = \) True

torch.backends.cudnn.benchmark = False

---

<!-- Media -->

对于Scikit-learn，更建议在类或函数允许的情况下，直接通过random_state参数设置随机种子。

## 探索性数据分析（EDA）的重要性

EDA这一术语源自现代统计学方法的重要倡导者约翰·W·图基的研究。在其1977年著作《探索性数据分析》（Exploratory Data Analysis，缩写即EDA）中，图基将EDA视为通过数据探索发现证据、形成假设的过程，这些假设后续可通过统计检验验证。他认为统计假设的建立应更多基于观察与推理，而非仅依赖数学计算的序列检验。这一理念与机器学习领域高度契合——正如我们将在下节讨论的，通过数据优化与预处理，能使学习算法更高效地工作。

在Kaggle竞赛的EDA过程中，你需要重点关注：

- 缺失值，尤其是与预测目标相关的缺失值模式

- 数值型变量的偏态分布及其可能的转换方法

- 分类变量中可合并的稀有类别

- 单变量及多变量潜在异常值。

- 高度相关（甚至重复）的特征。对于分类变量，重点关注重叠的类别。

- 针对该问题最具预测性的特征。

您可以通过多种描述性分析、图表和图形实现这一目标：首先检查每个独立特征（统计学中的单变量分析），然后匹配几个变量（双变量分析，如散点图），最后同时考虑更多特征（多变量方法）。

如果您感到无从下手，初期依赖自动化策略会很有帮助。例如，快速EDA免费工具AutoViz（https://github.com/AutoViML/AutoViz）能大幅节省时间。在Notebook中运行以下命令安装：

pip install git+git://github.com/AutoViML/AutoViz.git

阅读Dan Roth在Medium的文章（https://towardsdatascience.com/autoviz-a-new-tool-for-automated-visualization-ec9c1744a6ad）或浏览Georgii Vyshnia的公开Notebook（https://www.kaggle.com/gvyshnya/automating-eda-and-feature-importance-detection），可更清晰了解AutoViz功能。

后一个链接中还提及Sweetviz工具（https://github.com/fbdesignpro/sweetviz），其基于泰坦尼克数据集的概述文章见：https://towardsdatascience.com/powerful-eda-exploratory-data-analysis-in-just-two-lines-of-code-using-sweetviz-6c943d32f34。

另一个常用工具是Pandas Profiling（https://github.com/pandas-profiling/pandas-profiling），它更依赖经典统计描述与可视化，详见：https://medium.com/analytics-vidhya/pandas-profiling-5ecd0b977ecd。

关注Kaggle用户发布的EDA Notebook也是解决方案——这些资料可能包含宝贵提示，能助您启动建模阶段并理解竞赛基本准则。但请注意，当EDA高度针对具体问题时，它将从通用工具转变为竞赛优势，这种洞察力无法从自动化方案或公开Notebook中获得，必须亲自探索。

综上，我们建议尝试自动化工具——它们简单易用，能节省大量时间用于分析图表和推导洞见，从而提升竞赛表现。但之后仍需掌握Matplotlib和Seaborn，根据数据类型和问题创建非标准图表。

例如对于时间序列数据，绘制基于时间的连续函数与离散观测点同样重要，展示观测间的时间滞后可能揭示预测改进方向。

## 使用t-SNE和UMAP进行降维

EDA中有多种可视化方法，我们重点介绍两种能提供定制化图表信息的降维技术：t-SNE（https://lvdmaaten.github.io/tsne/）和UMAP（https://github.com/lmcinnes/umap）。

数据科学家常用t-SNE和UMAP将多维数据投影到低维空间，通常用二维呈现复杂数据集。二维UMAP/t-SNE图能揭示异常值存在和关键数据簇，若按目标值着色散点图，还可获得处理子群的策略线索。

虽然这与图像竞赛相关，但Chris Deotte在SIIM-ISIC黑色素瘤分类竞赛中的分析（参见https://www.kaggle.com/c/siim-isic-melanoma-classification/discussion/168028）很好地展示了UMAP和t-SNE如何帮助您更好地理解数据。在这个例子中，Chris将训练数据和测试数据关联到相同的低维投影上，突出显示了仅存在测试样本的区域。

尽管UMAP和t-SNE在发现难以察觉的数据模式方面提供了宝贵帮助，但您仍可将它们用作建模的特征。Mike Kim在Otto集团产品分类挑战中展示了这种用法的一个有趣例子，他使用t-SNE投影作为竞赛的训练特征（https://www.kaggle.com/c/otto-group-product-classification-challenge/discussion/14295）。

正如《如何有效使用t-SNE》（https://distill.pub/2016/misread-tsne/）一文所述，必须正确使用这些技术，因为很容易在不存在聚类和模式的地方发现它们。同样的警告也适用于UMAP，因为它也可能生成容易被误读的图表。像https://pair-code.github.io/understanding-umap/这样的指南提供了关于UMAP和t-SNE在真实数据上表现的可靠建议，并给出了注意事项。

尽管存在这些风险，但根据我们的经验，这些方法无疑比基于线性组合（如PCA或SVD）的方差重构传统方法更具揭示性。与这些方法相比，UMAP和t-SNE能够极大降低维度，在保持数据拓扑结构的同时实现结果的可视化图表化。副作用是它们的拟合速度较慢。然而，NVIDIA发布了基于CUDA的RAPIDS套件（https://developer.nvidia.com/rapids），使用GPU驱动的Notebook或脚本，可以在非常合理的时间内返回UMAP和t-SNE的结果，使其能够有效用作EDA工具。

您可以在以下链接找到一个有用的例子，展示了如何将UMAP和t-SNE与RAPIDS实现和GPU结合用于数据探索，适用于\( {30}\mathrm{{Days}} \)的\( {ML} \)竞赛：https://www.kaggle.com/lucamassaron/interesting-eda-tsne-umap/。在下图中（即上述示例Notebook的输出），您可以看到数据集中的多个聚类，但没有任何一个可以被认为揭示了与目标的特定关系：

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_231.jpg?x=687&y=400&w=505&h=490&r=0"/>

图7.1：t-SNE图中出现的多个聚类

<!-- Media -->

在另一个Notebook中（https://www.kaggle.com/lucamassaron/really-not-missing-at-random），同样的技术被应用于缺失样本的二进制指标，揭示了暗示由特定类型响应主导的独特区域的引人深思的图形。实际上，在那个例子中，缺失样本并非随机出现，它们具有很强的预测性：

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_231.jpg?x=685&y=1281&w=512&h=498&r=0"/>

图7.2：这个t-SNE图轻松揭示了阳性目标占主导地位的区域

<!-- Media -->

## 减小数据规模

如果您直接在Kaggle Notebooks上工作，会发现其限制相当烦人且耗时。其中一个限制是内存不足错误，这会停止执行并迫使您从头重新启动脚本。这在许多竞赛中相当常见。然而，与基于文本或图像的深度学习竞赛不同（在那些竞赛中，您可以从小批量磁盘中检索数据并进行处理），大多数处理表格数据的算法需要将所有数据加载到内存中。

最常见的情况是，您使用Pandas的read_csv从CSV文件上传数据，但DataFrame太大，无法在Kaggle Notebook中进行特征工程和机器学习处理。解决方案是在不丢失任何信息（无损压缩）的情况下压缩您正在使用的Pandas DataFrame的大小。这可以轻松实现，使用以下源自Guillaume Martin工作的脚本（原始Notebook在此：https://www.kaggle.com/gemartin/load-data-reduce-memory-usage）。

---

def reduce_mem_usage(df, verbose=True):

numerics = ['int16', 'int32', 'int64',

'float16', 'float32', 'float64']'

start_mem = df.memory_usage(   ).sum(   ) / 1024**2

for col in df.columns:

col_type = df[col].dtypes

if col_type in numerics:

c_min = df[col].min(   )

c_max = df[col].max(   )

if str(col_type)[:3] == 'int':

if c_min > np.iinfo(np.int8).min and c_max < np.iinfo(np.

int8).max:

df[col] = df[col].astype(np.int8)

elif c_min > np.iinfo(np.int16).min and c_max < np.iinfo(np.

int16).max:

df[col] = df[col].astype(np.int16)

elif c_min > np.iinfo(np.int32).min and c_max < np.iinfo(np.

int32).max:

df[col] = df[col].astype(np.int32)

elif c_min > np.iinfo(np.int64).min and c_max < np.iinfo(np.

int64).max:

\[\text{df[col] = df[col].astype(np.int64)}\]

否则：

若c_min大于np.finfo(np.float32).min且c_max小于np.finfo(np.

float32).max：

将df[col]类型转换为np.float32

否则：

将df[col]类型转换为np.float64

内存占用 = df.memory_usage(   ).sum(   ) / 1024**2

若启用详细模式：打印('内存占用降至\{:5.2f\} Mb（降幅\{:.1f\}%

）'.format(内存占用, 100 * (初始内存 - 内存占用) / 初始内存))

返回df

---

Guillaume Martin并非首个在Kaggle提出此类想法的用户。最早提出压缩Pandas DataFrame构想的Kaggle用户是Arjan Groen，他在Zillow竞赛期间编写了内存优化函数(https://www.kaggle.com/arjanso/reducing-dataframe-memory-size-by-65)。

该脚本利用了数据集中所有数值特征均处于特定取值范围的特性。鉴于Python中存在不同字节占用的整型和浮点型变量，脚本会比对每个特征值的范围与各数值类型的极值，从而将特征设置为既满足取值范围又占用最小内存的数值类型。

该方法在Kaggle Notebooks上运行流畅，但需注意：通过压缩为最佳数值类型后，任何可能导致超出该类型容量的特征工程操作都会产生错误结果。建议在特征工程完成后或进行不改变数据尺度的主要转换前应用此方法。配合垃圾回收库gc及其gc.collect(   )方法可进一步改善Notebook内存状况。

另一种缩减数据规模的方法（除其他外）是运用特征工程（特别是特征选择与数据压缩）。

## 应用特征工程

在实际项目中，区分优秀机器学习模型与平庸模型的关键往往是数据而非算法。优质数据的评判标准不仅在于缺失值数量、数值可靠性（"质量"）或样本量（"数量"），根据我们的经验，真正的差异在于内容本身的信息价值——这正体现在特征类型上。

特征才是数据科学项目中真正可塑的原材料，它们包含着模型用于分类或预测的信息。虽然每个模型都具备将特征转化为预测的表达能力，但若特征本身匮乏，任何模型都无法凭空生成更优预测。模型仅能显化数据中的价值，其本身并不具备魔力。

在Kaggle平台上，除极少数允许补充外部数据的竞赛外，所有参赛者最初获得的数据集都是相同的。此时，数据处理方式成为制胜关键。许多参赛者常犯的错误是忽视了数据优化的可能性。特征工程——这套将原始数据转化为模型更易理解信息的技术体系，始终是提升竞赛表现的核心。即便应用更强大的模型，仍需通过数据处理使其呈现更易解析的形态。

特征工程也是将先验知识（通常是问题领域的专业见解）注入数据的途径：通过对现有特征进行加总、差值或比率运算，可获得能更好解释目标问题的指标或估计量。特征工程还有其他价值：在Kaggle竞赛中虽不显著，但对实际项目至关重要。其一是缩减训练数据规模（在使用内存受限的Notebook参赛时也有助益）；其二是通过人类可理解的特性，提升模型结果的可解释性。

各领域都存在特定的变量转换方法，这些方法未必不言自明，却是该领域专家的常识。以金融为例，需通过卡尔曼滤波或小波变换等技术，从代表市场和公司数据的特征集中分离信号与噪声。鉴于领域多样性和特征工程流程的复杂性，本节不深入具体专业领域，而是介绍适用于任何表格类竞赛的通用技术。

## 易生成特征

通过转换生成特征是最简单却常最有效的方法。例如计算特征比率（两特征相除）就非常实用，因为许多算法（如梯度提升）无法模拟除法运算，或（如深度神经网络）难以有效学习除法关系。以下是值得尝试的常见转换：

- 时间特征处理：将日期拆解为年/月/日元素；转换为年度周序和星期几；计算日期差值；计算与关键事件（如节假日）的时间间隔

对于日期数据，另一种常见转换是从日期时间中提取时序元素。基于正弦余弦变换的循环连续转换，能有效表征时间连续性并创建周期特征：

---

cycle = 7

df['星期正弦'] = np.sin(2 * np.pi * df['col1'].dt.dayofweek /

cycle)

df['星期余弦'] = np.cos(2 * np.pi * df['col1'].dt.dayofweek /

cycle)

---

- 数值特征转换：标准化；归一化；对数/指数变换；分离整数与小数部分；数值特征间的加减乘除运算。若使用对特征尺度敏感的算法（如各类神经网络），采用统计学Z-score法标准化或最大最小归一化具有实际意义

- 数值特征分箱：通过将连续变量值分配到若干区间使其离散化。分箱技术能消除数据噪声和误差，当与独热编码结合时（参见Scikit-learn实现：https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.KBinsDiscretizer.html），可轻松建模分箱特征与目标变量的非线性关系

- 类别特征编码：独热编码；合并两三个类别特征的组合编码；或更复杂的目标编码（后续章节详述）

- 基于层级拆分聚合类别特征：例如在泰坦尼克竞赛（https://www.kaggle.com/c/titanic）中，可通过拆分姓名、姓氏及首字母创建新特征

多项式特征通过将特征提升至指数级生成。例如参见Scikit-learn的这一函数：https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.PolynomialFeatures.html。

虽然缺失值处理和离群值处理不属于严格的特征工程范畴而更偏向数据清洗技术，但这些操作会改变数据形态从而间接转换特征，有助于凸显数据中的信号：

- 缺失值处理：创建二元特征标记缺失值，因为缺失往往并非随机现象，其背后可能隐含重要信息。通常缺失情况能反映数据记录方式，相当于其他变量的代理指标。就像人口普查中：如果受访者拒绝透露收入，往往意味着极端贫困或极端富裕。若机器学习算法要求，可用均值、中位数或众数填补缺失值（极少需要更复杂的方法）。

可参考Parul Pandey(https://www.kaggle.com/parulpandey)撰写的完整指南：https://www.kaggle.com/ parulpandey/a-guide-to-handling-missing-values-in-python。

需注意某些模型能自主处理缺失值，其效果优于常规方法，因为缺失值处理已被纳入其优化流程。具备该能力的模型均为梯度提升树：

- XGBoost：https://xgboost.readthedocs.io/en/latest/faq.html

- LightGBM：https://lightgbm.readthedocs.io/en/latest/Advanced-Topics.html

- CatBoost：https://catboost.ai/docs/concepts/algorithm-missing-values-processing.html

- 离群值封顶或剔除：对数据中的异常值进行排除、上下限截断或修正。可使用Scikit-learn中的多元检测模型(https://scikit-learn.org/stable/modules/ outlier_detection.html)。

也可通过单变量方式定位异常样本，根据其与均值的标准差倍数或四分位距(IQR)边界距离进行判断。例如直接剔除大于\( {1.5} * \)IQR + Q3（上界离群点）或小于Q1 - 1.5*IQR（下界离群点）的数据点。发现离群值后，也可用二元变量进行标记。

这些数据转换都能提升模型预测性能，但在竞赛中很少起决定性作用。基础特征工程虽必要，却远远不够。后续章节我们将介绍更复杂的数据价值挖掘方法。

## 基于行列的元特征

要想具备竞争力，需要更精巧的特征工程。可从逐行计算的特征入手：

- 计算数值型数据（或其子集）的均值、中位数、总和、标准差、最小值或最大值

- 统计缺失值数量

- 计算行内常见值的出现频率（例如对二元特征统计正值出现次数）

- 将每行数据分配到通过聚类分析（如\( k \)-均值）得出的簇中

这些元特征（之所以称为"元"，是因为它们代表了一组单一特征的集合特征）通过向算法指明特定的样本分组，有助于区分数据中存在的各类样本。

元特征也可以基于列构建。对单一特征进行聚合和汇总操作的目的，则是提供关于数值型和类别型特征值的更多信息：该特征是普遍还是罕见？这是模型无法捕捉的信息，因为它无法统计特征中的类别实例。作为元特征，您可以使用任何类型的列统计量（如众数、均值、中位数、总和、标准差、最小值、最大值，以及数值特征的偏度和峰度）。对于基于列的元特征，您可以通过以下几种方式实现：

- 频率编码：简单地统计类别型特征中值的出现频率，然后创建一个新特征，用频率值替换原始值。当数值特征中存在频繁重复的值时，也可以应用频率编码。

- 针对相关组计算的频率和列统计量：这种情况下，您可以从数值型和类别型特征的值中创建新特征，因为您考虑的是数据中的不同分组。分组可以是通过聚类分析计算的簇，也可以是利用某个特征定义的组（例如，年龄可生成年龄组，地区可划分区域等）。描述每个组的元特征会根据样本所属组别应用于每个样本。例如，使用Pandas的groupby函数创建元特征后，基于分组变量将其与原始数据合并。该特征工程技术最复杂的部分，是在数据中找到有意义的计算分组。 - 通过组合更多分组，还能衍生出进一步的列频率和统计量。

这个列表虽非详尽无遗，但能让您了解如何利用频率和统计量，在特征级别和行级别寻找新特征。

让我们看一个基于亚马逊员工访问挑战数据的简单示例。首先对ROLE_TITLE特征进行频率编码：

---

import pandas as pd

train = pd.read_csv("../input/amazon-employee-access-challenge/train.csv")

#特征频次统计

feature_counts = train.groupby('ROLE_TITLE').size(   )

print(train['ROLE_TITLE'].apply(lambda x: feature_counts[x]))

---

结果显示特征类别已被其观测频率替代。

现在我们根据ROLE_DEPTNAME的分组来编码ROLE_TITLE特征，因为预计某些职称在特定部门更常见，在其他部门较罕见。

结果是一个由两者组合的新特征，我们用它来统计值的出现频率：

---

feature_counts = train.groupby(['ROLE_DEPTNAME', 'ROLE_TITLE']).size(   )

打印(train[['ROLE_DEPTNAME', 'ROLE_TITLE']].apply(lambda x: feature_

counts[x[0]][x[1]], axis=1))

---

您可在此Kaggle笔记本查看完整代码及运行结果：https://www.kaggle.com/lucamassaron/meta-features-and-target-encoding/

## 目标编码

得益于Scikit-learn提供的简单函数（如：

- 标签编码器(LabelEncoder)

- 独热编码器(OneHotEncoder)

- 序数编码器(OrdinalEncoder)

这些函数能将分类特征转换为数值特征，进而转化为机器学习算法易于处理的二元特征。但当分类数量过多时，独热编码会产生稀疏数据集（大部分值为零），对计算机内存和处理器造成负担。这种情况我们称之为高基数特征，需要特殊处理。

自早期Kaggle竞赛起，高基数变量便采用Micci-Barreca提出的编码函数处理，详见其论文《分类与预测问题中高基数类别属性的预处理方案》（ACM SIGKDD Explorations Newsletter 3.1, 2001: 27-32）。

该方法核心是将分类特征的多个类别转换为对应目标期望值：回归问题中为类别均值，二分类中为条件概率，多分类中为各结果的类条件概率。例如在泰坦尼克号入门竞赛（https://www.kaggle.com/competitions/titanic）中，对性别特征进行目标编码即是用该性别乘客的平均生存概率替代原始值。

如此既实现了分类特征数值化，又避免了数据稀疏化。本质上，目标编码类似基于高基数特征的堆叠预测，虽效果显著但存在过拟合风险——当某些类别样本过少时，目标编码近乎直接泄露标签信息。不过已有相应防范措施。

在介绍可直接导入的现成实现前，让我们看一个目标编码的实际代码示例。这段代码曾用于PetFinder.my领养预测竞赛的高分方案：

---

导入 numpy 库

导入 pandas 库

从sklearn.base导入BaseEstimator和TransformerMixin

类目标编码器（TargetEncode）继承自基础估计器（BaseEstimator）和转换混合类（TransformerMixin）：

def _init_(self, 类别='auto', k=1, f=1,

噪声级别=0, 随机状态=None):

if type(类别)==str and 类别!='auto':

self.类别 = [类别]

else:

self.类别 = 类别

self.k = k

self.f = f

self.噪声级别 = 噪声级别

self.编码字典 = dict(   )

self.先验值 = None

self.随机状态 = 随机状态

def 添加噪声(self, 序列, 噪声级别):

return 序列 * (1 + 噪声级别 *

np.随机标准正态(len(序列)))

定义拟合方法(self, X, y=None):

若类型(self.分类列)=='auto':

self.分类列 = np.定位(X.数据类型 == 类型(object(   )))[0]

临时数据 = X.局部拷贝(:, self.分类列).副本(   )

临时数据['目标列'] = y

self.先验概率 = np.均值(y)

遍历变量 在 self.分类列 中:

平均值 = (临时数据.按组聚合(依据=变量)['目标列']

.聚合(['均值', '计数']))

#计算平滑系数

平滑系数 = (1 / (1 + np.指数(-(平均值['计数'] - self.k) /

self.f)))

#计数越大则整体平均值权重越小

self.编码字典[变量] = 字典(self.先验概率 * (1 -

平滑系数) + 平均值['均值'] * 平滑系数)

返回 self

定义转换方法(self, X):

Xt = X.copy(   )

遍历变量 in 分类集合:

Xt[变量].替换(编码字典[变量],

原地替换=True)

未知值 = \{值:先验概率 for 值 in

X[变量].去重(   )

if 值 不在

编码字典[变量].键集合(   )\}

若 未知值长度 > 0 :

Xt[变量].替换(未知值, 原地替换=True)

Xt[变量] = Xt[变量].转为浮点型

若 噪声强度 > 0 :

若 随机种子 非空:

np.随机数种子(随机种子)

Xt[变量] = 添加噪声(Xt[变量],

---

self.noise_level)

---

return Xt

def fit_transform(self, X, y=None):

self.fit(X, y)

return self.transform(X)

---

函数输入参数说明：

- categories：需要进行目标编码的特征列名。设为'auto'时，类将自动选择对象字符串。

- k（整型）：考虑类别平均值的最小样本数。

- f（整型）：平滑系数，用于平衡类别平均值与先验概率（即相对于所有训练样本的均值）。

- noise_level：为避免过拟合而添加到目标编码的噪声量，建议从极小值开始。

- random_state：当noise_level>0时，用于复现相同目标编码的随机种子。

注意\( \mathrm{k} \)和\( \mathrm{f} \)参数的存在。实际上，对于分类特征的\( i \)级别，我们寻找一个近似值来通过单一编码变量更好地预测目标。用观测到的条件概率替换该级别虽是解决方案，但对少量观测的级别效果不佳。解决方案是使用lambda因子将该级别的观测后验概率（给定编码特征值的目标概率）与先验概率（整个样本的目标概率）混合。这称为经验贝叶斯方法。

实际操作中，我们通过函数决定对分类变量的特定级别使用条件目标值、平均目标值还是两者的混合。这由lambda因子决定：对于固定的\( \mathrm{k} \)参数（通常为单位值，暗示最小单元格频率为两个样本），根据所选\( f \)值会产生不同输出。

<!-- Media -->

<!-- figureText: lambda(n) f=1 f=2 f=3 f=5 f=25 f=50 60 80 100 1.0 0.9 0.8 0.7 0.6 0.5 20 40 -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_243.jpg?x=240&y=213&w=1400&h=948&r=0"/>

图7.3：y轴显示lambda值随f值和分类值样本量（\( x \)轴）的变化曲线

<!-- Media -->

如图所示，\( x \)轴表示分类级别的案例数量，\( y \)轴表示条件目标值的权重。较小的\( f \)值会突然从使用平均值切换到使用条件值；较大的\( f \)值倾向于混合两者，除非处理大样本量的分类级别。因此，固定\( k \)时，较大的\( f \)值意味着更少依赖观测经验频率，更多依赖所有单元格的经验概率。\( f \)的最佳值通常需通过测试（交叉验证支持）确定，因其本身可视为超参数。

经过这些解释后，该类的使用其实相当简单：用要目标编码的特征名和待试参数实例化，拟合训练数据后，即可对任何数据仅转换已拟合特征的目标编码：

---

te = TargetEncode(categories='ROLE_TITLE')

te.fit(train, train['ACTION'])

te.transform(train[['ROLE_TITLE']])

---

该示例沿用我们之前使用的亚马逊员工权限挑战数据集，仅对ROLE_TITLE特征进行目标编码。

除了自行编写代码，您也可以使用https://github.com/scikit-learn-contrib/category_encoders提供的Target Encoder工具包（http://contrib.scikit-learn.org/category_encoders/targetencoder.html）。这是开箱即用的解决方案，其运作方式与本小节代码完全一致。

## 利用特征重要性评估工作成果

过度应用特征工程可能产生副作用。若创建过多相关性特征或与问题无关的特征，会导致模型训练时间延长且效果下降。这看似矛盾，实则因为每个变量都携带噪声（测量或记录误差导致的随机成分），模型可能误将噪声当作有效信号：使用的变量越多，模型捕捉噪声而非信号的概率就越高。因此，应尽量保留训练数据集中相关特征，将特征选择视为特征工程流程的组成部分（剪枝阶段）。

确定需要保留的特征是复杂难题，因为可用特征数量增加时，可能的组合数量也会剧增。存在多种特征选择方法，但首先需考虑数据预处理流程中实施选择的阶段。根据经验，建议将特征选择置于数据预处理流程末端。由于特征间存在方差共享，单独测试每个特征无法评估其有效性，必须整体考量才能准确判断应保留哪些特征。

此外，应通过交叉验证测试所选特征的有效性。当完成所有特征准备、建立稳定流程和可运行模型（无需完全优化，但需正常运作并产出可接受结果）后，即可测试哪些特征应保留或剔除。此时可采用多种特征选择方法：

- 统计学经典方法采用前向添加或后向消除策略，通过逐个测试特征进出预测集的效果。这种方法耗时较长，因其依赖变量内部重要性度量或对模型特定指标表现的影响，每个步骤都需要重新计算。

- 回归模型中，通过稳定性选择流程的lasso选择可揭示重要但相关的特征（该流程可能保留高度相关特征）。稳定性选择采用bagging程序多次测试应保留的特征（仅选择每次测试中系数非零的特征），然后通过投票系统保留最常获得非零系数的特征。

该存储库提供更详细的流程说明：https://github.com/scikit-learn-contrib/stability-selection。

- 基于树的模型（如随机森林或梯度提升）常用分裂带来的杂质减少或目标指标增益进行特征排序，通过阈值剔除最不重要的特征。

- 同样适用于树模型（但可推广至其他模型）的特征随机化测试（或与随机特征的简单对比），可区分真正有助于预测的特征与噪声/冗余特征。Chris Deotte在呼吸机压力预测竞赛中的示例（https://www.kaggle.com/cdeotte/lstm-feature-importance）演示了随机化如何辅助特征选择：该笔记测试了LSTM神经网络中特征的作用，先建立模型记录基准表现，然后逐个打乱特征要求模型重新预测。若预测结果恶化，说明打乱的是重要特征；若结果不变或改善，则表明该特征无影响甚至有害。

重要性评估中同样不存在免费午餐。特征洗牌无需重新训练模型，这在训练新模型耗时的情况下是一大优势。然而，该方法在某些场景会失效——洗牌可能产生无实际意义的虚假输入组合，也可能因高度相关特征的存在而误判（错误认定某个特征重要而另一个不重要）。此时最佳解决方案是直接移除特征（而非洗牌）、重新训练模型，再与基线模型进行性能对比评估。

基于特征洗牌的另一种方法是Boruta（https://github.com/scikit-learn-contrib/boruta_py），它通过随机特征以迭代方式验证模型有效性。其变体BorutaShap（https://github.com/Ekeany/Boruta-Shap）则利用SHAP值实现特征选择与可解释性双重目标。由于特征需多次与随机特征进行统计显著性对比以证明其重要性，这种选择方法通常比简单的特征删除或随机化更可靠。Boruta或BorutaShap可能需要多达100次迭代，且仅适用于基于树的机器学习算法。

若为线性模型选择特征，Boruta可能会过度筛选。因为它会同时考虑特征的主效应和与其他特征的交互作用（而线性模型只需关注主效应及特定交互子集）。此时仍可通过设置最大深度为1的梯度提升树来有效使用Boruta，这样仅评估特征主效应而忽略交互作用。

通过30 Days of ML竞赛中的教程Notebook（https://www.kaggle.com/lucamassaron/tutorial-feature-selection-with-boruta-shap），您可直观了解BorutaShap特征选择的简易快速配置流程。

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_247.jpg?x=242&y=236&w=356&h=357&r=0"/>

<!-- Media -->

## 博扬·通古兹

https://www.kaggle.com/tunguz

博扬·通古兹是深谙特征工程重要性的Kaggle专家（同时亦是XGBoost(c)的忠实拥趸）。我们很荣幸采访到这位NVIDIA机器学习建模师兼Kaggle四重特级大师，聆听他的洞见。

## 您最青睐哪类竞赛？原因何在？在技术方法层面，您在Kaggle的核心竞争力是什么？

我钟爱所有非代码类竞赛，这一偏好随时间不断演变。曾痴迷图像竞赛，但相关工程栈的复杂度已今非昔比；也曾深耕NLP竞赛，可惜这类赛事在Kaggle较为罕见。不过对表格数据问题的热情始终未减——这类曾代表Kaggle精髓的赛题现已近乎绝迹。我仍对该ML领域保持浓厚兴趣，甚至开展了基础研究。相较于ML/DL其他领域，表格数据\( {ML} \)的改进进展缓慢，我认为这里蕴藏巨大机遇。

## 您如何规划Kaggle竞赛策略？与日常工作方法有何差异？

我始终认真对待Kaggle的游戏属性。具体表现为：初期会趣味性地提交简易方案、奇思妙想、他人方案改编或混合模型等。这有助于感知问题本质、有效方法边界及简单技巧的潜力。这些经验部分适用于日常建模，但缺失了关键要素——来自社区和排行榜的反馈支持。独自或小团队工作时，永远无法确知当前方案是否已达最优。

## 请分享您参与过最具挑战性的竞赛及攻克难关的洞见。

Home Credit违约风险竞赛是我Kaggle生涯最具挑战性且最重要的赛事。这场史上规模第二的竞赛恰逢我人生低谷期。信贷核保是极具挑战的数据科学问题，需要精巧的特征工程和可靠的验证方案。我的关键突破是采用简单线性模型进行特征选择，最终助力团队夺冠。至今我仍视此胜利为Kaggle生涯高光时刻。

## Kaggle对您的职业发展有何助益？

Kaggle平台是我机器学习职业生涯中最强大的助推器。在我从事过的四份ML相关工作中，有三份直接源于我在Kaggle上的优异表现。Kaggle认证对职业发展的关键性，怎么强调都不为过。

## 根据你的经验，新手Kaggle选手常忽视哪些问题？你现在掌握的哪些知识希望初学时就知道？

所有机器学习问题（尤其是Kaggle竞赛）有两个关键维度，我长期未能充分重视或投入不足：特征工程和稳健的验证策略。我痴迷于ML算法库，总想尽快搭建模型。但真正决定模型性能上限的，往往来自精妙的特征工程。遗憾的是，特征工程更像艺术而非科学，高度依赖具体模型和数据集。那些最精妙的特征工程技巧，在标准ML课程或资料中几乎从未涉及——其中许多无法言传，需要针对特定问题的洞察力。但培养"优先考虑特征工程"的思维模式是可以训练的，不过这通常需要多年实践才能精通。

你会推荐哪些工具或库用于Kaggle竞赛？

XGBoost就是终极答案！

## 伪标签技术

在训练样本数量影响模型表现的竞赛中，伪标签技术能通过引入测试集的高置信度预测样本来提升分数。其核心是将你认为可靠的测试集预测结果加入训练集。该技术由Wizardry团队在桑坦德客户交易预测竞赛中首创（参阅：https://www.kaggle.com/c/santander-customer-transaction-prediction/discussion/89003），更多数据能帮助模型优化参数，但效果并不稳定。首先，某些竞赛中伪标签毫无必要——添加后可能毫无改善，若伪标签含噪声甚至会适得其反。

遗憾的是，赛前无法确知伪标签是否有效（需实证检验），但绘制学习曲线可暗示增加数据是否有益（参考Scikit-learn示例：https://scikit-learn.org/stable/auto_examples/model_selection/plot_learning_curve.html）。

其次，如何筛选测试集预测结果及优化整个流程极具挑战。常规操作流程如下：

1. 训练初始模型

2. 在测试集进行预测

3. 建立置信度评估标准

4. 筛选待添加的测试集样本

5. 用合并数据重建模型

6. 使用新模型预测并提交

Chris Deotte在Instant Gratification竞赛中提供了完整的伪标签实现范例（https://www.kaggle.com/cdeotte/pseudo-labeling-qda-0-969），掌握几个关键技巧即可应用。

在尝试应用伪标签技术时，需注意以下几点：

- 必须确保模型性能优异，能生成可用于训练的高质量预测结果。否则只会引入更多噪声。

- 由于测试集的预测不可能完全准确，需要区分可用与不可用的预测。若使用交叉验证折叠进行预测，应检查预测结果的标准差（适用于回归和分类问题），仅选取标准差最低的测试样本。若预测概率，则只采用极高或极低的预测概率（即模型置信度较高的案例）。

- 第二阶段将训练样本与测试样本合并时，测试样本数量不得超过\( {50}\% \)。理想比例为\( {70}\% \)原始训练样本搭配30%伪标签样本。若伪标签样本过多，新模型可能过度学习简单测试样本而忽略原始数据，导致蒸馏模型性能不增反降。需注意，模型训练过程中本应学习处理标签噪声，但伪标签样本恰恰缺乏这种噪声。

切记伪标签并非完全可靠，将测试预测用作训练样本会部分污染数据。只有当收益大于负面影响时，这种技巧才值得采用。

- 若需通过验证集进行早停、超参数调优或模型评估，切勿在验证阶段使用伪标签。这些标签可能产生严重误导。基于前述原因，请始终使用原始训练样本。

- 理想情况下，在训练伪标签预测模型与最终模型（同时使用原始标签和伪标签）时应采用不同模型架构。这能确保模型不仅继承先前模型的信息，还能从伪标签中提取新知识。

显然，伪标签技术更像是一门艺术而非精确科学。它能在特定竞赛中成为制胜关键，但需要精湛运用才能见效。建议将其视为辅助工具，至少提交一次基于伪标签的解决方案。

## 自编码器去噪技术

自编码器最初以非线性数据压缩（一种非线性PCA）和图像去噪著称，直到Michael Jahrer（https://www.kaggle.com/mjahrer）在Porto Seguro安全驾驶预测大赛（https://www.kaggle.com/c/porto-seguro-safe-driver-prediction）中成功运用后，才被认可为表格竞赛的有效工具。该保险风险评估比赛（超5000人参与）以特征噪声显著著称。Jahrer阐释了如何通过去噪自编码器（DAE）重构数值数据表征，为后续神经网络监督学习提供更优输入。DAE能基于网络中心隐藏层及中间编码层的激活值，生成包含海量特征的新数据集。

在其著名帖子（https://www.kaggle.com/c/porto-seguro-safe-driver-prediction/discussion/44629）中，Jahrer指出DAE不仅能降噪，还可自动创建新特征，其表征学习方式类似图像比赛。他透露DAE的核心秘诀不在于网络层数，而在于为数据增强注入的噪声类型。同时他强调该技术需合并训练集与测试集，暗示其仅适用于Kaggle竞赛场景。事实上，该技术在此次夺冠后便从论坛消失，直到最近表格数据竞赛系列才重现。

从技术角度看，DAE由编码器与解码器组成。编码器以训练数据为输入，经过若干全连接层处理。理想情况下，中间隐藏层的激活值能完整编码训练信息。若该层节点数少于输入维度，则实现数据压缩（统计学上可视为对输入数据生成过程的潜在维度表征）；否则仅完成冗余消除与信噪分离（这已是良好结果）。

在解码器部分，网络层逐步扩展直至恢复原始输入维度。通过对比输出与输入计算误差损失，反向传播至整个网络。

由此可归纳两类DAE架构：

- 瓶颈式DAE：借鉴图像处理思路，将分隔编码/解码部分的中间层激活值作为新特征。这种沙漏型结构先逐层缩减神经元至瓶颈层，再逐步扩展。隐藏层数恒为奇数。

<!-- Media -->

<!-- figureText: Input Reconstruction Decoder Encoder Bottleneck -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_252.jpg?x=521&y=211&w=983&h=570&r=0"/>

图7.4：瓶颈式DAE仅提取瓶颈层权重作为特征

<!-- Media -->

- 深度堆叠DAE：提取所有隐藏层激活值，不区分编码/解码/中间层。此类架构各层维度相同，隐藏层数可奇可偶。

<!-- Media -->

<!-- figureText: Input Reconstruction Hidden layers -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_252.jpg?x=490&y=1056&w=1017&h=582&r=0"/>

图7.5：深度堆叠DAE将所有隐藏层权重作为特征

<!-- Media -->

如前所述，关键环节是向DAE注入随机噪声。为有效训练任何DAE，需通过噪声实现数据增强，防止过参数化神经网络单纯记忆输入（即过拟合）。在Porto Seguro比赛中，Jahrer采用交换噪声技术，具体描述如下：

我对特征值按上表"inputSwapNoise"概率进行采样替换。0.15表示15%的特征值会被其他行的数值替代。

所述方法本质上是一种称为混合增强（mixup）的技术（该技术也用于图像增强：https://arxiv.org/abs/1710.09412）。在表格数据的混合增强中，需设定混合概率。根据该概率，将样本中的部分原始值替换为来自同一训练数据中相似度不同的样本值。

丹泽尔（Danzel）在其演练教程（https://www.kaggle.com/springmanndaniel/1st-place-turn-your-data-into-daeta）中描述了三种实现方式：按列处理、按行处理和随机处理：

- 在列向噪声替换中，交换指定数量列中的值。需交换值的列比例由混合概率决定。

- 在行向噪声替换中，每行固定交换一定数量的值。本质上每行包含相同比例的替换值（基于混合概率），但被替换的特征会逐行变化。

- 在随机噪声替换中，根据混合概率确定待替换值的数量，并从整个数据集中随机选取（效果上与行向替换类似）。

与伪标签技术类似，去噪自编码器（DAE）更像艺术而非科学，这意味着需要反复试错。它并非总是有效，且针对某问题的成功细节往往无法复用于其他问题。要构建适合竞赛的高效DAE，需持续关注以下需测试调优的环节：

- DAE架构（深层堆叠通常效果更好，但需确定每层神经元数量和总层数）

- 学习率与批大小

- 损失函数（区分数值型与类别型特征的损失计算亦有助益）

- 停止点（最低损失未必最优；建议使用验证集和早停机制）根据问题特性，搭建正确架构并使其有效运行可能面临挑战。但您的努力或将在最终私有排行榜上获得回报。事实上，在近期表格类竞赛中，DAE技术已成为多个夺冠方案的核心组件：

- 丹泽尔（https://www.kaggle.com/springmanndaniel）在https://www.kaggle.com/c/tabular-playground-series-jan-2021/discussion/216037中披露，其使用了三层1500神经元网络的隐藏权重，将原始数据从14列扩展至4500列。该处理后的新数据集被用作其他神经网络和梯度提升模型的输入。

- 张任（https://www.kaggle.com/ryanzhang）在https://www.kaggle.com/c/tabular-playground-series-feb-2021/discussion/222745讨论其方案并开源代码（https://github.com/ryancheunggit/Denoise-Transformer-AutoEncoder），表明其采用堆叠Transformer编码器而非传统的线性ReLU隐藏层（此方法可能导致训练合格DAE耗时达20小时）。他还建议通过噪声掩模向数据添加随机噪声，并基于原始数据重建误差和噪声掩模误差计算复合损失。这种复合损失有助于网络更好收敛。研究GitHub代码和Kaggle讨论帖中的图表将助您理解并复现这一创新方法。

- 简TT（https://www.kaggle.com/jiangtt）发现DAE关键技术（特别是通过添加噪声创建新观测值）可不构建完整DAE而提升算法训练效果：https://www.kaggle.com/c/tabular-playground-series-apr-2021/discussion/235739

若不愿耗费过多时间构建DAE，但仍想探索该技术对当前竞赛的适用性，可测试几种现成方案。首先参考Hung Khoi的PyTorch网络Notebook（https://www.kaggle.com/hungkhoi/train-denoise-transformer-autoencoder）并按需调整，或使用Jeong-Yoon Lee开发的Kaggler库（https://www.kaggle.com/jeongyoonlee）。Lee在其Notebook中演示了该库在Tabular Playground竞赛中的应用：https://www.kaggle.com/jeongyoonlee/dae-with-2-lines-of-code-with-kaggler

## 表格竞赛中的神经网络应用

在探讨了自编码器神经网络后，我们需要更全面地讨论神经网络如何助力表格类竞赛。虽然梯度提升方案仍在表格竞赛（及实际项目）中占据主导地位，但神经网络有时能捕捉梯度提升模型无法识别的特征信号，既可成为卓越的独立模型，也能在集成模型中大放异彩。

正如众多顶尖数据科学家反复强调的，在表格数据问题中，融合多样化模型（如神经网络与梯度提升模型）总能产生优于单一模型的效果。前Kaggle冠军Owen Zhang在此访谈中详细阐述了如何巧妙结合神经网络与GBM以提升竞赛表现：https://www.youtube.com/watch?v=LgLcfZjNF44。

为表格竞赛快速构建神经网络已非难事。借助TensorFlow/Keras和PyTorch等库，配合TabNet等预制网络架构，开发过程变得极为便捷。

快速入门神经网络构建可参考多种资源。我们特别推荐本社出版的《TensorFlow机器学习实战指南》（https://www.packtpub.com/product/machine-learning-using-tensorflow-cookbook/9781800208865），其中第七章专门讲解使用TensorFlow构建DNN处理表格数据预测问题。该书还包含大量TensorFlow在Kaggle中的应用技巧。

此外，您可参考\( {ML} \)竞赛30天活动中推荐的相关网络资源：

- 观看TensorFlow处理表格数据教程视频：https://www.youtube.com/watch?v=nQgUt_uADSE

- 使用GitHub教程代码：https://github.com/1massaron/deep_learning_for_tabular_data

- 最关键的是，在此获取应用于竞赛的教程Notebook：https://www.kaggle.com/lucamassaron/tutorial-tensorflow-2-x-for-tabular-data 构建方案时需重点考虑：

- 采用GeLU、SeLU或Mish等激活函数替代ReLU，多篇论文指出它们更适合表格数据建模，我们的实践也证实其性能更优

- 尝试不同批次规模

- 应用mixup数据增强技术（自编码器章节已讨论）

- 对数值特征进行分位数转换，强制生成均匀分布或高斯分布

- 善用嵌入层，但需注意嵌入层无法建模所有特征关系。实际上它们会遗漏嵌入特征与其他特征的交互作用（因此需要通过直接特征工程将这些交互强制注入网络）

特别提醒：嵌入层具有可复用性。其本质是通过矩阵乘法将高基数变量的稀疏独热编码降维为稠密低维表示。保存训练好的神经网络嵌入矩阵后，可将其转化应用于梯度提升、线性模型等多种其他算法。

参考图7.6可清晰理解24级分类变量的处理流程。该图展示了分类特征值如何从文本/整型转化为神经网络可处理的向量：

<!-- Media -->

<!-- figureText: Text on variable: ID_8080 [001000000000000000000000000000000] Weights matrix (size input x output, i.e. 24x4) Backpropagation Pre-processing Label Encoding: \( 3/{24} \) One hot Encoding vector (size \( = {24} \) ,) Embeddings [[0.48 0.997 0.706 0.475] tf.keras.layers. ... Embedding ( [0.794 0.922 0.086 0.921]] input_dim, output_dim) Output vector (size = 4,) \( \left\lbrack  {{0.283},{0.34},{0.789},{0.867}}\right\rbrack \) Dense layers Fully connected Target -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_257.jpg?x=303&y=212&w=1260&h=868&r=0"/>

图7.6：嵌入层工作原理示意图

<!-- Media -->

一切始于了解特征包含多少个不同的取值。这构成了字典大小，是关键信息。本例中我们考虑具有24个不同取值的特征。通过该信息可创建24维的独热编码向量来表示每个可能的特征值。随后将该向量与矩阵相乘，矩阵的行尺寸对应独热编码向量的维度，列尺寸对应输出维度。通过这种向量-矩阵乘法，分类变量输入将被转化为多维数值形式。神经网络的反向传播算法会更新矩阵中的每个值，确保乘法运算能获得最具预测性的结果。若不想在TensorFlow或PyTorch中自建深度神经网络，可采用几种开箱即用的架构方案。这些方案之所以能直接使用，或因已封装打包，或因其他Kaggle选手根据原论文实现了代码。根据它们在表格竞赛中的优异表现，以下是参与表格竞赛时可尝试的主流方案：

- TabNet是谷歌研究人员提出的网络架构（Arık, S. O. and Pfister. T. Tabnet: Attentive interpretable tabular learning. arXiv 2020. https://www.aaai.org/AAAI21Papers/ AAAI-1063. ArikS.pdf），能智能处理分类与数值特征并筛选相关特征。其需调参的超参数不多，但调参前后结果差异显著（因此需投入时间优化性能）。现有多个实现版本，如优秀的pytorch-tabnet包（https://github.com/dreamquark-ai/tabnet），或Yirun Zhang开发的代码（https://www.kaggle.com/gogo827jz），详见https://www.kaggle.com/ludovick/introduction-to-tabnet-kfold-10-training 与 https://www.kaggle.com/ludovick/introduction-to-tabnet-kfold-10-inference，这些实现均针对"作用机制预测（MoA）"竞赛设计。

- 神经 oblivious 决策集成（NODE）是一种在神经网络中模拟决策树工作的架构（Popov, S., Morozov, S., and Babenko, A. Neural oblivious decision ensembles for deep learning on tabular data. arXiv preprint arXiv:1909.06312, 2019. https://arxiv.org/abs/1909.06312）。可使用Yirun Zhang提供的TensorFlow实现（https://www.kaggle.com/gogo827jz/moa-neural-oblivious-decision-ensembles-tf-keras）或PyTorch实现（https://www.kaggle.com/ gogo827jz/moa-public-pytorch-node）。

- 可采用多种模型，如Wide & Deep、DeepFM、xDeepFM、AutoInt等基于因子分解机的模型（多用于点击率预估）。无需自行构建这些神经网络架构，可借助DeepCTR（https://github.com/shenweichen/DeepCTR）或DeepTables（https://github.com/DataCanvasI0/deeptables）等工具包——这些由Categorical Feature Encoding Challenge II竞赛冠亚军Chang-hao Lee（https://www.kaggle.com/leechh）与Jian Yang（https://www.kaggle.com/ jackguagua）推荐。总之，可通过组合分类特征的嵌入层与数值特征的稠密层来构建表格数据专用神经网络。若效果不佳，众多优质现成方案可供选择。时刻关注新工具包的出现，它们可能提升Kaggle竞赛与实际项目的表现。根据经验建议：别指望神经网络成为表格竞赛的最佳模型（这种情况极少），应将梯度提升模型等传统表格数据解决方案与神经网络融合，因为它们能从数据中捕捉不同信号，通过集成实现优势互补。

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_259.jpg?x=242&y=764&w=358&h=362&r=0"/>

<!-- Media -->

## 让-弗朗索瓦·普吉特

https://www.kaggle.com/cpmpml

我们采访了让-弗朗索瓦·普热（又名CPMP），探讨了可重复性的重要性、数据处理方法、他参与过的最佳竞赛等话题。作为Kaggle竞赛与讨论版块的双料特级大师，以及NVIDIA RAPIDS团队的杰出工程师，他为我们分享了许多深刻见解。编辑尤其欣赏他关于科学方法的论述。

## 您最青睐哪种类型的竞赛？为什么？在技术方法和解决思路上，您在Kaggle的专长是什么？

我偏好具有科学背景或与我专业相关的竞赛。除非数据来自精确的物理模拟，否则我不喜欢匿名数据和合成数据。更广泛地说，我钟爱那些涉及陌生领域的Kaggle竞赛——这正是我能最大化学习效益的契机。虽然这不是获取积分最高效的方式，却是我最乐在其中的选择。

您如何规划Kaggle竞赛策略？这与日常工作方法有何不同？

我首先会深入分析数据并尽可能理解其内涵。通过\( x \)轴和\( y \)轴的两个特征（或衍生特征）绘制样本点，并用第三个特征进行颜色编码，我着力寻找其中的规律性——尤其是预测性模式。目标变量也可作为三个特征之一。我大量运用可视化手段，因为我相信人类视觉是最强大的数据分析工具。

其次我会重点研究模型或流程的性能评估方法。准确评估模型表现至关重要，通常采用k折交叉验证的变体。但折数划分需适配竞赛类型：预测类竞赛采用时间序列划分，当样本存在关联性（如相同用户ID的操作）时则采用分组k折。

接着构建从数据预处理到提交的端到端基线模型进行验证。对于代码竞赛而言，确保流程正确性尤为关键。

随后尝试更复杂模型（深度学习场景）或更多特征（使用XGBoost/RAPIDS/sklearn时）。通过提交结果验证本地评估分数与公开测试分数的相关性，若相关性良好则逐渐减少提交频次。

几周后集中进行超参数调优，通常只在竞赛临近结束时进行1-2次。因为这是导致过拟合的主要风险之一，我对此始终保持警惕。

## 请分享您遇到过最具挑战性的竞赛，以及您破局的关键洞察

我最自豪的是TalkingData广告欺诈检测挑战赛。面对仅含少量特征却多达5亿条点击记录的数据集（当时仅使用64GB内存设备），我创新性地发现：1）促成应用下载的点击必定是用户在该应用页面的最后一次点击，"同一用户对同一应用的下次点击间隔时间"成为核心特征；2）当存在相同时间戳的多条点击时，下载行为必然发生在最后一条；3）采用矩阵分解近似特征共现关系，通过在Keras实现libFM模型并加入潜在向量特征，最终在特级大师团队云集的竞赛中独获第六名——此时我尚未获得Kaggle特级大师称号。

## Kaggle对您的职业发展有何助益？

Kaggle曾两次推动我的职业发展：在IBM期间，它成为我获取机器学习前沿实践的重要知识库，这些洞见直接指导了IBM Watson系列机器学习工具的研发。

例如2016年当IBM还是Java/Scala阵营时，我力主引入Python生态支持；若没有我的坚持，IBM可能会完全错过Python机器学习浪潮。同样在IBM只愿支持Spark ML和TensorFlow时，我早早推动了XGBoost的整合。

Kaggle第二次帮助我是获得现在这份工作。英伟达(NVIDIA)当时正在寻找具有良好社交影响力的Kaggle竞赛大师(GM)，以协助推广其技术栈，包括RAPIDS GPU加速机器学习套件。

## 根据你的经验，新手Kaggle用户常忽视什么？你现在掌握的哪些知识希望刚开始时就知晓？

Kaggle用户与其他数据科学家的关键区别在于模型性能评估能力。他们必须精通此道，否则会选择在公开排行榜表现优异却在私有排行榜表现糟糕的提交方案。当掌握构建私有排行榜优秀模型的技巧时，就意味着能构建在新数据上表现良好（即不过拟合）的模型。

新手常犯的另一个错误是询问方法/模型\( X \)是否适用于某竞赛。我的回答永远是："试过才知道。"人们常忽略机器学习是实验科学这一本质。要构建优秀模型必须遵循科学方法：

- 提出假设（例如：添加此特征或神经网络层将提升流程性能）

- 设计实验验证假设（训练修改后的流程）

- 分析实验结果（交叉验证分数是否提升？哪些方面改善？哪些恶化？）

每个实验都应能验证或推翻假设。因此每次只能改变一个变量。新手常同时改动多个因素，导致无法判断实际效果。

## 有哪些特别推荐的数据分析与机器学习工具或库？

数据探索主要使用Matplotlib绘图。小数据集用Pandas处理，大数据集用RAPIDS的cuDF。机器学习使用RAPIDS的cuML、GPU加速的XGBoost和PyTorch。优先选用预训练模型，如Hugging Face的NLP模型或timm包的图像分类模型。

# 参加竞赛时最需要牢记或做到什么？

确保投入足够时间。

## 本章小结

本章探讨了Kaggle表格类竞赛。由于这类竞赛所需知识大多与标准数据科学重叠，我们重点聚焦Kaggle特有技巧。

从新推出的Tabular Playground系列出发，我们涉及了可复现性、探索性数据分析(EDA)、特征工程、特征选择、目标编码、伪标签技术及表格数据神经网络应用等主题。

想要制胜竞赛，EDA是关键阶段。这个过程高度非结构化且依赖数据类型。除通用建议外，我们重点介绍了t-SNE和UMAP等能快速呈现数据集全貌的技术。特征工程阶段同样依赖数据类型，因此我们列举了多种可针对具体情况尝试的方案。特征选择方面，在简要概述后重点讲解了基于特征重要性和随机化的通用技术。

在解释完目标编码（需特别指出无法通过自动化方式处理）后，我们接着探讨了现实项目中可能不会采用、但在Kaggle竞赛中表现优异的特殊技术：用于表格竞赛的伪标签技术和去噪自编码器。最后，在讨论如何通过神经网络嵌入层处理分类特征后，我们简要概述了适用于表格数据的预制神经网络架构。

下一章中，我们将通过讨论超参数优化的最佳实践，完整介绍应对表格竞赛所需的所有技术。

## 加入本书的Discord空间

加入本书的Discord工作区，每月参与作者问答专场：

https://packt.link/KaggleDiscord

##

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_265.jpg?x=250&y=308&w=168&h=239&r=0"/>

<!-- Media -->

超参数优化

Kaggle解决方案的表现不仅取决于所选学习算法类型。除了数据和特征外，算法超参数——即训练前必须设定且无法在训练过程中学习的参数——也起着决定性作用。在表格数据竞赛中，选择合适的变量/数据/特征最为有效；而超参数优化则对所有类型竞赛都至关重要。事实上，在数据和算法固定的情况下，超参数优化是提升算法预测性能、冲击排行榜的唯一可靠途径。它还能提升集成模型效果，因为调优模型的集成始终优于未调优模型的集成。

你可能听说，若了解参数选择对算法的影响，手动调参是可行的。许多Kaggle大师和特级大师宣称常在竞赛中直接调参。他们采用二分法操作风格，针对关键超参数逐步缩小参数值区间，直至找到最佳值，再转向其他参数。这种方法在参数存在单一最小值且相互独立时效果显著，此时搜索主要依赖算法经验。但根据我们的实践，Kaggle上大多数任务并非如此。问题复杂性和算法精密度需要系统化的搜索算法支持。因此本章将探讨如何扩展交叉验证方法，寻找能泛化至测试集的最佳超参数，以应对竞赛中的时间和资源压力。我们将重点介绍贝叶斯优化方法——这是基于可用资源优化复杂模型和数据问题的成熟方案。我们不仅限于搜索预设超参数的最优值，还将深入探讨神经网络架构问题。

本章将涵盖以下主题：

- 基础优化技术

- 关键参数及其使用方法

- 贝叶斯优化

现在开始！

## 基础优化技术

Scikit-learn包提供的核心超参数优化算法包括网格搜索和随机搜索。近期贡献者还加入了减半算法来提升这两种策略的性能。

本节将详解这些基础技术。掌握它们不仅能获得特定问题的有效优化工具（如SVM通常采用网格搜索优化），还能理解超参数优化的基本原理。

首先，必须明确所需的要素包括：

- 需要优化超参数的模型

- 包含每个超参数搜索值边界的搜索空间

- 交叉验证方案

- 评估指标及其评分函数

这些要素在搜索方法中共同作用，以确定您寻求的解决方案。下面我们来看具体运作方式。

## 网格搜索

网格搜索是一种穷举遍历超参数的方法，在高维空间中不可行。您需要为每个参数选定一组待测试值，然后测试该集合中所有可能的组合。其穷举性正源于此：尝试所有可能性。虽然这种简单算法受维度诅咒影响，但优势在于其具有令人尴尬的并行性（该计算机科学术语定义参见https://www.cs.iusb.edu/~danav/teach/b424/ b424_23_embpar.html）。这意味着只要有足够处理器运行搜索，就能快速获得最优调参结果。

以分类问题和支持向量机分类（SVC）为例。无论是分类还是回归问题，支持向量机（SVM）很可能是您最常使用网格搜索的机器学习算法。通过Scikit-learn的make_classification函数，我们可以快速生成分类数据集：

---

from sklearn.datasets import make_classification

from sklearn.model_selection import train_test_split

X, y = make_classification(n_samples=300, n_features=50,

n_informative=10,

n_redundant=25, n_repeated=15,

n_clusters_per_class=5,

flip_y=0.05, class_sep=0.5,

random_state=0)

---

下一步，我们定义一个基础SVC算法并设置搜索空间。由于SVC的核函数（SVM中用于转换输入数据的内部函数）决定了需要设置的不同超参数，我们提供了一个包含两套参数字典的列表，分别对应不同类型核函数所使用的搜索空间。同时设定评估指标（本例使用准确率，因目标类别完全平衡）：

---

from sklearn import svm

svc = svm.SVC(   )

svc = svm.SVC(probability=True, random_state=1)

from sklearn import model_selection

search_grid = [

{'C': [1, 10, 100, 1000], 'kernel': ['linear']},

{'C': [1, 10, 100, 1000], 'gamma': [0.001, 0.0001],

'kernel': ['rbf']}

	]

scorer = 'accuracy'

---

本例中，线性核函数无需调整gamma参数，而该参数对径向基函数核至关重要。因此我们提供两套参数字典：第一套包含线性核参数，第二套包含径向基函数核参数。每套字典仅关联对应核函数类型及其相关参数范围。

需特别注意：评估指标可能与算法优化的损失函数不同。如第5章"竞赛任务与评估指标"所述，竞赛评估指标可能相异，但无法修改算法损失函数。此时根据评估指标调参仍有助于获得性能良好的模型。虽然调参围绕算法损失函数进行，但最终获得的超参数组合将在约束条件下返回最佳评估指标——这可能并非理论最优解，但通常相去不远。

所有要素（模型、搜索空间、评估指标、交叉验证方案）被整合到GridSearchCV实例中，随后将模型拟合至数据：

---

search_func = model_selection.GridSearchCV(estimator=svc,

param_grid=search_grid,

评分器=scorer,

并行任务数=-1,

交叉验证折数=5)

搜索函数.fit(X, y)

打印 (搜索函数.最佳参数_)

打印 (搜索函数.最佳分数_)

---

经过一段时间后（具体取决于运行优化的机器配置），您将获得基于交叉验证结果的最佳参数组合。总之，网格搜索是一种非常简单的优化算法，能充分利用多核计算机的优势。它适用于无需过多调参的机器学习算法（如支持向量机、岭回归和套索回归），但在其他情况下适用性相当有限。首先，它仅能通过离散选择来优化超参数（需要预先设定有限的候选值范围）。此外，对于需要调整多个超参数的算法，其效果往往不佳。这是因为搜索空间复杂度呈指数级增长，且这种盲目尝试参数值的搜索方式会导致大量无效计算。

## 随机搜索

随机搜索通过对搜索空间进行随机采样，在高维空间中具有可行性，因此被广泛实际应用。但需注意，与网格搜索类似，随机搜索无法利用先前实验信息来选择后续参数配置。此外，要想快速找到最优解，除了寄希望于运气外别无他法。

随机搜索效果惊人且原理简单。尽管依赖随机性，但并非完全凭运气运作——这类似于统计学中的随机抽样原理：只要进行足够多的随机测试，就有很大概率直接找到最优参数，而无需在性能相近的参数组合上浪费计算资源。

当需要设置的参数过多时，许多自动机器学习系统（参见Golovin, D.等人2017年发表的《Google Vizier：黑盒优化服务》）会采用随机搜索。经验法则是：当超参数优化问题的维度较高时（例如超过16维），就应考虑使用随机搜索。

下面我们使用随机搜索重跑前例：

---

import scipy.stats as stats

from sklearn.utils.fixes import loguniform

参数字典 = \{'核函数': ['线性', '径向基函数'],

'正则化系数': loguniform(1, 1000),

'gamma': 对数均匀分布(0.0001, 0.1)

	\}

评分器 = '准确率'

搜索函数 = 模型选择.随机搜索交叉验证

(估计器=支持向量分类器, 参数分布=搜索字典, 迭代次数=6,

评分=评分器, 并行任务数=-1, 交叉验证折数=5)

搜索函数.fit(X, y)

打印 (搜索函数.最佳参数_)

打印 (搜索函数.最佳分数_)

---

请注意，现在我们无需关心针对不同核函数在独立空间进行搜索。与网格搜索不同——网格搜索会系统性地测试每个参数（包括无效参数）从而耗费计算时间——此处的搜索效率不受测试超参数集的限制。搜索过程不依赖无关参数，而是由随机性引导；每次尝试都有价值，即便在选定核函数的众多参数中仅测试了一个有效参数。

## 减半搜索

如前所述，网格搜索和随机搜索都是以无指导方式工作的：即便某些测试发现特定超参数不影响结果，或某些值区间无效，这些信息也不会传递到后续搜索中。

因此，Scikit-learn近期引入了HalvingGridSearchCV和HalvingRandomSearchCV评估器，它们可通过对网格搜索和随机搜索调参策略应用连续减半法来搜索参数空间。

减半法的首轮测试会评估大量超参数组合，但仅消耗少量计算资源。这是通过使用训练数据中的少量案例子样本进行测试实现的。较小的训练集需要更少的计算量进行测试，因此能以性能估算精度下降为代价节省资源（即时间）。首轮测试可筛选出在该问题上表现较好的候选超参数值子集，用于训练集规模扩大的第二轮测试。后续轮次采用相同方式，随着测试值范围的收窄（此时测试需要更长时间执行，但能获得更精确的性能估算），分配的训练集子样本规模逐轮增大，同时候选参数数量持续减半。

以下是对前文问题的应用示例：

<!-- Media -->

---

from sklearn.experimental import enable_halving_search_cv

from sklearn.model_selection import HalvingRandomSearchCV

搜索函数 = 减半随机搜索CV(估计器=svc,

参数分布=搜索字典,

资源='n_samples',

最大资源=100,

激进消除=True,

评分=评分器,

并行作业=-1,

	CV=5,

随机状态=0)

---

搜索函数.拟合(X, y)

打印 (搜索函数.最佳参数_)

打印 (搜索函数.最佳分数_)

<!-- Media -->

通过这种方式，减半算法通过候选者的选择为后续优化步骤提供信息。在接下来的章节中，我们将讨论更智能的方法，以实现对超参数空间更精确和高效的搜索。

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_271.jpg?x=241&y=1644&w=359&h=364&r=0"/>

<!-- Media -->

## 小野寺和树

https://www.kaggle.com/onodera

让我们暂停一下，采访另一位Kaggle高手。小野寺和树是竞赛大师和讨论大师，拥有约7年的竞赛经验。他同时也是NVIDIA的高级深度学习数据科学家，以及NVIDIA KGMON（NVIDIA Kaggle大师团队）的成员。

## 你最喜欢哪种类型的竞赛？为什么？在技术和解决方法方面，你在Kaggle上的专长是什么？

Instacart市场篮子分析。这个竞赛对Kaggle社区来说相当具有挑战性，因为它使用了与客户随时间变化的订单相关的匿名数据，来预测用户下一次订单中会包含哪些之前购买过的产品。我喜欢这个竞赛的原因是我热爱特征工程，并且我能想出一些其他人想不到的优秀且有趣的特征，这使我在竞赛中获得了第二名。

你如何着手参加Kaggle竞赛？这种方式与你日常工作有何不同？

我会设想模型如何运作，并深入研究假阴性和假阳性问题。这与日常工作方法相同。

## 请讲述你参加过最具挑战性的竞赛，以及你用来解决问题的洞察方法

人类蛋白质图谱单细胞分类赛。这本质上是个实例分割竞赛，但未提供掩码标注，因此转化为弱监督的多标签分类问题。我构建了一个两阶段流水线来消除标签噪声。

## Kaggle对你的职业发展有帮助吗？具体体现在哪些方面？

当然。我现在就职于英伟达KGMON（Kaggle顶级大师）团队。Kaggle举办各类机器学习竞赛，涵盖表格数据、图像、自然语言和信号等不同数据类型，以及工业、金融、天文、病理学、体育、零售等多领域。除了Kaggle玩家，恐怕没人能接触并精通如此多样的数据。

## 根据你的经验，新手Kaggle玩家常忽视哪些要点？你现在掌握的哪些知识希望初学时就知道？

目标分析。还有种子平均法常被低估——总是简单却有效。

## 你在过往竞赛中犯过哪些错误？

目标分析。顶尖团队总能更透彻地分析目标，所以当我在比赛中名次不佳时，就会研究冠军方案——他们总能揭示我在竞赛期间忽略的数据认知。

# 对于数据分析或机器学习，有哪些特别推荐的工具或库？

Python和Jupyter Notebook足矣。

# 参加竞赛时最需要牢记或做到的关键是什么？

若能从失败中汲取教训，就未尝真正失败。

你是否使用其他竞赛平台？它们与Kaggle相比如何？

KDD杯和RecSys。这两个平台都达到了有趣且具有挑战性的基本要求。

## 关键参数及其使用方法

接下来的问题是为每种模型选择正确的超参数组合。具体而言，为了优化效率，您需要了解针对不同算法实际需要测试的各超参数值。

本节将探讨Kaggle竞赛中最常用的模型（特别是表格数据模型），并讨论为获得最佳效果需要调整的超参数。我们将针对通用表格数据问题，区分传统机器学习模型与梯度提升模型（后者对参数空间的要求更为严苛）。

关于神经网络，我们会在介绍标准模型时提供具体参数调整建议（例如TabNet神经网络模型需要设置特定参数才能正常运行）。但Kaggle竞赛中深度神经网络的优化大多针对定制模型而非标准模型。因此除学习率和批量大小等基础参数外，神经网络优化需基于模型架构特性进行专门处理。本章末尾将展示使用KerasTuner（https://keras.io/keras_tuner/）进行神经架构搜索(NAS)的实例。

## 线性模型

需要调优的线性模型通常是带正则化的线性回归或逻辑回归：

- C：搜索范围应为np.logspace(-4,4,10)；值越小表示正则化强度越大

- alpha：搜索范围应为np.logspace(-2,2,10)；值越小/越大均表示更强的正则化（注：使用lasso时较大值需要更长的处理时间）

- 11_ratio：从[.1, .5, .7, .9, .95, .99, 1]中选择；仅适用于弹性网络

在Scikit-learn中，根据算法不同，您会遇到超参数\( \mathrm{C} \)（逻辑回归）或alpha（lasso/ridge/弹性网络）

## 支持向量机

支持向量机(SVM)是强大的监督学习技术家族，可自动拟合线性和非线性模型，适用于分类与回归问题。Scikit-learn基于LIBSVM（完整的SVM分类/回归实现库）和LIBLINEAR（适合大规模数据集特别是稀疏文本数据的线性分类库）提供实现。SVM在优化过程中会通过最大化类别间隔的决策边界来实现分类目标。

虽然SVM在默认参数下表现良好，但通常并非最优。您需要通过交叉验证测试不同参数组合来寻找最佳配置。按重要性排序需设置以下参数：

- C：惩罚系数。降低该值会增大类别间隔，从而忽略更多噪声但也会增强模型泛化能力。最佳值通常位于np.\( \operatorname{logspace}\left( {-3,3,7}\right) \)范围内

- kernel：决定SVM的非线性实现方式，可选'linear'/'poly'/'rbf'/'sigmoid'或自定义核函数。最常用的是rbf核

- degree：配合kernel='poly'使用，决定多项式展开维度。其他核函数会忽略此参数。通常2到5之间的值效果最佳

- gamma（伽马）：'rbf'、'poly'和'sigmoid'核函数的系数。较高值能更好地拟合数据，但可能导致过拟合。直观理解，gamma代表单个样本对模型的影响力。低gamma值使每个样本的影响范围更广，由于需考虑更多数据点，SVM决策边界会趋于平滑；高gamma值则使决策边界更关注局部点分布，导致更曲折的边界曲线。建议超参数搜索范围为np.logspace(-3, 3, 7)。- nu：在nuSVR和nuSVC中，该参数为靠近边界且分类错误的训练点设置容错度，可忽略边界附近的误分类点从而使决策边界更平滑。取值范围应为\( \left\lbrack  {0,1}\right\rbrack \)（相对于训练集的比例），作用类似参数C，较高值会扩大边界间隔。

- epsilon（ε）：该参数定义SVR训练时的误差容忍带，在此范围内预测错误不施加惩罚。建议搜索范围为np.logspace(-4, 2, 7)。

- penalty（惩罚项）、loss（损失函数）和dual（对偶问题）：LinearSVC接受('11','squared_hinge',False)、('12','hinge',True)、('12','squared_hinge',True)和('12','squared_hinge',False)组合。其中('12','hinge',True)组合等效于SVC(kernel='linear')学习器。

虽然SVM看似需设置众多超参数，但多数参数仅针对特定实现或核函数，实际只需选择相关参数即可。

## 随机森林与极端随机树

随机森林算法的核心思想由Leo Breiman和Adele Cutler提出，其名称至今仍是他们的商标（尽管算法已开源）。Scikit-learn中以RandomForestClassifier和RandomForestRegressor实现。

随机森林运作方式类似Leo Breiman提出的装袋法，但仅使用二叉分裂决策树并允许完全生长。其通过自助采样为每棵树选择样本，且在每次节点分裂时随机选取特征子集。这种在分裂时随机选择样本和特征的方式，使得集成中的树彼此差异显著且不相关。当集成结果时，分布两端的极值会相互抵消从而降低方差。换言之，装袋算法保证了预测多样性，能发现单一学习器（如决策树）可能遗漏的规则。这种多样性有助于构建比集成中任何单棵树更具预测力的平均模型。

极端随机树（Extra Trees）通过ExtraTreesClassifier/ExtraTreesRegressor类实现，是一种随机性更强的随机森林变体。它以增加估计偏差为代价降低方差估计，在CPU效率上显著优于随机森林，特别适合处理大规模样本和特征数据。其核心差异在于分裂方式：随机森林会从随机特征子集中精选最佳分裂值，而极端随机树完全随机选择分裂特征和分裂值，虽可能牺牲分裂效果（导致偏差），但大幅减少了计算量。两种算法的关键超参数包括：

- max_features（最大特征数）：控制每次分裂时考虑的特征数量，直接影响算法性能。该值越小计算越快，但偏差越高。

- min_samples_leaf（最小叶样本数）：该参数用于控制树的深度。数值增大会降低方差但增加偏差。

- bootstrap（自助采样）：布尔值参数，决定是否启用自助采样法。

- n_estimators（树的数量）：决策树的数量需注意，虽然树越多效果通常越好，但根据具体数据问题存在收益递减临界点。同时需考虑计算资源消耗。

极端随机树是随机森林的优秀替代方案，特别适用于噪声数据。由于其在分裂时采用随机选择策略，以牺牲部分方差减少为代价换取更高偏差，能有效降低对噪声重要特征的过拟合——这些特征在随机森林中往往会主导分裂过程。

## 梯度提升树

梯度提升树（GBDT）是提升算法的改进版本（提升算法通过序列化弱学习器对数据加权版本来实现）。与AdaBoost类似，GBDT基于梯度下降函数。该算法被证明是集成模型家族中最强大的成员之一，但其特点包括：估计方差增大、对数据噪声更敏感（可通过子采样缓解）、以及因非并行操作导致的高计算成本。

除深度学习外，梯度提升是发展最成熟的机器学习算法。自Jerome Friedman提出AdaBoost和初始梯度提升实现以来，已衍生出XGBoost、LightGBM和CatBoost等多种改进版本。

## LightGBM算法

高性能LightGBM算法（https://github.com/Microsoft/LightGBM）支持分布式计算并能快速处理海量数据，由微软团队在GitHub开源（相关论文：https://papers.nips.cc/paper/2017/hash/6449f44a102fde848669bdd9eb6b76fa-Abstract.html）。

与XGBoost类似，LightGBM基于决策树但采用不同策略：XGBoost采用逐层生长策略探索变量分裂，而LightGBM采用叶向生长策略——专注单次分裂并持续深化，从而更快实现数据拟合。算法结构上，XGBoost类似广度优先搜索（BFS），LightGBM则类似深度优先搜索（DFS）。两种方案的结合可有效降低估计方差。

LightGBM调参看似复杂（含百余参数，详见：https://github.com/Microsoft/LightGBM/blob/master/docs/Parameters.rst），但实际只需重点关注以下对结果影响最大的超参数：

- n_estimators（迭代次数）：10至10,000的整数

- learning_rate（学习率）：0.01至1.0的实数，通常取自对数均匀分布，代表梯度下降过程中组合权重的步长

- max_depth（最大深度）：1至16的整数，控制特征分裂最大次数。设为负值将允许最大可能分裂，但易导致过拟合

- num_leaves（叶节点数）：2至\( 2 \land \) max_depth的整数，限定单棵树的最大叶节点数

- min_data_in_leaf（叶最小数据量）：0至300的整数，设定叶节点包含数据点的最低数量

- min_gain_to_split：介于0到15之间的浮点数，用于设定树分裂时算法所需的最小增益。通过调整此参数可避免不必要的树分裂，从而降低过拟合风险（对应XGBoost中的gamma参数）。

- max_bin：32至512之间的整数，设定特征值分箱的最大数量。若该参数大于默认值255，可能导致过拟合风险增加。

- subsample：0.01到1.0之间的实数，表示训练时使用的样本比例。

- subsample_freq：0到10之间的整数，指定算法进行样本子采样的迭代频率。

注意：若设为0，算法将忽略subsample参数的任何设定值。由于该参数默认值为0，仅设置subsample参数不会生效。

- feature_fraction：0.1至1.0之间的实数，用于设定特征子采样的比例。特征子采样是通过增加随机性来对抗特征噪声和多重共线性的另一种方法。

- subsample_for_bin：30到样本总数之间的整数，设定构建直方图分箱时的抽样样本量。

- reg_lambda：0至100.0之间的实数，用于设置L2正则化。由于该参数对数值尺度比具体数值更敏感，通常采用对数均匀分布采样。

- reg_alpha：0至100.0之间的实数（通常采用对数均匀分布采样），用于设置L1正则化。

- scale_pos_weight：1e-6到500之间的实数（建议采用对数均匀分布采样），该参数通过加权正例（有效上采样或下采样）来平衡负例（固定权重为1）。

虽然LightGBM的超参数调优看似复杂，但实际上关键参数寥寥。Kaggle大师Kohei Ozaki在其博客中指出：在固定迭代次数和学习率时，仅少数参数影响显著（feature_fraction、num_leaves、subsample、reg_lambda、reg_alpha、min_data_in_leaf）。他基于此开发了Optuna快速调优流程（本章末尾将详述Optuna优化器）：https://medium.com/optuna/lightgbm-tuner-new-optuna-integration-for-hyperparameter-optimization-8b7095e99258

## XGBoost

XGBoost（https://github.com/dmlc/XGBoost）是极致梯度提升算法的开源实现。虽非Scikit-learn原生组件，但通过其封装接口可轻松融入Scikit-learn风格的数据流水线。

该算法在2015年Kaggle等数据科学竞赛中崭露头角。据开发者（陈天奇、Tong He和Carlos Guestrin）论文所述，当年29场Kaggle竞赛中17个冠军方案都采用了XGBoost（单独使用或模型集成）。尽管后来面临LightGBM和CatBoost等竞品的创新挑战，其在数据科学社区仍保持重要地位。

XGBoost兼具准确性与计算效率，是可扩展的分布式多核解决方案。通过对传统GBM算法的关键改进，它引领了新一代GBM算法的发展：

- 稀疏感知：能高效处理稀疏矩阵，既节省内存（无需稠密矩阵）又提升计算效率（对零值特殊处理）。

- 近似树学习（加权分位数草图），相比传统对可能分支切割的完整探索，能在更短时间内产生相似结果。

- 单机并行计算（在搜索最佳分割时使用多线程），以及类似的跨多台机器的分布式计算。

- 单机外存计算，利用称为列块的数据存储方案。该方案按列在磁盘上排列数据，从而通过以优化算法（基于列向量工作）预期的方式从磁盘提取数据来节省时间。

XGBoost还能有效处理缺失数据。基于标准决策树的其他树集成方法需要先用超出范围的值（如负数）填补缺失数据，才能构建适当的分支来处理缺失值。

关于XGBoost参数（https://xgboost.readthedocs.io/en/latest/parameter.html），我们重点介绍竞赛和项目中常见的几个关键参数：

- n_estimators：通常为10至5,000之间的整数。

- learning_rate：0.01到1.0之间的实数，建议从对数均匀分布中采样。

- min_child_weight：通常为1到10之间的整数。

- max_depth：通常为1到50之间的整数。

- max_delta_step：通常采样0到20之间的整数，表示允许每个叶节点输出的最大增量步长。

- subsample：0.1到1.0之间的实数，表示子采样样本比例。

- colsample_bytree：0.1到1.0之间的实数，表示每棵树的列采样比例。

- colsample_bylevel：0.1到1.0之间的实数，表示树中每层的列采样比例。

- reg_lambda：1e-9到100.0之间的实数，建议从对数均匀分布中采样。该参数控制L2正则化。

- reg_alpha：1e-9到100.0之间的实数，建议从对数均匀分布中采样。该参数控制L1正则化。

- gamma：指定树分割的最小损失减少量，该参数需要1e-9到0.5之间的实数，建议从对数均匀分布中采样。

- scale_pos_weight：介于1e-6到500.0之间的实数，建议从对数均匀分布中采样，代表正类样本的权重。

与LightGBM类似，XGBoost也有许多需要调优的超参数，因此前文针对LightGBM的所有考量同样适用于XGBoost。

## CatBoost

2017年7月，俄罗斯搜索引擎Yandex公开了另一种有趣的GBM算法CatBoost（https://catboost.ai/），其名称由"Category"和"Boosting"两个单词组合而成。该算法的强项在于通过混合使用独热编码和目标编码策略，能有效处理构成关系型数据库主要信息的类别型变量。目标编码通过为分类层级分配与当前问题相关的数值进行表达，更多细节可参阅第7章《表格竞赛建模》。

CatBoost采用的类别变量编码思路并非首创，而是一种在数据科学竞赛中已有应用的特征工程方法。目标编码（亦称似然编码、影响编码或均值编码）本质上是根据标签与目标变量的关联性将其转换为数值。对于回归问题，可基于该层级典型的目标均值进行转换；对于分类问题，则是给定该标签时目标分类的条件概率。虽然这种特征工程技巧看似简单巧妙，但会带来过拟合等副作用，因为预测变量中引入了目标变量的信息。

CatBoost拥有众多参数（参见https://catboost.ai/en/docs/references/training-parameters/），我们重点讨论其中八个最关键的参数：

- iterations：通常为10到1,000之间的整数，但可根据问题复杂度增大。

- depth：1到8之间的整数，数值越大通常需要更长的拟合时间且未必产生更好结果。

- learning_rate：0.01到1.0之间的实数值，建议从对数均匀分布中采样。

- random_strength：从1e-9到10.0范围对数线性采样的实数，用于指定划分得分的随机性强度。

- bagging_temperature：0.0到1.0之间的实数值，用于设置贝叶斯自助法。

- border_count：1到255之间的整数，表示数值特征的分割次数。

- leaf_reg：2到30之间的整数，代表L2正则化系数。

- scale_pos_weight：0.01到10.0之间的实数，表示正类样本的权重。

尽管CatBoost看似只是另一种GBM实现，但其诸多差异（通过独特的参数设置亦可体现）能在竞赛中提供重要帮助，无论是作为单一模型解决方案，还是作为集成模型的一部分。

## HistGradientBoosting

近期，Scikit-learn推出了受LightGBM分箱数据和直方图启发的新版梯度提升算法（参见Olivier Grisel在EuroPython的演讲：https://www.youtube.com/watch?v=urVUlKbQfQ4）。无论是作为分类器（HistGradientBoostingClassifier）还是回归器（HistGradientBoostingRegressor），该算法都可用于通过不同模型增强集成学习，且需要调优的超参数范围更为精简：

- learning_rate：介于0.01到1.0之间的实数，通常从对数均匀分布中采样。

- max_iter：可取值范围为10至10,000的整数。

- max_leaf_nodes：2到500之间的整数。该参数与max_depth存在交互作用，建议仅设置其中一个参数，另一个保留为None。

- max_depth：2到12之间的整数。

- min_samples_leaf：2到300之间的整数。

- 12_regularization：0.0到100.0之间的浮点数。

- max_bins：一个介于32到512之间的整数。尽管Scikit-learn的HistGradientBoosting与LightGBM或XG-Boost并无本质差异，但它为竞赛中的梯度提升模型实现提供了另一种思路。在集成多个预测结果时（例如混合堆叠法），由HistGradientBoosting构建的模型可能会产生独特贡献。

通过本节学习，您应当已熟悉最常见的机器学习算法（仅未涉及深度学习方案）及其需调优的核心超参数，这将助力您在Kaggle竞赛中构建卓越解决方案。掌握基础优化策略、可用算法及其关键参数仅是起点，下一节我们将深入探讨如何运用贝叶斯优化进行更高效的参数调优。

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_283.jpg?x=246&y=841&w=352&h=359&r=0"/>

<!-- Media -->

## 阿尔贝托·达内塞

https://www.kaggle.com/albedan

本章第二位访谈对象是阿尔贝托·达内塞，意大利信用卡与数字支付公司Nexi的数据科学主管。这位2015年加入平台的竞赛特级大师，其大部分金牌均以个人参赛者身份获得。

## 您最青睐哪类竞赛？原因何在？在技术方法层面，您在Kaggle的专长领域是什么？

我长期从事金融服务业结构化数据处理，自然更偏好此类竞赛。我享受对数据实质的切实把握，通过精巧的特征工程充分挖掘数据价值。

技术层面，我在传统机器学习库（尤其是梯度提升决策树）方面经验丰富，XGBoost、LightGBM、CatBoost等主流工具始终是我的首选。

## 您如何开展Kaggle竞赛？这与日常工作有何差异？

我会投入大量时间进行数据探索，厘清主办方试图通过机器学习解决的实际问题。与新手认知不同，我并不过度纠结于特定算法的"微调"——事实证明这策略行之有效！日常工作中数据理解同样关键，但还涉及Kaggle竞赛所没有的环节：

- 与业务部门协作定义待解决的机器学习业务问题

- 从内外部数据源获取所需数据

- 完成机器学习环节后，需规划部署方案并管理迭代更新

## 请分享您参与过最具挑战性的竞赛及攻克难关的洞见

TalkingData广告点击欺诈检测挑战赛令我受益匪浅，正是此役使我晋升特级大师。除了打击点击农场欺诈的趣味性，海量数据（超1亿标记行）迫使我优化特征工程效率，压缩计算时间以测试不同方案。这还促使我深入掌握滞后/领先特征（及其他窗口函数）的最佳应用方式，在传统机器学习问题中构建类时间序列模型。

## Kaggle对您的职业发展有何助益？

毋庸置疑！可验证的卓越竞赛成绩显著提升简历竞争力。2016年我被营销情报服务公司Cerved录用时，招聘主管深谙Kaggle价值——面试中能探讨真实项目案例极具优势。Kaggle无疑在我职业进阶中扮演了重要角色。

## 根据你的经验，新手Kaggle选手常会忽视什么？你现在掌握的哪些知识希望初学时就能知道？

我认为新手往往直接开始编码，比如fork公开内核后仅修改几行代码或参数。这在初期完全没问题！但必须投入足够时间不写代码，而是研究数据、理解问题本质。

## 你在过往比赛中犯过哪些错误？

不确定是否算错误，但我常偏好单人参赛：一方面这迫使你处理竞赛每个环节，并能自由安排时间。但我也非常享受在几次比赛中与队友合作：或许该更频繁组队，因为协作能学到很多。

# 有哪些特别推荐用于数据分析或机器学习的工具/库？

除常规工具外，我一直推崇data.table（从R版开始）：它值得更多认可！当需要本地处理海量数据时，这个包堪称神器。

# 参加比赛时最需要牢记的要点是什么？

先理解问题和数据：不要立刻开始编码！

## 贝叶斯优化(Bayesian optimization)

当实验空间有限时可采用网格搜索，但实践者通常会在随机搜索优化与贝叶斯优化(BO)技术间选择后者，后者需要更复杂的配置。

该方法最初由Snoek, J., Larochelle, H.和Adams, R. P.在论文《机器学习算法的实用贝叶斯优化》中提出（论文链接：http://export.arxiv.org/pdf/1206.2944）。其核心思想是优化代理函数而非真实目标函数（网格搜索和随机搜索都直接优化真实目标函数）。当梯度不可得、真实目标函数评估成本高（否则直接用随机搜索）、且搜索空间足够复杂嘈杂时采用此法。

贝叶斯搜索平衡探索与利用。初期随机探索以训练代理函数，随后基于该函数利用对预测器机制的近似认知进行采样，从而最小化成本函数。如名称所示，该方法运用先验概率在优化过程中做出更智能的采样决策，通过减少评估次数快速实现最小化。

贝叶斯优化通过采集函数评估观测价值。算法定义采集函数来量化探索任意给定点的效用，以此平衡探索与利用的矛盾。

通常贝叶斯优化由高斯过程驱动，当搜索空间响应平滑可预测时效果最佳。若搜索空间更复杂，可采用树算法（如随机森林）或树结构Parzen估计器(TPEs)。TPEs不直接建模参数集成功率，而是通过实验提供的连续近似值，估计定义最佳参数值的多元分布参数，从概率分布中采样获得最优参数集。

我们将首先分析基于高斯过程的Scikit-optimize和KerasTuner（前者也支持随机森林，后者支持多臂老虎机），然后研究主要基于TPE的Optuna（它也提供其他策略：https://optuna.readthedocs.io/en/stable/reference/samplers.html）。

虽然贝叶斯优化被视为超参数调优的前沿技术，但需注意：对于更复杂的参数空间，相比随机搜索方案，贝叶斯优化在时间和计算成本上并无优势。例如Google云机器学习引擎服务中，贝叶斯优化仅限最多16个参数的问题，更多参数时自动转为随机采样。

## 使用Scikit-optimize

Scikit-optimize（skopt）采用了与Scikit-learn相同的API接口开发，并大量使用了NumPy和SciPy函数库。该项目由Scikit-learn核心贡献者（如Gilles Louppe）参与创建。

该工具包基于高斯过程算法，维护状况良好，但由于Scikit-learn、NumPy或SciPy的版本更新，有时需要降级适配。例如在撰写本文时，若要在Kaggle Notebooks中正常运行，需按GitHub问题(#981)说明回退到旧版本依赖库。

该工具包API设计直观，便于二次开发用于自定义优化策略。其可视化功能尤为出色，通过plot_objective函数绘制优化过程结果，可帮助重新定义问题搜索空间并解释优化机制。我们的案例将参考以下Kaggle Notebook中的实现：

- https://www.kaggle.com/lucamassaron/tutorial-bayesian-optimization-with-lightgbm

- https://www.kaggle.com/lucamassaron/scikit-optimize-for-lightgbm

本文旨在演示如何快速解决类似"30 Days of \( {ML} \)"竞赛的优化问题——该赛事要求参赛者在30天内学习新技能并完成保险理赔金额预测（回归问题）。相关数据可通过https://www.kaggle.com/thirty-days-of-ml获取（所有资料均公开）。

若因未参赛无法访问原始数据，可使用此Kaggle数据集：https://www.kaggle.com/ lucamassaron/30-days-of-ml

以下代码将展示如何加载数据，并通过贝叶斯优化提升LightGBM模型性能。

## 首先加载依赖库：

---

# 导入核心库

import numpy as np

import pandas as pd

from time import time

import pprint

import joblib

from functools import partial

#因skopt冗长而抑制警告

import warnings

warnings.filterwarnings("ignore")

#分类器

import lightgbm as lgb

#模型选择

from sklearn.model_selection import KFold

#评估指标

from sklearn.metrics import mean_squared_error

from sklearn.metrics import make_scorer

#Skopt函数

from skopt import BayesSearchCV

from skopt.callbacks import DeadlineStopper, DeltaYStopper

from skopt.space import Real, Categorical, Integer

---

下一步是加载数据。除需将某些以字母为级别的分类特征转换为有序数值外，数据无需过多处理：

---

#加载数据

X = pd.read_csv("../input/30-days-of-ml/train.csv")

X_test = pd.read_csv("../input/30-days-of-ml/test.csv")

#将数据准备为表格矩阵

y = X.target

X = X.set_index('id').drop('target', axis='columns')

X_test = X_test.set_index('id')

#处理分类数据

分类列 = [列名 for 列名 in X.columns if 'cat' in 列名]

分类值 = np.unique(X[分类列].values)

分类字典 = dict(zip(分类值, range(len(分类值))))

X[分类列] = X[分类列].replace(分类字典).astype('category')

X_test[分类列] = X_test[分类列].replace(分类字典).

astype('category')

---

数据就绪后，我们定义一个报告函数供Scikit-optimize用于各类优化任务。该函数接收数据和优化器作为输入，还能处理回调函数——这些函数可执行诸如报告进度、基于达到特定搜索时间阈值或性能未提升（例如连续多次迭代未见改进）的提前终止、或在每次优化迭代后保存处理状态等操作：

---

#不同优化器的报告工具

def report_perf(optimizer, X, y, title="model", callbacks=None):

	"""

用于测量优化器时间和性能的封装函数

optimizer = sklearn或skopt优化器

X = 训练集

y = 目标变量

title = 实验的字符串标签

	"""

start = time(   )

if callbacks is not None:

optimizer.fit ( X, y, callback=callbacks )

else:

optimizer.fit(X, y)

d=pd.DataFrame(optimizer.cv_results_)

best_score = optimizer.best_score_

best_score_std = d.iloc[optimizer.best_index_].std_test_score

best_params = optimizer.best_params_

print((title + "耗时%.2f秒，检查候选参数：%d，最佳交叉验证

得分：%.3f" + u" ±"+" %.3f") %

(time(   ) - 开始时间,

len(optimizer.cv_results_['params']),

最佳得分,

最佳得分标准差))

print('最佳参数：')

pprint.pprint(最佳参数)

print(   )

return 最佳参数

---

现在我们需要准备评分函数（评估的基础）、验证策略（基于交叉验证）、模型及搜索空间。对于应采用均方根误差指标的评分函数，我们参考Scikit-learn的惯例——始终最小化函数（如需最大化则最小化其负值）。

make_scorer包装器可轻松实现此类操作：

---

#设置评分函数

scoring = make_scorer(partial(mean_squared_error, squared=False),

greater_is_better=False)

#设置验证策略

kf = KFold(n_splits=5, shuffle=True, random_state=0)

#设置基础回归器

reg = lgb.LGBMRegressor(boosting_type='gbdt',

metric='rmse',

objective='regression',

n_jobs=1,

verbose=-1,

random_state=0)

---

设置搜索空间需要使用Scikit-optimize的不同函数，如Real、Integer或Choice，每个函数从您定义的不同类型分布中采样（通常是均匀分布，但当您更关注参数的尺度效应而非具体值时，也会使用对数均匀分布）：

---

#设置搜索空间

search_spaces = \{

#提升学习率

'learning_rate': Real(0.01, 1.0, 'log-uniform'),

#待拟合的提升树数量

'n_estimators': Integer(30, 5000),

#基学习器的最大树叶数

'num_leaves': Integer(2, 512),

#基学习器的最大树深度

'max_depth': Integer(-1, 256),

#单个叶节点的最小数据量

'min_child_samples': Integer(1, 256),

#最大分箱桶数

'max_bin': Integer(100, 1000),

#训练实例的采样比例

'subsample': Real(0.01, 1.0, 'uniform'),

#子采样频率

'subsample_freq': Integer(0, 10),

#列采样比例

'colsample_bytree': Real(0.01, 1.0, 'uniform'),

#实例权重的最小和

'min_child_weight': Real(0.01, 10.0, 'uniform'),

#L2正则化

'reg_lambda': Real(1e-9, 100.0, 'log-uniform'),

##L1正则化

'reg_alpha': Real(1e-9, 100.0, 'log-uniform'),

\}

---

定义完成后：

- 您的交叉验证策略

- 您的评估指标

- 您的基础模型

- 您的超参数搜索空间 剩下的只需将它们输入优化函数BayesSearchCV。根据提供的CV方案，该函数将在搜索空间内寻找评分函数的最小值。您可以设置最大迭代次数、代理函数类型（高斯过程(GP)适用于大多数情况）以及确保可复现性的随机种子：

---

#将所有内容整合到贝叶斯优化器中

opt = BayesSearchCV(estimator=reg,

search_spaces=search_spaces,

scoring=scoring,

cv=kf,

n.iter=60. # 最大试验次数

n_jobs=-1, # 并行任务数

iid=False,

#若非独立同分布则优化CV分数

return_train_score=False,

refit=False,

#高斯过程(GP)

optimizer_kwargs=\{'base_estimator': 'GP'\},

#随机状态以确保可复现性

random_state=0)

---

此时，您可以使用之前定义的报告函数开始搜索。经过一段时间后，该函数将返回针对该问题的最佳参数。

---

#运行优化器

overdone_control = DeltaYStopper(delta=0.0001)

#当优化收益过小时停止

time_limit_control = DeadlineStopper(total_time=60 * 60 * 6)

#设置时间限制（6小时）

best_params = report_perf(opt, X, y,'LightGBM_regression',

callbacks=[overdone_control, time_limit_

control])

---

在本示例中，我们通过指定最大允许时间（6小时）来限制操作时长，之后停止并报告最佳结果。由于贝叶斯优化方法将超参数不同组合的探索与利用相结合，在任何时候停止都会返回当前找到的最佳解决方案（但不一定是可能的最佳方案）。这是因为采集函数会根据代理函数返回的预估性能及其不确定性区间，始终优先探索搜索空间中最有希望的区域。

## 定制贝叶斯优化搜索

Scikit-optimize提供的BayesSearchCV函数确实很方便，因为它自动封装并组织了超参数搜索的所有元素，但它也存在局限性。例如，在竞赛中你可能会发现以下功能很有用：

- 对每次搜索迭代有更多控制权，比如混合随机搜索和贝叶斯搜索

- 能够对算法应用早停机制

- 更灵活地定制验证策略

- 提前终止无效实验（例如，在获得单折交叉验证结果时立即评估性能，而非等待最终所有折的平均结果）

- 创建表现相似的超参数组合集群（例如，用于构建仅超参数不同的多个模型，以实现混合集成）

若能修改BayesSearchCV内部流程，这些任务都不算复杂。幸运的是，Scikit-optimize恰好提供了这种可能性。实际上，在BayesSearchCV及其他包装器背后，都有可作为独立部件使用的特定最小化函数：

- gp_minimize：使用高斯过程进行贝叶斯优化

- forest_minimize：使用随机森林或极端随机树进行贝叶斯优化

- gbrt_minimize：使用梯度提升进行贝叶斯优化

- dummy_minimize：仅随机搜索

接下来的示例将用自定义搜索函数修改先前搜索。新函数将支持训练过程中的早停机制，并在某折验证结果未达最优时终止实验。

您可以在Kaggle Notebook查看运行示例：https://www.kaggle.com/lucamassaron/hacking-bayesian-optimization

如前例所示，我们首先导入必要的包。

---

#导入核心库

导入 numpy 库（np）

导入 pandas 库（pd）

从 time 模块导入 time 函数

导入 pprint 模块

导入 joblib 库

从 functools 模块导入 partial 函数

#由于 skopt 的冗余输出，抑制警告信息

导入 warnings 模块

设置警告过滤器忽略警告

#分类器/回归器

从 xgboost 库导入 XGBRegressor 回归器

#模型选择

从 sklearn.model_selection 模块导入 KFold 和 StratifiedKFold

从 sklearn.model_selection 模块导入 cross_val_score 函数

从 sklearn.model_selection 模块导入 train_test_split 函数

#评估指标

从sklearn.metrics导入均方误差(mean_squared_error)

从sklearn.metrics导入创建评分器(make_scorer)

#Skopt函数库

从skopt导入贝叶斯搜索交叉验证(BayesSearchCV)

从skopt.callbacks导入截止停止器(DeadlineStopper)和增量停止器(DeltaYStopper)

从skopt.space导入实数域(Real)、分类域(Categorical)、整数域(Integer)

从skopt导入高斯过程最小化(gp_minimize)和森林最小化(forest_minimize)

从skopt导入梯度提升回归树最小化(gbrt_minimize)和虚拟最小化(dummy_minimize)

#将参数列表转换为命名参数的装饰器

从skopt.utils导入使用命名参数(use_named_args)

#数据处理

从sklearn.preprocessing导入序数编码器(OrdinalEncoder)

---

沿用之前的方法，我们从30天机器学习竞赛加载数据：

---

#加载数据

X_train = pd.read_csv("../input/30-days-of-ml/train.csv")

X_test = pd.read_csv("../input/30-days-of-ml/test.csv")

#将数据准备为表格矩阵

y_train = X_train.target

X_train = X_train.set_index('id').drop('target', axis='columns')

X_test = X_test.set_index('id')

#标识分类特征

categoricals = [item for item in X_train.columns if 'cat' in item]

#使用OrdinalEncoder处理分类数据

ordinal_encoder = OrdinalEncoder(   )

X_train[categoricals] = ordinal_encoder.fit_transform(X_train[categoricals])

X_test[categoricals] = ordinal_encoder.transform(X_test[categoricals])

---

现在我们已经为超参数搜索设置了所有必要元素，包括评分函数、验证策略、搜索空间以及待优化的机器学习模型。评分函数和验证策略后续将构成目标函数的核心要素，贝叶斯优化将致力于最小化该目标函数。

---

#设置评分函数

scoring = partial(mean_squared_error, squared=False)

#设置交叉验证策略

kf = KFold(n_splits=5, shuffle=True, random_state=0)

#设置搜索空间

space = [Real(0.01, 1.0, 'uniform', name='learning_rate'),

Integer(1, 8, name='max_depth'),

Real(0.1, 1.0, 'uniform', name='subsample'),

#每棵树的列采样比例

Real(0.1, 1.0, 'uniform', name='colsample_bytree'),

#L2正则化

Real(0, 100., 'uniform', name='reg_lambda'),

#L1正则化

Real(0, 100., 'uniform', name='reg_alpha'),

#实例权重最小和(海森矩阵)

Real(1, 30, 'uniform', name='min_child_weight')

	]

model = XGBRegressor(n_estimators=10_000,

booster='gbtree', random_state=0)

---

注意这次我们没有在搜索空间包含估计器数量(n_estimators参数)。而是在实例化模型时直接设定了较大值，因为我们预期会基于验证集提前停止模型。

下一步需要创建目标函数。该函数应仅接收待优化参数作为输入并返回评分结果。但目标函数还需纳入您刚准备的搜索所需元素。虽然可以在函数内部引用这些元素，但最佳实践是将它们纳入函数自身的内存空间。这样做有诸多优势：例如可使元素不可变，并能随目标函数一起传递(通过序列化或在多处理器层面分发搜索任务时)。您可以通过创建make函数来实现这一点——该函数接收这些元素，并返回修改后的目标函数。通过这种简单结构，您的目标函数将整合数据和模型等所有元素，您只需传入待测试参数即可。

现在开始编写这个函数。我们将在过程中暂停讨论相关要点：

<!-- Media -->

---

待最小化的目标函数

def 构建目标函数(model, X, y, space, cv, scoring, validation=0.2):

#该装饰器将带命名参数的目标函数

#自动转换为可接受列表参数的函数

#并自动完成参数转换

@use_named_args(space)

def 目标函数(**params):

model.set_params(**params)

print("\\n测试参数: ", params)

validation_scores = list(   )

for k, (train_index, test_index) in enumerate(kf.split(X, y)):

val_index = list(   )

train_examples = int(train_examples * (1 - validation))

train_index, val_index = (train_index[:train_examples],

train_index[train_examples:])

start_time = time(   )

model.fit(X.iloc[train_index,:], y[train_index],

---

<!-- Media -->

---

早停轮数=50,

验证集=[(X.iloc[val_index,:], y[val_index])],

日志输出=0

				)

结束时间 = time(   )

最佳迭代轮数 = model.best_iteration

测试集预测 = model.predict(X.iloc[test_index,:])

测试分数 = scoring(y[test_index], test_preds)

print(f"交叉验证折 \{k+1\} 均方根误差:\{test_score:0.5f\}-\{rounds\}

轮数 - 耗时 \{end_time-start_time:0.0f\} 秒")

验证分数列表.append(test_score)

---

在函数的第一部分，您只需创建一个目标函数，执行交叉验证并使用早停策略拟合数据。我们采用了激进的早停策略以节省时间，但如果您认为增加耐心轮数可能更适合您的问题，可以调整该参数。请注意，验证样本是从训练折的样本中依次抽取的（参见代码中train_index和val_index的定义方式），而保留折外样本（由kf交叉验证分割得到的test_index）用于最终验证。如果您希望避免在用于早停的数据上产生自适应过拟合，这一点至关重要。

在下一部分中，继续交叉验证循环并处理剩余待训练和测试的交叉验证折之前，您需要分析当前折在折外集上获得的结果：

---

if len ( history [ k ] ) >= 10 :

阈值 = np.percentile(history[k], q=25)

if 测试分数 > 阈值:

打印(f"提前终止表现不佳的折:

阈值为\{threshold:0.5f\}")

返回验证分数的平均值

历史记录[k].append(测试分数)

返回验证分数的平均值

返回目标函数

---

注意我们维护了一个全局字典history，用于记录截至目前每个折的实验结果。通过固定随机种子保证交叉验证可复现，使得不同实验间相同折的结果具有可比性。当当前折的结果低于历史迭代中其他折的表现（以底部四分位数为参考基准）时，将提前终止并返回已测试折的平均值。其原理在于：若某折结果不理想，整个交叉验证很可能也不理想。因此可中止当前参数搜索，转向更有潜力的参数组合。这种交叉验证早停机制能加速搜索过程，在更短时间内探索更多实验组合。

接下来通过make_objective函数，我们将模型、数据、搜索空间、验证策略和评分函数整合为目标函数。最终得到一个仅接收待优化参数并返回评分的函数，优化引擎将基于该评分决定后续实验方向：

---

目标函数 = make_objective(模型,

X_train, y_train,

空间=空间,

交叉验证=kf,

评分=scoring)

---

为控制优化过程并保存中间结果，我们准备了回调函数用于在每次迭代时记录实验参数及其结果。仅需这两类信息，优化引擎即可随时中断并从检查点恢复：

---

def 每步回调(res):

全局计数器

x0 = res.x_iters # 输入点列表

y0 = res.func_vals # 输入点评估值

print('最后评估: ', x0[-1],

' - 得分 ', y0[-1])

print('当前迭代: ', counter,

' - 最佳得分 ', res.fun,

' - 最佳参数: ', res.x)

# 保存检查点到磁盘

joblib.dump((x0, y0), 'checkpoint.pkl')

counter += 1

---

至此，我们已准备就绪。贝叶斯优化需要一些初始点才能正常工作。我们通过随机搜索（使用dummy_minimize函数）创建若干实验并保存结果：

---

counter = 0

history = \{i:list(   ) for i in range(5)\}

used_time = 0

gp_round = dummy_minimize(func=objective,

dimensions=space,

调用次数=30,

回调函数=[逐步执行],

随机种子=0)

---

随后我们可以调取已保存的实验数据，并打印出贝叶斯优化测试过的多组超参数序列及其结果。实际上，我们能在\( {x\theta } \)和\( {y\theta } \)列表中找到这些参数组及其对应结果：

---

x0, y0 = joblib.load('检查点.pkl')

打印(len(x0))

---

此时，我们甚至可以调整搜索空间、采集函数、调用次数或回调函数等设置，继续执行贝叶斯优化：

---

x0, y0 = joblib.load('检查点.pkl')

高斯过程轮次 = gp_minimize(函数=目标函数,

x0=x0, # x的已检测值

y0=y0, # x0的观测值

维度=空间,

采集函数='gp_hedge',

调用次数=30,

初始点数=0,

回调函数=[逐步执行],

random_state=0)

---

当我们确认无需继续调用优化函数时，即可输出基于输入和验证方案获得的最佳分数及最优超参数组合：

---

x0, y0 = joblib.load('checkpoint.pkl')

print(f"最佳分数: \{gp_round.fun:0.5f\}")

print("最优超参数：")

for sp, x in zip(gp_round.space, gp_round.x):

print(f"\{sp.name:25\} : \{x\}")

---

根据最优结果，我们可以重新训练模型用于竞赛。

现在掌握了参数集及其对应结果（x0和y0列表），我们还可以分析不同结果，将输出相似但参数组合相异的方案聚类。这有助于训练一组性能相近但优化策略多样的模型，是实现模型融合（blending）的理想场景——通过多个模型的平均预测来降低估计方差，从而提升公开和私有排行榜分数。

关于融合技术的详细讨论，请参阅第9章《集成方法：融合与堆叠解决方案》。

## 将贝叶斯优化拓展至神经架构搜索

转向深度学习领域，神经网络同样存在大量需要确定的超参数：

- 批大小

- 学习率

- 优化器类型及其内部参数

这些参数共同影响网络学习效果，微小的批大小或学习率差异都可能决定网络能否突破特定误差阈值。

尽管如此，这些学习参数并非深度神经网络（DNN）中唯一可优化的部分。网络的分层组织方式及其架构细节往往更具决定性。从技术角度而言，架构决定了DNN的表征能力——这意味着所选层结构将直接影响网络能否完整读取并处理数据中的全部信息。与传统机器学习算法有限的选择空间不同，DNN的架构组合近乎无限，唯一的制约因素在于你对神经网络组件的掌握程度与组合经验。

优秀深度学习实践者构建高性能DNN的通用准则主要基于：

- 采用预训练模型（需精通现有解决方案，如Hugging Face(https://huggingface.co/models)或GitHub上的资源）

- 研读前沿论文

- 借鉴同类型或往届Kaggle竞赛中的顶级Notebook方案

- 反复试错

- 创新思维与运气

Geoffrey Hinton教授在其著名课程中指出：采用贝叶斯优化等自动化方法可获得相当甚至更优的结果。该方法还能避免因海量超参数组合而陷入局部最优困境。

Geoffrey Hinton教授课程视频见：https://www.youtube.com/ watch?v=i0cKa0di_lo

课程幻灯片见：https://www.cs.toronto.edu/~hinton/coursera/lecture16/ lec16.pdf

如前所述，即便在最先进的AutoML系统中，当超参数过多时，随机优化可能在与贝叶斯优化相同时间内获得同等或更好效果。但DNN优化面临陡峭的搜索地形——许多参数是布尔型而非连续型，单个改动就可能戏剧性改变网络性能。经验表明随机优化不适用于Kaggle竞赛，因为：

- 时间与资源有限

- 需利用历史优化结果寻找更优解

贝叶斯优化在此场景堪称完美：可根据可用资源分阶段优化，通过多次迭代精调参数。由于DNN依赖GPU运算，除非配备多台高性能机器，否则难以实现并行调参。贝叶斯优化仅需单机即可顺序执行任务，且能基于历史实验数据规避无效参数组合——而随机优化除非动态调整搜索空间，否则总会遍历所有可能。

但贝叶斯优化也有缺陷：其代理函数基于历史试验构建，可能错误地将搜索聚焦于局部区域（而全局最优解可能在其他位置）。解决方案是进行大量实验，或交替使用随机搜索与贝叶斯优化——通过随机试验迫使模型重构更优的搜索路径。

本示例再次使用Kaggle"30 Days of ML"竞赛的回归任务数据。虽然基于TensorFlow实现，但稍作修改即可运行于PyTorch或MXNet等深度学习框架。

如之前所述，您可以在Kaggle上找到示例：https://www.kaggle.com/ lucamassaron/hacking-bayesian-optimization-for-dnns。

现在开始：

---

导入tensorflow库

---

导入TensorFlow包后，我们利用其Dataset函数创建一个可迭代对象，用于向神经网络批量输送数据：

---

定义数据框转数据集函数（支持乱序与批量设置）：

复制数据框副本

提取目标标签列

构建张量切片数据集

（含特征字典与标签）

若需乱序：

添加缓冲区乱序操作

设置批次大小

返回数据集对象

将LeakyReLU激活函数（α=0.2）

注册为可调用自定义对象

---

我们还将LeakyReLU激活函数设为模型自定义对象，支持通过字符串调用，无需直接使用函数。

我们开始编写一个函数，根据一组超参数创建深度神经网络模型：

---

def create_model(cat0_dim, cat1_dim, cat2_dim,

cat3_dim, cat4_dim, cat5_dim,

cat6_dim, cat7_dim, cat8_dim, cat9_dim,

layers, layer_1, layer_2, layer_3, layer_4, layer_5,

activation, dropout, batch_normalization, learning_rate,

**others):

dims = \{'cat0': cat0_dim, 'cat1': cat1_dim, 'cat2': cat2_dim,

'cat3': cat3_dim, 'cat4': cat4_dim, 'cat5': cat5_dim,

'cat6': cat6_dim, 'cat7': cat7_dim, 'cat8': cat8_dim,

'cat9': cat9_dim\}

vocab = \{h:X_train['cat4'].unique(   ).astype(int)

for h in ['cat0', 'cat1', 'cat2', 'cat3',

'cat4', 'cat5', 'cat6', 'cat7',

'cat8', 'cat9']\}

layers = [layer_1, layer_2, layer_3, layer_4, layer_5][:layers]

特征列 = list(   )

for 表头 in ['连续1', '连续2', '连续3', '连续4', '连续5',

'连续6','连续7', '连续8', '连续9', '连续10',

'连续11', '连续12', '连续13']:

特征列.append(tf.特征列.数值列(表头))

for 表头 in ['类别0', '类别1', '类别2', '类别3', '类别4', '类别5',

'类别6', '类别7', '类别8', '类别9']:

特征列.append(   )

tf.特征列.嵌入列(   )

tf.特征列.词汇表分类列(   )

表头, 词汇表=词汇[表头]),

维度=维度[表头]))

特征层 = tf.keras.layers.密集特征(特征列)

网络结构 = [特征层]

for 节点数 in 层数:

网络结构.append(   )

tf.keras.layers.Dense(节点数, activation=激活函数))

如果 batch_normalization 为 True:

网络结构.append(   )

tf.keras.layers.BatchNormalization(   ))

如果 dropout > 0 :

网络结构.append(tf.keras.layers.Dropout(dropout值))

模型 = tf.keras.Sequential(网络结构 +

[tf.keras.layers.Dense(1)])

模型.compile(optimizer=tf.keras.optimizers.Adam(   )

learning_rate=学习率),

loss= tf.keras.losses.MeanSquaredError(   ),

metrics=['均方误差'])

返回 模型

---

在内部，create_model函数中的代码会根据提供的输入自定义神经网络架构。例如，作为函数参数，您可以提供每个类别变量的嵌入维度，或定义网络中密集层的结构和数量。所有这些参数都与贝叶斯优化要探索的参数空间相关，因此创建模型的函数每个输入参数都应关联到搜索空间中定义的采样函数。您只需将采样函数按create_model函数预期的顺序放入列表：

---

#设置搜索空间

space = [Integer(1, 2, name='cat0_dim'),

Integer(1, 2, name='cat1_dim'),

Integer(1, 2, name='cat2_dim'),

Integer(1, 3, name='cat3_dim'),

Integer(1, 3, name='cat4_dim'),

Integer(1, 3, name='cat5_dim'),

Integer(1, 4, name='cat6_dim'),

Integer(1, 4, name='cat7_dim'),

Integer(1, 6, name='cat8_dim'),

Integer(1, 8, name='cat9_dim'),

Integer(1, 5, name='layers'),

Integer(2, 256, name='layer_1'),

Integer(2, 256, name='layer_2'),

Integer(2, 256, name='layer_3'),

Integer(2, 256, name='layer_4'),

Integer(2, 256, name='layer_5'),

Categorical(['relu', 'leaky-relu'], name='activation'),

Real(0.0, 0.5, 'uniform', name='dropout'),

Categorical([True, False], name='batch_normalization'),

Categorical([0.01, 0.005, 0.002, 0.001], name='learning_rate'),

Integer(256, 1024, name='batch_size')

							]

---

如前所述，现在您需要将与搜索相关的所有元素整合到一个目标函数中，该函数由包含基础搜索元素（如数据和交叉验证策略）的函数创建：

---

def make_objective(model_fn, X, space, cv, scoring, validation=0.2):

#此装饰器将带命名参数的目标函数

#转换为接受列表作为参数的函数，同时自动完成

#转换过程

@use_named_args(space)

def objective(**params):

print("\\n测试参数: ", params)

validation_scores = list(   )

for k, (train_index, test_index) in enumerate(kf.split(X)):

val_index = list(   )

train_examples = len(train_index)

train_examples = int(train_examples * (1 - validation))

train_index, val_index = (train_index[:train_examples],

train_index[train_examples:])

start_time = time(   )

model = model_fn(**params)

measure_to_monitor = 'val_mean_squared_error'

modality='min'

early_stopping = tf.keras.callbacks.EarlyStopping(   )

monitor=measure_to_monitor,

mode=modality,

patience=5,

verbose=0)

model_checkpoint = tf.keras.callbacks.ModelCheckpoint(   )

'best.model',

monitor=measure_to_monitor,

mode=modality,

仅保存最佳模型=True,

详细输出=0)

运行 = 模型.fit(数据集转换(   )

X_train.iloc[训练索引, :],

批次大小=参数['batch_size']),

验证数据=数据集转换(   )

X_train.iloc[验证索引, :],

批次大小=1024),

训练轮数=1_000,

回调函数=[模型检查点,

早停],

详细输出=0)

结束时间 = 时间(   )

最佳轮次 = np.argmin(   )

运行历史['验证均方误差']) + 1

模型 = tf.keras.models.加载模型('最佳模型')

shutil.rmtree('best.model')

测试预测值 = 模型.predict(转为数据集(   )

X.iloc[测试索引, :], 不打乱顺序=False,

批次大小=1024)).展平(   )

测试分数 = 评分函数(   )

X.iloc[测试索引, :]['目标值'],

测试预测值)

打印(f"交叉验证折数 \{k+1\} 均方根误差:\{测试分数:0.5f\} - \{轮次\}

轮次 - 耗时 \{结束时间-开始时间:0.0f\} 秒")

验证分数集.append(测试分数)

若历史记录[ k ]长度 >= 10:

阈值 = np.百分位数(历史记录[k], q=25)

若测试分数 > 阈值:

打印(f"低性能折数提前停止:

阈值为 \{阈值:0.5f\}")

返回 np.平均值(验证分数集)

历史记录[k].追加(测试分数)

返回 np.平均值(验证分数)

返回目标函数

---

下一步是提供一系列随机搜索运行（作为从搜索空间构建反馈的起点）并收集结果作为初始数据。随后可将其输入贝叶斯优化，并使用forest_minimize作为代理函数继续：

---

计数器 = 0

历史记录 = \{i:列表(   ) for i in 范围(5)\}

已用时间 = 0

高斯过程轮次 = 虚拟最小化(函数=目标函数,

维度=空间,

调用次数=10,

回调=[单步回调],

随机状态=0)

垃圾回收.收集(   )

初始参数, 初始结果 = 作业库.加载('检查点.pkl')

高斯过程轮次 = 高斯过程最小化(函数=目标函数,

初始参数=初始参数, # 已检测的x值

y0=y0, # x0的观测值

维度=空间,

调用次数=30,

初始点数=0,

回调函数=[单步回调],

随机种子=0)

垃圾回收(   )

---

请注意，在完成前十轮随机搜索后，我们采用随机森林算法作为代理函数继续搜索。相比高斯过程，这种方法能确保获得更优且更快的效果。与之前相同，在此过程中我们必须努力使优化在现有时间和资源条件下可行（例如通过设置较低的调用次数）。因此，我们可以通过保存优化状态、检查已获结果来分批进行搜索迭代，进而决定是继续优化还是终止流程，不再投入更多时间精力寻找更优解。

## 使用KerasTuner创建更轻量更快速的模型

若前文内容因复杂度令您困惑，KerasTuner能为您提供无需繁琐设置的快速优化方案。虽然其默认采用贝叶斯优化和高斯过程，但KerasTuner的创新理念在于超带宽优化（Hyperband optimization）。该技术利用赌博机方法确定最佳参数（参见http://web.eecs.umich.edu/~mosharaf/Readings/HyperBand.pdf），尤其适合优化地形不规则且不连续的神经网络——这类场景往往不适用于高斯过程。

请注意，您仍需构建通过输入超参数生成自定义网络的函数，KerasTuner只是大幅简化了操作流程。

让我们从头开始。Keras创始人François Chollet将KerasTuner（https://keras.io/keras_tuner/）定义为"面向Keras模型的灵活高效超参数调优工具"。

Chollet提出的KerasTuner使用方案包含简单步骤，基于现有Keras模型即可实施：

1. 将模型封装为以hp为首个参数的函数

2. 在函数起始处定义超参数

3. 用超参数替代DNN静态值

4. 根据给定的超参数编写复杂神经网络的建模代码。

5. 在构建网络过程中，如需可动态定义超参数。

现在我们将通过一个示例，探讨如何在Kaggle竞赛中运用这些步骤。目前KerasTuner已集成在Kaggle Notebook的预装工具栈中，因此无需额外安装。此外，TensorFlow插件也属于Notebook的预装包。若您未使用Kaggle Notebook但需要尝试KerasTuner，可通过以下命令轻松安装：

!pip install -U keras-tuner

!pip install -U tensorflow-addons

您可在此处查看已配置好的Kaggle Notebook示例：https://www.kaggle.com/lucamassaron/kerastuner-for-imdb/

第一步是导入必要的包（为某些命令创建快捷方式，如pad_sequences），并从Keras直接加载我们将使用的数据：

---

import numpy as np

import pandas as pd

import tensorflow as tf

from tensorflow import keras

import tensorflow_addons as tfa

from sklearn.model_selection import train_test_split

from tensorflow.keras.models import Sequential

from tensorflow.keras.layers import LeakyReLU

from tensorflow.keras.layers import Activation

从 tensorflow.keras.optimizers 导入 SGD（随机梯度下降）、Adam（自适应矩估计）优化器

从 tensorflow.keras.wrappers.scikit_learn 导入 KerasClassifier（Keras分类器包装器）

从 tensorflow.keras.callbacks 导入 EarlyStopping（早停法）、ModelCheckpoint（模型检查点）回调函数

pad_sequences = keras.preprocessing.sequence.pad_sequences（序列填充函数）

imdb = keras.datasets.imdb（训练数据，训练标签），

（测试数据，测试标签）= imdb.load_data（词汇量上限=10000）

训练数据，验证数据，训练标签，验证标签 = train_test_split（训练_

数据，训练标签，测试集比例=0.30，

随机打乱=True，随机种子=0）

---

本次使用的IMDb数据集（互联网电影资料库）可直接通过Keras包获取（https://keras.io/api/datasets/imdb/），该数据集具有以下特征：

- 包含25,000条来自IMDb的影评

- 每条影评均标注情感倾向（正面/负面）

- 目标类别均衡（因此准确率可作为评估指标）

- 每条影评被编码为单词索引（整数）列表

- 为便于处理，单词按总体词频进行索引

该数据集还曾成功应用于Kaggle词嵌入竞赛（https://www.kaggle.com/c/word2vec-nlp-tutorial/overview）。

本示例涉及自然语言处理。这类问题通常通过基于LSTM或GRU层的循环神经网络(RNN)解决。BERT、RoBERTa等基于Transformer的模型往往能取得更好效果——这些预训练模型依赖大规模语料库——但并非所有问题都如此，RNN仍可作为需要超越的强基线或神经模型集成中的有效补充。本例中所有单词已完成数字化索引，我们只需在现有索引基础上添加表示填充（便于统一文本至固定长度）、句首、未知词及未使用词的数字编码：

<!-- Media -->

---

#将单词映射为整型索引的字典

word_index = imdb.get_word_index(   )

#前几个索引为预留位

word_index = \{k:(v+3) for k,v in word_index.items(   )\}

word_index["<PAD>"] = 0

word_index["<START>"] = 1

word_index["<UNK>"] = 2 # 未知词

word_index["<UNUSED>"] = 3

reverse_word_index = dict([(value, key) for (key, value) in word_index.

items(   )])

def decode_review(text):

return ' '.join([reverse_word_index.get(i, '?') for i in text])

---

<!-- Media -->

下一步需创建自定义注意力层。注意力机制是Transformer模型的基础，也是近年神经语言处理领域最具创新性的思想之一。

关于此类层的工作原理，详见注意力机制的开创性论文：Vaswani, A. 等《Attention is all you need》，载于《神经信息处理系统进展》2017年(https://proceedings.neurips.cc/paper/2017/fil e/3f5ee243547dee91fbd053c1c4a845aa-Paper.pdf)。

注意力机制的核心思想易于理解。LSTM和GRU层会输出处理后的序列，但这些输出序列中的元素并非都对预测至关重要。不同于通过池化层对分层序列进行简单平均，实际上可采用加权平均（并在训练阶段学习合适的权重）。这种加权过程（注意力）能显著提升后续传递的结果。当然，可通过多层注意力（即多头注意力）使方法更精密，但本例中单层已足够——我们旨在证明对该问题使用注意力机制比直接平均或简单拼接所有结果更有效：

---

从tensorflow.keras.layers导入全连接层(Dense)、丢弃层(Dropout)

从tensorflow.keras.layers导入扁平化层(Flatten)、重复向量层(RepeatVector)、点积运算(dot)、逐元素乘法(multiply)

置换层(Permute)、Lambda层

K设为keras后端接口

定义注意力函数(attention):

#--- 注意力机制就是全部所需 ---#

_,_,单元数 = 获取层形状列表(layer.shape.as_list())

注意力权重 = 全连接层(1, 激活函数='tanh')(layer)

注意力权重 = 扁平化层()(注意力权重)

注意力权重 = 激活层('softmax')(注意力权重)

注意力权重 = 重复向量层(单元数)(注意力权重)

注意力权重 = 置换层([2,1])(注意力权重)

表征向量 = 逐元素乘法([layer, 注意力权重])

表征向量 = Lambda层(lambda函数: 沿轴求和张量(K.sum(x, axis=-2))

输出形状=(单元数,))(表征向量)

	#------------------------------------ #

返回表征向量

---

作为针对该问题的深度神经网络架构研究的进一步变体，我们还希望测试使用不同类型优化器的有效性，例如修正Adam（一种自适应学习率的Adam优化器；详见此文：https://lessw.medium.com/new-state-of-the-art-ai-optimizer-rectified-adam-radam-5d854730807b）或随机权重平均（SWA）。SWA是一种基于改进学习率调度策略对优化过程中遍历的权重进行平均的方法：若模型易出现过拟合或超调现象，SWA有助于逼近最优解，尤其被证明在自然语言处理问题中效果显著。

---

def get_optimizer(option=0, learning_rate=0.001):

if option==0:

return tf.keras.optimizers.Adam(learning_rate)

elif option==1:

return tf.keras.optimizers.SGD(learning_rate,

momentum=0.9, nesterov=True)

elif option==2:

return tfa.optimizers.RectifiedAdam(learning_rate)

elif option==3:

return tfa.optimizers.Lookahead(   )

tf.optimizers.Adam(learning_rate), sync_period=3)

elif option==4:

return tfa.optimizers.SWA(tf.optimizers.Adam(learning_rate))

elif option==5:

return tfa.optimizers.SWA(   )

tf.keras.optimizers.SGD(学习率,

动量=0.9, 内斯特洛夫=True))

else:

return tf.keras.optimizers.Adam(学习率)

---

定义完两个关键函数后，我们现在面临最重要的编码函数：该函数将根据参数提供不同的神经网络架构。我们并未编码所有希望连接到不同架构选择的参数；仅提供hp参数，它应包含我们想使用的所有可能参数，这些参数将由KerasTuner运行。除函数输入中的hp外，我们还固定了词汇表大小和填充长度（若实际长度较短则添加虚拟值，较长则截断短语）：

---

layers = keras.layers

models = keras.models

def 创建可调模型(hp, 词汇量=10000, 填充长度=256):

#实例化模型参数

嵌入维度 = hp.Int('embedding_size', 最小值=8,

最大值=512, 步长=8)

空间丢弃率 = hp.Float('spatial_dropout', 最小值=0,

最大值=0.5, 步长=0.05)

卷积层数 = hp.Int('conv_layers', 最小值=1,

最大值=5, 步长=1)

循环层数 = hp.Int('rnn_layers', 最小值=1,

max_value=5, step=1)

密集层数 = hp.Int('dense_layers', min_value=1,

max_value=3, step=1)

卷积过滤器 = hp.Int('conv_filters', min_value=32,

max_value=512, step=32)

卷积核 = hp.Int('conv_kernel', min_value=1,

max_value=8, step=1)

拼接丢弃率 = hp.Float('concat_dropout', min_value=0,

max_value=0.5, step=0.05)

密集丢弃率 = hp.Float('dense_dropout', min_value=0,

max_value=0.5, step=0.05)

---

在函数的第一部分，我们仅从hp参数中恢复所有设置，并明确每个参数的搜索空间范围。与目前所见解决方案不同，这部分工作是在模型函数内部而非外部完成的。

该函数继续使用从hp提取的参数定义不同网络层。某些情况下，参数会启用或禁用执行特定数据处理的网络部分。例如，我们在代码中插入了一个图分支（conv_filters和conv_kernel），该分支使用卷积层处理词序列——一维卷积在NLP问题中同样有效，因为它们能捕捉LSTM可能较难把握的局部词序和语义关系。

现在我们可以定义实际模型：

---

inputs = layers.Input(name='inputs',shape=[pad_length])

layer = layers.Embedding(vocab_size, embedding_size,

输入长度=填充长度)(输入)

层 = 空间丢弃层(spatial_dropout)(层)

循环卷积层次数:

当首次循环时:

卷积 = 一维卷积层(滤波器数=卷积过滤器,

卷积核尺寸=卷积核, 填充方式='有效',

核初始化器='he_uniform')(层)

否则:

卷积 = 一维卷积层(滤波器数=卷积过滤器,

卷积核尺寸=卷积核, 填充方式='有效',

核初始化器='he_uniform')(卷积)

平均池化卷积 = 全局平均池化层()(卷积)

最大池化卷积 = 全局最大池化层()(卷积)

表征列表 = 列表()

循环RNN层次数:

是否双向 = 超参选择(f'是否双向_\{层序号\}',

values=[0, 1])

use_lstm = hp.Choice(f'use_lstm_\{l\}', values=[0, 1])

units = hp.Int(f'units_\{l\}', min_value=8, max_value=512, step=8)

if use_lstm == 1 :

rnl = layers.LSTM

else:

rnl = layers.GRU

if use_bidirectional==1:

layer = layers.Bidirectional(rnl(units,

return_sequences=True))(layer)

else:

layer = rnl(units, return_sequences=True)(layer)

representations.append(attention(layer))

layer = layers.concatenate(representations + [avg_pool_conv,

max_pool_conv])

layer = layers.Dropout(concat_dropout)(layer)

for l in range(dense_layers):

dense_units = hp.Int(f'dense_units_\{l\}', min_value=8,

max_value=512, step=8)

layer = layers.Dense(dense_units)(layer)

layer = layers.LeakyReLU(   )(layer)

layer = layers.Dropout(dense_dropout)(layer)

layer = layers.Dense(1, name='out_layer')(layer)

outputs = layers.Activation('sigmoid')(layer)

model = models.Model(inputs=inputs, outputs=outputs)

---

我们首先定义输入层，并通过后续的嵌入层对其进行转换，该层将序列值编码为密集层。在此过程中使用了SpatialDropout1D进行随机丢弃正则化，该函数会随机丢弃输出矩阵的整列（标准丢弃法则是随机丢弃矩阵中的单个元素）。经过这些初始阶段后，我们将网络分为基于卷积（Conv1D）和基于循环层（GRU或LSTM）的两条处理路径。正是在循环层之后，我们应用了注意力层。最后，这两条路径的输出被合并，再经过几个密集层，到达最终的输出节点——由于需要表示0到1范围内的概率值，此处采用sigmoid激活函数。

模型定义完成后，我们在返回模型前设置学习参数并编译模型：

---

hp_learning_rate = hp.Choice('learning_rate',

values=[0.002, 0.001, 0.0005])

optimizer_type = hp.Choice('optimizer', values=list(range(6)))

optimizer = get_optimizer(option=optimizer_type,

learning_rate=hp_learning_rate)

model.compile(optimizer=optimizer,

loss='binary_crossentropy',

metrics=['acc'])

return model

---

请注意，我们使用的是Keras的函数式API而非顺序式API构建模型。实际上我们建议避免使用顺序式API——虽然它更易设置，但会严重限制架构的潜在可能性。

至此大部分工作已完成。根据实践经验，在我们使用KerasTuner完成多次优化后，更倾向于先构建非参数化模型：包含所有待测试的架构特性，并将网络中互斥部分设置为最复杂的解决方案。当生成函数设置完毕且模型运行正常后，例如可绘制其计算图并通过成功拟合测试样本验证。之后才开始向架构中插入参数化变量，并设置超参数(hp)定义。

根据我们的经验，直接开始构建参数化函数会耗费更多时间和调试成本。KerasTuner的核心思想是让您将深度神经网络视为模块化电路集合，并优化其中的数据流动。现在导入KerasTuner，首先设置调优器本身，然后开始搜索：

---

import keras_tuner as kt

tuner = kt.BayesianOptimization(hypermodel=create_tunable_model,

objective='val_acc',

max_trials=100,

num_initial_points=3,

directory='storage',

project_name='imdb',

seed=42)

tuner.search(train_data, train_labels,

训练轮数=30,

批大小=64,

验证数据=(验证集数据, 验证集标签),

打乱顺序=True,

日志显示=2,

回调函数 = [早停法('验证集准确率',

耐心值=3,

\[\text{restore_best_weights=True)]}\]

)

---

作为调优器，我们选择贝叶斯优化器，但您也可以尝试Hyperband调优器(https://keras.io/api/keras_tuner/tuners/hyperband/)并检查它是否更适合您的问题。我们将模型函数提供给hypermodel参数。然后，我们使用字符串或函数设置优化目标、最大试验次数（如果无需继续，KerasTuner会提前停止）以及初始随机试验次数——越多越好——以便为贝叶斯过程提供信息。早停法是DNN建模中标准且高效的做法，您绝对不能忽视。最后但同样重要的是，我们设置保存搜索结果的目录和用于优化步骤可复现性的种子数。

搜索阶段像标准Keras模型训练一样运行，并且——这一点非常重要——它接受回调函数。因此，您可以轻松地为模型添加早停法。在这种情况下，给定的epoch数应被视为最大epoch数。您可能还想优化批大小，我们在示例中未进行此操作。这仍需要一些额外工作，但您可以通过阅读这个GitHub已关闭问题了解实现方法：https://github.com/keras-team/keras-tuner/issues/122。

优化完成后，您可以提取最佳参数并保存最佳模型，无需重新训练：

---

最佳超参 = 调优器.get_best_hyperparameters(   )[0]

模型 = 调优器.hypermodel.build(最佳超参)

打印(最佳超参.values)

模型.summary(   )

模型.save("最佳模型.h5")

---

本示例中，KerasTuner找到的解决方案使用：

- 更大的嵌入层

- 仅使用普通GRU和LSTM层（非双向层）

- 堆叠多个一维卷积层（Conv1D）

- 更多且更密集的全连接层

有趣的是，该解决方案不仅比我们之前基于直觉和问题经验的尝试更有效，而且更轻量、更快速。Chollet本人建议使用KerasTuner不仅能提升DNN性能，还能将其压缩至更易管理的规模——这在编程竞赛中可能成为制胜关键。这使您能在比赛主办方提供的有限推理时间内，整合更多协同工作的模型。

如需查看更多KerasTuner应用实例，François Chollet还为Kaggle竞赛创建了一系列Notebook，用以展示其优化器的工作原理与功能：

- https://www.kaggle.com/fchollet/keras-kerastuner-best-practices 数字识别器数据集

- https://www.kaggle.com/fchollet/titanic-keras-kerastuner-best-practices 泰坦尼克号数据集

- https://www.kaggle.com/fchollet/moa-keras-kerastuner-best-practices 作用机制(MoA)预测竞赛

## Optuna中的TPE方法

我们将通过另一个有趣工具和方法来完成贝叶斯优化的概述。如前所述，Scikit-optimize使用高斯过程（及树算法）直接建模代理函数和采集函数。

回顾这些概念：代理函数帮助优化过程模拟尝试某组超参数时的潜在性能结果。它基于先前的实验及其结果构建，本质上是用于预测特定机器学习算法在特定问题上表现的预测模型。向代理函数输入任何参数组合，都能获得预期性能输出——这种机制既直观又可灵活调整。

采集函数则指出应测试哪些超参数组合，以增强代理函数对算法性能的预测能力。它还能验证我们是否真的能基于代理函数的预测达到顶尖性能。这两个目标分别对应贝叶斯优化中的探索阶段（运行实验）和开发阶段（测试性能）。而基于TPE的优化器通过估算参数值的成功概率来解决问题，即通过连续优化对参数本身建立成功分布模型，为更优值组合赋予更高概率。

该方法通过分布将超参数划分为优/劣两组，这些分布取代了贝叶斯优化中代理函数和采集函数的角色——因为它们能指示应在何处采样以获得更好性能，或探索存在不确定性的区域。

要了解TPE的技术细节，我们推荐阅读Bergstra, J.等人的《超参数优化算法》（神经信息处理系统进展24卷，2011年：https://proceedings.neurips.cc/paper/2011/file/86e8f7ab32cfd12577bc2619bc635690-Paper.pdf）。

因此，TPE既能建模搜索空间，又能通过从调整后的参数概率分布中采样，为算法推荐下一步尝试方向。

长期以来，Hyperopt是那些倾向于使用TPE而非基于高斯过程的贝叶斯优化者的选择。然而2018年10月，Optuna作为开源工具问世，凭借其多功能性（可即装即用于神经网络甚至集成学习）、速度以及相较于先前优化器更高的寻优效率，迅速成为Kaggle竞赛选手的首选。

本节将展示如何轻松建立搜索流程——在Optuna术语中称为"研究"。您只需编写一个目标函数：该函数接收Optuna待测试参数作为输入，并返回评估结果。验证环节及其他算法细节可直接在目标函数内处理，亦可引用函数外部的变量（包括全局变量和局部变量）。Optuna还支持剪枝功能，即当特定实验效果不佳时发出信号，使Optuna能中止并放弃该次尝试。Optuna提供了一系列触发此回调的函数（参见https://optuna.readthedocs.io/en/stable/reference/integration.html）；此后算法将高效运行所有流程，显著缩短优化所需时间。

下个示例将完整呈现这些功能。我们继续针对30 Days of \( {ML} \)竞赛进行优化，本次重点探究XGBoost在该赛事中的最佳参数配置。

本示例的Notebook详见：https://www.kaggle.com/lucamassaron/optuna-bayesian-optimization

第一步照例加载库与数据：

---

import pandas as pd

import numpy as np

from sklearn import preprocessing

from sklearn.metrics import mean_squared_error

from sklearn.model_selection import train_test_split

from sklearn.preprocessing import OrdinalEncoder

from xgboost import XGBRegressor

import optuna

from optuna.integration import XGBoostPruningCallback

#加载数据

X_train = pd.read_csv("../input/30-days-of-ml/train.csv").iloc[:100_000,

				:]

X_test = pd.read_csv("../input/30-days-of-ml/test.csv")

#将数据准备为表格矩阵

y_train = X_train.target

X_train = X_train.set_index('id').drop('target', axis='columns')

X_test = X_test.set_index('id')

#标识分类特征

categoricals = [item for item in X_train.columns if 'cat' in item]

#使用OrdinalEncoder处理分类数据

ordinal_encoder = OrdinalEncoder(   )

X_train[categoricals] = ordinal_encoder.fit_transform(X_

train[categoricals])

X_test[categoricals] = ordinal_encoder.transform(X_test[categoricals])

---

使用Optuna时，只需定义包含模型、交叉验证逻辑、评估指标和搜索空间的目标函数。

自然地，对于数据可以引用函数外部的对象，这使得函数构建更加简单。与KerasTuner类似，这里需要一个基于Optuna类的特殊输入参数：

---

def objective(trial):

params = \{

'learning_rate': trial.suggest_float("learning_rate",

0.01, 1.0, log=True),

'reg_lambda': trial.suggest_loguniform("reg_lambda",

																														1e-9,100.0),

'reg_alpha': trial.suggest_loguniform("reg_alpha",

																														1e-9,100.0),

'subsample': trial.suggest_float("subsample", 0.1, 1.0),

'colsample_bytree': trial.suggest_float(   )

"colsample_bytree", 0.1, 1.0),

'max_depth': trial.suggest_int("max_depth", 1, 7),

'min_child_weight': trial.suggest_int("min_child_weight",

																														1, 7),

'gamma': trial.suggest_float("gamma", 0.1, 1.0, step=0.1)

		\}

model = XGBRegressor(   )

random_state=0,

tree_method="gpu_hist",

predictor="gpu_predictor",

n_estimators=10_000,

**params

		)

model.fit(x, y, early_stopping_rounds=300,

eval_set=[(x_val, y_val)], verbose=1000,

callbacks=[XGBoostPruningCallback(trial, 'validation_0-rmse')])

preds = model.predict(x_test)

rmse = mean_squared_error(y_test, preds, squared=False)

return rmse

---

本示例出于性能考虑，不采用交叉验证，而是使用固定数据集分别进行训练、验证（早停）和测试。本例使用GPU运算，并对可用数据进行了子集划分，以便在合理时间内完成60次试验。若无需使用GPU，只需从XGBRegressor实例化中移除tree_method和predictor参数。另请注意我们在fit方法中设置回调函数，以便向Optuna反馈模型表现，使优化器能提前终止表现不佳的实验，为其他尝试腾出空间。

---

x, x_val, y, y_val = train_test_split(X_train, y_train, random_state=0,

test_size=0.2)

\( x,x \) _____test, \( y,y \) _____test = train_test_split( \( x,y \) ,random_state=0,test_size=0.25)

study = optuna.create_study(direction="minimize")

study.optimize(objective, n_trials=100)

---

另一个显著特点是可根据问题类型选择最小化或最大化优化（Scikit-optimize仅支持最小化问题）。

---

print(study.best_value)

print(study.best_params)

---

运行结束时，只需打印或导出优化得到的最佳测试性能及最优参数即可。

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_323.jpg?x=241&y=1323&w=360&h=367&r=0"/>

<!-- Media -->

## 鲁奇·巴蒂亚

https://www.kaggle.com/ruchi798

作为本章的总结，让我们来看最后一位访谈对象。这次我们采访的是数据集与笔记本领域的大师级人物鲁奇·巴蒂亚。她目前是卡内基梅隆大学研究生、OpenMined数据科学家，同时担任惠普\( \mathrm{Z} \)项目的数据科学全球大使。

## 你最喜欢哪类竞赛？为什么？在技术方法和解题思路上，你在Kaggle的专长是什么？

我最钟爱自然语言处理（NLP）和分析类竞赛。多语言能力深刻影响了我对自然语言处理的研究方向。至于分析类竞赛，我享受从复杂数据中提炼洞见，并用数据支撑问题答案的过程。Kaggle每项竞赛都独具特色，需要不同技术手段。我主要采用数据驱动的算法选择策略，没有固定偏好。

## 你如何着手Kaggle竞赛？这与日常工作有何不同？

新竞赛发布后，我首先会深度理解问题陈述。有时问题会超出我们熟悉的领域，因此在开展探索性数据分析（EDA）前必须确保充分理解。进行EDA时，我的目标是掌握数据分布规律，重点了解现有数据特征。这个过程常会发现某些规律，我们需要努力理解这些规律，并对异常值形成假设。

接着我会研究竞赛评估指标，然后建立无数据泄露的交叉验证策略。之后选择基线模型进行首次提交。若本地验证与竞赛排行榜相关性不理想，我会持续迭代直至找出差异原因并解决。

随后逐步优化建模方法。此外，通过调整参数和尝试新实验来寻找最优方案（整个过程需防范过拟合）。最后几周进行模型集成并测试方案的鲁棒性。

至于非Kaggle项目，我主要时间花在数据采集、清洗和提取有效信息上。

## Kaggle对你的职业发展有帮助吗？具体体现在？

Kaggle极大加速了我的职业发展。它不仅帮我找到对数据科学的热情，更激励我持续做出实质性贡献。这个平台能让我们便捷地进行海量数据实验，并向全球展示成果。此外，作品易于传播，可以触达更广泛受众。

我将多数Kaggle作品纳入作品集，展现迄今完成的工作多样性。Kaggle竞赛旨在解决新颖的现实问题，我认为雇主看重这种问题解决能力。我还整理了大量数据集，突显处理原始数据的敏锐度。这些项目帮我获得了多个工作机会。

## 据你观察，新手常忽视哪些要点？你现在掌握了哪些希望初学时就知道的经验？

我发现许多新手因竞赛排名不如预期而气馁。经过数周数月努力后，我理解他们可能过早放弃，但赢得Kaggle竞赛本非易事。参赛者教育背景和工作经验各异，勇于尝试才是关键。我们应关注自身成长，看看自己走了多远。

## 有哪些特别推荐的数据分析或机器学习工具/库？

全面的探索性数据分析配合可视化能帮助我们发现改进方法的数据趋势。因此我推荐Seaborn（用于EDA）和TensorBoard（用于机器学习流程可视化），偶尔也会使用Tableau。我相信可视化能有效揭示数据内涵。

## 参加比赛时最需要牢记或做到的关键事项是什么？

我认为参赛者应当做好深入剖析赛题并开展研究的准备。Kaggle竞赛尤其具有挑战性，往往能助力解决现实问题。保持积极心态至关重要，切勿轻言放弃。这类竞赛正是学习成长的绝佳机会！

## 本章小结

本章详细探讨了通过超参数优化提升模型性能及排行榜得分的方法。我们首先解析了Scikit-learn的网格搜索、随机搜索等代码功能，以及新一代减半算法。

接着深入贝叶斯优化领域，依次探究了Scikit-optimize、KerasTuner及Optuna工具。我们重点讨论了高斯过程对代理函数的直接建模及其优化技巧，因为这能带来更强的直觉判断和定制化解决方案。值得注意的是，Optuna因其在Kaggle Notebook限定时间内快速收敛至最优参数的特性，已成为表格类竞赛和深度神经网络竞赛的金标准。但若想在竞争中脱颖而出，仍需尝试其他优化器的解决方案。

下一章将探讨提升Kaggle竞赛表现的另一种方法：模型集成。通过解析平均法、混合法和堆叠法的原理，我们将展示如何突破单纯调参的局限，实现更优结果。

## 加入本书Discord社区

欢迎加入本书Discord工作区，每月参与作者问答专场：

https://packt.link/KaggleDiscord

##

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_327.jpg?x=241&y=308&w=178&h=241&r=0"/>

<!-- Media -->

混合与堆叠解决方案的模型集成

初涉Kaggle竞赛便会发现，仅凭单一精妙模型难以取胜，必须集成多个模型。随之而来的问题是：如何构建有效集成？现存指南寥寥，更多经验源自Kaggle社区而非学术论文。

关键在于，虽然模型集成是Kaggle夺冠法宝，但在实际应用中却意味着复杂度高、可维护性差、难以复现及隐性技术成本。排行榜上那点提升对现实场景往往意义不大，因为成本远超收益。但这不意味着集成技术全无实用价值——通过有限形式（如融合多个异构模型）仍能高效解决诸多数据科学问题。

Kaggle中的集成不仅是提升预测性能的手段，更是团队协作策略。整合队员各自成果往往产生1+1>2的效果，同时能结构化地引导团队向明确目标迈进。考虑到队员身处不同时区、面临不同约束（如工作时间、学业考试等），结对编程等协作方式显然不现实。竞赛团队既无必要也难以实现全员任务同步，更何况队员技能水平参差不齐。

共享的集成策略使队员能按自身节奏工作，同时为团队成功贡献力量。因此，基于预测多样性的集成技术反而能将差异化技能转化为优势。

本章将从随机森林、梯度提升等算法中已嵌入的集成技术讲起，逐步扩展到多模型平均法、混合法与堆叠法。我们将提供理论指导、实践案例及代码模板，助你在Kaggle构建自己的解决方案。

本章将涵盖以下主题：

- 集成算法简要介绍

- 将模型平均集成

- 使用元模型混合模型

- 堆叠模型

- 构建复杂的堆叠与混合解决方案

在开始本章阅读和实践前，我们必须推荐一个对Kaggle竞赛参与者极具价值的集成学习指南：由Triskelion（亨德里克·雅各布·范维恩）与合著者（黎阮德达、阿曼多·塞尼尼）2015年发表的博客文章。原载于mlwave博客（现已关闭）的《Kaggle集成指南》，可通过https://usermanual.wiki/Document/Kaggle20ensembling20gui de.685545114.pdf获取。该文章系统整理了当时Kaggle论坛中关于集成学习的显性与隐性知识。

## 集成算法简论

模型集成优于单一模型的理念源远流长，可追溯至维多利亚时代的弗朗西斯·高尔顿爵士。他发现县集市上估算牛体重时，采集众人粗略估计的平均值比专家精心计算的单一估值更准确。1996年，里奥·布雷曼通过提出bagging技术（即"自助聚合"方法）将多模型组合提升预测力的理念形式化，这后来催生了更强大的随机森林算法。此后梯度提升和堆叠等集成技术相继问世，构成了当今完整的集成方法体系。

以下文献可追溯这些集成算法的起源：

- 随机森林：参阅布雷曼《Bagging predictors》（《机器学习》24.2期-1996）

- 提升算法细节：参考弗罗因德与沙皮尔《新提升算法实验》（ICML 1996），及弗里德曼《梯度提升机：贪婪函数逼近》（《统计年鉴》2001）

- 堆叠技术：详见丁与威滕《堆叠Bagged与Dagged模型》（1997）的技术初稿

Kaggle早期竞赛直接沿用分类回归中的bagging和随机森林策略，通过多预测结果平均形成基础集成技术。这种"平均法"从11年前的首届Kaggle竞赛乃至更早的Netflix竞赛中崭露头角，不同模型结果的平均策略占据主导。其成功为后续赛事树立标杆，至今仍是提升排行榜分数的有效手段。

随着赛题复杂度提升和竞争白热化，计算量更大的堆叠技术应运而生。正如随机森林启发预测平均，提升算法深刻影响了堆叠方法。梯度提升通过序列化决策树建模前序迭代未捕捉的数据特征，类似地，堆叠集成通过逐层处理前序模型结果来提升预测性能。

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_330.jpg?x=245&y=235&w=355&h=358&r=0"/>

<!-- Media -->

## 罗伯·穆拉专访

https://www.kaggle.com/robikscube

这位竞赛/笔记/讨论三料大师，Biocore LLC高级数据科学家，向我们分享了他的集成学习见解与Kaggle实战经验。

## 您最青睐哪类竞赛？从技术方法论角度，您在Kaggle的专长领域是什么？

我最青睐的比赛类型是那些涉及独特数据集、需要融合多种建模方法创新解决方案的竞赛。当比赛不仅要求训练大型模型，更需要深入理解数据并运用针对任务特性设计的架构时，我会格外享受。我不局限于任何特定方法——初入Kaggle时主要使用梯度提升模型，但为保持近年竞争力，我已拓展了深度学习、计算机视觉、自然语言处理和优化算法等领域的知识储备。最吸引我的赛事往往需要综合运用多项技术。

## 你如何规划Kaggle竞赛策略？与日常工作有何不同？

我的Kaggle竞赛方法论与工作项目存在共通之处：首先是数据理解。现实项目中需自行定义问题并制定评估指标，而Kaggle已提供这些要素。关键在于把握数据与指标的关联性，进而开发验证最优建模技术。最大差异在于最终阶段的模型集成与调优——现实中往往无需复杂集成，因为计算成本与性能提升可能不成正比。

## 请分享最具挑战性的参赛经历及破局思路

NFL头盔撞击检测比赛令我倍感挑战，这涉及我毫无经验的视频数据领域，需要研读相关论文并采用两阶段解决方案。另一场室内导航定位竞赛同样棘手，它要求建模、优化与深度数据理解，虽未取得佳绩却让我获益良多。

## Kaggle是否助力了你的职业发展？

当然。Kaggle极大提升了我在数据科学领域的知名度，拓展了新技术认知边界，更让我结识众多杰出同行，共同促进机器学习能力的精进。

我们团队在NFL头盔检测赛中荣获亚军，此前的系列参赛经历最终助我获得现职——赛事主办方主动向我抛出了橄榄枝。

## 新手常犯哪些疏漏？你希望初学时明白什么？

新人常过度关注模型集成与超参调优，但这些应在构建优质基模型后才具意义。深刻理解竞赛评估指标同样关键——许多选手忽视了针对指标优化方案的重要性。

## 你曾犯过哪些竞赛错误？

教训颇多：从过拟合模型到徒劳无功的尝试。但这些恰恰是必要的成长代价——特定比赛的失利往往铸就后续赛事的成功。

## 推荐哪些数据分析/机器学习工具？

探索性分析推荐掌握NumPy、Pandas及Matplotlib等可视化库。建模需精通Scikit-learn的交叉验证方案，XGBoost/LightGBM等基准模型必不可少。深度学习领域则应掌握TensorFlow/Keras或PyTorch任一主流框架。

## 模型平均集成技术

为更好阐述平均集成技术，让我们回顾Leo Breiman提出的所有集成策略。他的研究是集成方法的里程碑，其发现在众多领域仍具实用价值。Breiman探索这些可能性，旨在解决决策树等强模型容易过拟合训练数据导致的误差方差问题。

从概念上讲，他发现集成效果取决于三个要素：如何处理训练样本的抽样、如何构建模型，以及最终如何组合所获得的不同模型。

关于抽样方法，经过测试发现主要有以下几种：

- 粘贴法（Pasting）：通过无放回抽样从数据行中选取子样本构建多个模型

- 装袋法（Bagging）：通过有放回的自助抽样随机选取样本构建多个模型

- 随机子空间法：通过无放回抽样从特征列（数据列）中选取子样本构建多个模型

- 随机补丁法：类似装袋法，但在选择每个模型时还会像随机子空间法那样对特征进行抽样

采用抽样而非相同数据的原因是：通过对样本和特征进行子抽样，我们创建的模型都能解决同一问题却又彼此不同。这种差异性也体现在每个模型对样本的过拟合方式上——我们希望所有模型以相同方式捕捉数据中有用且可泛化的信息，而以不同方式处理对预测无用的噪声。因此，建模的差异性会减少预测的波动，因为误差往往会相互抵消。

既然这种差异性如此有用，下一步就不应仅修改模型学习的数据，还应调整模型本身。我们有两种主要建模方法：

- 同类型模型集成

- 异质模型集成

有趣的是，当集成模型的预测能力差异过大时，无论采用何种集成方式都收效甚微。关键在于：只有当组合的模型能正确预测同类结果时，才能在平均其错误预测时平滑误差。若集成性能悬殊的模型，最终效果将适得其反——不仅无法平滑错误预测，还会削弱正确预测。这是平均法的重要局限：它只能整合预测能力相近的不同模型（例如因使用不同样本和特征训练而产生的模型）。以线性回归和\( k \)近邻算法为例，二者建模和捕捉数据信号的方式截然不同，凭借各自核心的（独特）函数形式，这些算法能从数据中提取不同的预测细节，在特定预测任务上表现更优，但采用平均法时无法真正发挥这种优势。相比之下，堆叠法（stacking）能有效利用算法捕捉信号的不同方式，因为它可以汲取每个算法的最佳结果。

基于此，我们可以总结出有效的平均法集成（对多个模型结果取平均）应满足：

- 使用不同训练样本构建的模型

- 使用不同特征子样本构建的模型

- 由预测能力相近的模型组成

从技术上讲，这意味着各模型的预测应尽可能不相关，同时在预测任务上保持相同精度水平。

在探讨了集成多个机器学习模型的优势与局限后，我们现在将深入技术细节。平均化多个分类或回归模型有三种方法：

- 多数表决法，采用多个模型中最频繁出现的分类结果（仅适用于分类模型）

- 对数值或概率取平均值

- 采用加权平均数值或概率

接下来几节中，我们将结合Kaggle竞赛场景详细讨论每种方法。

## 多数表决法

通过改变集成模型中使用的样本、特征和模型来生成不同模型（若它们具有前文讨论过的可比预测能力），虽然需要一定计算资源，但无需构建与单模型迥异的数据处理流程。该流程只需收集不同的测试预测结果，并记录所用模型、训练时的样本/特征采样方式、超参数设置及交叉验证表现。

若竞赛要求预测类别，可采用多数表决法：即对每个预测结果选取模型最常预测的类别。这适用于二分类和多分类场景，其前提是模型虽偶有错误但多数情况下判断正确。多数表决法作为"纠错机制"，能过滤噪声保留有效信号。

首个简单示例将演示多数表决原理。我们先用Scikit-learn的make_classification函数生成类Madelon数据集。

原始Madelon是人工数据集，其数据点聚集于高维超立方体顶点并随机标注。该数据集包含若干有效特征，混杂无关及重复特征（制造特征间多重共线性），并注入随机噪声。由SVM算法创始人之一Isabelle Guyon为NIPS 2003特征选择挑战赛设计，现已成为竞赛用复杂人工数据集的典范，甚至启发多个Kaggle赛事：https://www.kaggle.com/c/overfitting 及较新的 https://www.kaggle.com/c/dont-overfit-ii。

本章将使用这个复现的Madelon数据集作为集成技术测试基准：

---

from sklearn.datasets import make_classification

from sklearn.model_selection import train_test_split

X, y = make_classification(n_samples=5000, n_features=50,

n_informative=10,

n_redundant=25, n_repeated=15,

每类簇数=5，

翻转比例=0.05，类别间隔=0.5，

随机种子=0）

X_train, X_test, y_train, y_test = 训练测试分割(X, y,

测试集比例=0.33，随机种子=0）

---

将数据划分为训练集和测试集后，我们开始实例化学习算法。仅使用三种基础算法进行演示：支持向量机（SVMs）、随机森林以及\( k \)近邻分类器，均采用默认超参数。可尝试调整参数或增加算法数量：

---

from sklearn.svm import SVC

from sklearn.ensemble import RandomForestClassifier

from sklearn.neighbors import KNeighborsClassifier

from sklearn.metrics import log_loss, roc_auc_score, accuracy_score

model_1 = SVC(概率输出=True, 随机种子=0)

model_2 = RandomForestClassifier(随机种子=0)

model_3 = KNeighborsClassifier(   )

---

下一步仅需在训练集上训练每个模型：

---

model_1.fit(X_train, y_train)

model_2.fit(X_train, y_train)

model_3.fit(X_train, y_train)

---

此时需要对每个模型在测试集上进行预测，并通过多数表决法集成所有预测结果。为此我们将使用SciPy库中的mode函数：

---

import numpy as np

from scipy.stats import mode

preds = np.stack([model_1.predict(X_test),

model_2.predict(X_test),

model_3.predict(X_test)]). T

max_voting = np.apply_along_axis(mode, 1, preds)[:,0]

---

首先检查每个独立模型的准确率：

---

for i, model in enumerate(['SVC', 'RF ', 'KNN']):

acc = accuracy_score(y_true=y_test, y_pred=preds[:, i])

print(f"模型\{model\}的准确率为：\{acc:0.3f\}")

---

可见三个模型性能相近，均在0.8左右。现在检查多数表决集成效果：

---

max_voting_accuray = accuracy_score(y_true=y_test, y_pred=max_voting)

print(f"多数表决的准确率为：\{max_voting_accuray:0.3f\}")

---

表决集成实际准确率更高（0.817），因其成功整合了多数模型的正确信号。

针对多标签问题（当需要预测多个类别时），只需选取预测次数超过设定阈值的类别，该阈值表示对类别的预测是有效信号而非噪声。例如，若有五个模型，可将阈值设为3，这意味着只要至少三个模型预测了某类别，就应判定该预测正确。

在回归问题或概率预测场景中，多数投票法并不适用，因其仅适用于类别归属判断。当需要预测数值时，应采用数值方式整合结果，此时求取算术平均或加权平均是组合预测的正确方法。

## 模型预测的平均方法

在竞赛中整合不同模型的预测时，若认为所有预测具有同等效力，可采用算术平均数获得综合预测值。

除算术平均外，我们还发现以下方法颇具成效：

- 几何平均：将\( n \)次提交结果相乘后，对乘积取\( 1/{n}^{\text{th }} \)次方根

- 对数平均：类似几何平均，先对提交结果取对数，求平均值后再对结果取指数

- 调和平均：先计算提交结果倒数的算术平均，再对结果取倒数

- 幂次平均：先计算提交结果\( {n}^{\text{th }} \)次方的平均值，再对结果开\( 1/{n}^{\text{th }} \)次方根

简单算术平均通常效果显著且操作简便，其有效性常超预期。但几何平均或调和平均等变体有时表现更优。延续前例，当我们改用ROC-AUC作为评估指标时，需探究何种平均方法最适用。首先评估各单一模型表现：

---

proba = np.stack([model_1.predict_proba(X_test)[:, 1],

model_2.predict_proba(X_test)[:, 1],

model_3.predict_proba(X_test)[:, 1]]]).T

for i, model in enumerate(['SVC', 'RF ', 'KNN']):

ras = roc_auc_score(y_true=y_test, y_score=proba[:, i])

print(f"ROC-AUC for model \{model\} is: \{ras:0.5f\}")

---

结果显示数值范围在0.875至0.881之间。

首次测试采用算术平均数进行计算：

---

arithmetic = proba.mean(axis=1)

ras = roc_auc_score(y_true=y_test, y_score=arithmetic)

print(f"均值平均法ROC-AUC值为：\{ras:0.5f\}")

---

所得ROC-AUC分数0.90192显著优于单次测试结果。我们还验证了几何平均数、调和平均数、对数平均数及幂平均数是否优于普通平均数：

---

geometric = proba.prod(axis=1)**(1/3)

ras = roc_auc_score(y_true=y_test, y_score=geometric)

print(f"几何平均法ROC-AUC值为：\{ras:0.5f\}")

harmonic = 1 / np.mean(1. / (proba + 0.00001), axis=1)

ras = roc_auc_score(y_true=y_test, y_score=harmonic)

print(f"几何平均法ROC-AUC值为：\{ras:0.5f\}")

n = 3

mean_of_powers = np.mean(proba**n, axis=1)**(1/n)

ras = roc_auc_score(y_true=y_test, y_score=mean_of_powers)

print(f"幂平均法ROC-AUC值为：\{ras:0.5f\}")

logarithmic = np.expm1(np.mean(np.log1p(proba), axis=1))

ras = roc_auc_score(y_true=y测试集, y_score=对数预测值)

print(f"对数平均ROC-AUC值为: \{ras:0.5f\}")

---

运行代码将证明它们都无法胜任。此时，算术平均值成为集成模型的最佳选择。但几乎所有情况下，比简单平均更有效的方法是将先验知识融入数值组合方式——即在均值计算中为模型分配权重。

## 加权平均法

模型加权时，需通过实证方法确定最佳权重。常见做法是在公开排行榜测试不同权重组合（尽管极易导致自适应过拟合），但这无法保证在私有排行榜获得相同表现。核心原则是赋予表现更好的模型更高权重，但正如我们反复强调的，由于私有测试数据存在显著差异，公开排行榜反馈往往不可靠。此时可参考交叉验证分数或留出法分数（后者将在后续堆叠章节讨论）。另一种有效策略是根据模型的交叉验证表现按比例分配权重。

尽管有违直觉，另一种高效方法是按预测结果协方差的倒数分配权重。由于我们试图通过平均消除误差，基于各预测独特方差进行加权时，相关性更低、多样性更强的预测会获得更高权重，从而更有效降低估计值的方差。

下例中，我们将先创建预测概率的相关系数矩阵，然后：

1. 将对角线上的1值替换为0

2. 按行平均相关系数矩阵得到向量

3. 取每行和的倒数

4. 标准化使权重总和为1.0

5. 将最终权重向量与预测概率矩阵相乘

实现代码如下：

---

相关系数矩阵 = np.corrcoef(概率矩阵.T)

np.fill_diagonal(相关系数矩阵, 0.0)

权重向量 = 1 / np.mean(相关系数矩阵, axis=1)

W = W / sum(W) # 归一化至总和为1.0

加权结果 = 概率矩阵点乘权重W

ras = roc_auc_score(真实标签=y_test, 预测分数=加权结果)

print(f"加权平均ROC-AUC值为: \{ras:0.5f\}")

---

最终得到的0.90206 ROC-AUC值略优于简单平均法。给予相关性较低的预测更多权重，这种集成策略往往能取得成功。即便提升幅度有限，也足以在竞赛中占据优势。

## 交叉验证策略中的平均法

如前所述，平均法无需构建特殊复杂流程，仅需若干常规数据管道生成待平均模型，可采用等权重或经验权重。唯一验证方式是在公开排行榜提交结果，但这存在过拟合风险——因为评估完全依赖Kaggle平台的反馈。

不过在提交排行榜前，可通过在验证集（未用于模型训练的折数据）上运行平均操作进行训练阶段测试。相比排行榜反馈，这种方法偏差更小。以下代码展示了交叉验证预测的实现示例：

---

from sklearn.model_selection import KFold

kf = KFold(折数=5, 打乱=True, 随机种子=0)

分数列表 = list(   )

for 折序号, (训练索引, 测试索引) in enumerate(kf.split(训练集X)):

模型1.fit(训练集X[训练索引, :], 训练标签y[训练索引])

模型2.fit(训练集X[训练索引, :], 训练标签y[训练索引])

模型3.fit(训练集X[训练索引, :], 训练标签y[训练索引])

概率矩阵 = np.stack(   )

[model_1.predict_proba(X_train[test_index, :])[:, 1],

model_2.predict_proba(X_train[test_index, :])[:, 1],

model_3.predict_proba(X_train[test_index, :])[:, 1]]]).T

算术平均值 = proba.mean(axis=1)

ras = roc_auc_score(y_true=y_train[test_index],

y_score=算术平均值)

scores.append(ras)

print(f"FOLD \{k\} 平均ROC-AUC值为: \{ras:0.5f\}")

print(f"交叉验证平均ROC-AUC值为: \{np.mean(scores):0.5f\}")

---

依赖上述代码中的交叉验证结果，可帮助评估哪种平均策略更具潜力，而无需直接在公开排行榜上测试。

## 修正ROC-AUC评估的平均方法

若任务采用ROC-AUC评分评估，简单平均可能不足。因为不同模型可能采用不同优化策略，其输出结果可能存在显著差异。解决方案可包括校准模型（我们在第5章《竞赛任务与评估指标》中讨论过的后处理方法），但这显然需要额外时间和计算资源。

此类情况下，直接解决方案是将输出概率转换为排名后进行平均（或加权平均）。采用最小-最大缩放方法，只需将各模型估计值转换至0-1范围再进行平均预测。这将有效把模型概率输出转换为可比较的排名：

---

from sklearn.preprocessing import MinMaxScaler

proba = np.stack(   )

[model_1.predict_proba(X_train)[:, 1],

model_2.predict_proba(X_train)[:, 1],

model_3.predict_proba(X_train)[:, 1]]).T

算术平均 = MinMaxScaler(   ).fit_transform(proba).mean(axis=1)

ras = roc_auc_score(y_true=y_test, y_score=arithmetic)

print(f"均值融合的ROC-AUC值为: \{ras:0.5f\}")

---

当直接处理测试集预测时，这种方法效果极佳。但若在交叉验证过程中尝试融合结果，可能会因训练数据与测试数据的预测值范围差异而出现问题。此时可通过训练校准模型解决（参见Scikit-learn的概率校准章节（https://scikit-learn.org/stable/modules/calibration.html）及第五章），将各模型的预测值转换为真实可比较的概率。

## 使用元模型进行模型融合

Netflix竞赛（第一章已详细讨论）不仅证明了数据科学竞赛中融合策略对复杂问题的有效性，更开创了使用元模型优化模型结果融合的思路。冠军团队BigChaos在其论文（Töscher, A., Jahrer, M., and Bell, R.M. The BigChaos Solution to the Netflix Grand Prize. Netflix prize documentation - 2009）中多次提及混合(blending)技术，并揭示了其运作机制与显著效果。

简言之，混合技术是一种通过保留集和元模型来估计预测组合权重的加权平均方法。元模型本质上是学习其他机器学习模型输出的算法，通常采用线性模型（下节将探讨非线性情形），但实际可自由选择算法类型——不过需承担相应风险。

混合技术的实施流程简明直接：

1. 建模前先从训练数据随机抽取保留集（团队协作时应统一保留集）。通常保留\( {10}\% \)比例数据，但根据具体情况（如训练样本量、分层需求）可增减。抽样时建议强制分层以保证代表性，并通过对抗性验证确保其与训练集分布一致。

2. 在剩余训练数据上训练所有模型

3. 对保留集和测试集进行预测

4. 将保留集预测作为元模型的训练数据，再利用该元模型处理测试集预测得到最终结果。也可用元模型确定加权平均所需的预测变量及其权重。

此方法利弊兼具。优势在于：实施简便（仅需确定保留集），且通过元学习算法能自动获取最优权重，无需依赖公开排行榜测试。劣势包括：样本量减少可能增加预测方差（取决于模型类型）；即使精心抽样，仍可能因元模型过复杂导致适应性过拟合（即权重仅适用于保留集）；且与传统训练-测试集划分类似，当保留集过小或抽样不具代表性时，评估结果不可靠。

## 混合技术最佳实践

在混合学习中，所选用的元学习器类型至关重要。常用的选择是线性模型或非线性模型。线性模型中，线性回归或逻辑回归是首选。使用正则化模型也有助于剔除无效模型（L1正则化）或削弱次要模型的影响（L2正则化）。这类元学习器的局限在于可能给某些模型分配负权重——从模型系数值即可看出。若出现这种情况，通常表明模型过拟合，因为所有模型理应对集成产生正向贡献（最差也应保持中性）。Scikit-learn最新版本支持强制设定正权重并移除截距项，这些约束相当于正则化器，能防止过拟合。

非线性元学习器在回归和二元分类问题中较少使用，因其易导致过拟合，但在多类别和多标签分类任务中表现突出——它们能建模类别间的复杂关系。若除模型预测结果外还提供原始特征，其性能通常更优，因为能识别有助于判断模型可信度的有效交互特征。

接下来的示例中，我们先尝试用线性模型（逻辑回归）进行混合学习，再采用非线性方法（随机森林）。首先将训练集划分为混合元素训练集和元学习器验证集，随后在可训练部分拟合模型，并在验证集上预测。

---

from sklearn.preprocessing import StandardScaler

X_blend, X_holdout, y_blend, y_holdout = train_test_split(X_train, y_

train, test_size=0.25, random_state=0)

model_1.fit(X_blend, y_blend)

model_2.fit(X_blend, y_blend)

model_3.fit(X_blend, y_blend)

proba = np.stack([model_1.predict_proba(X_holdout)[:, 1],

model_2.predict_proba(X_holdout)[:, 1],

model_3.predict_proba(X_holdout)[:, 1]]]).T

scaler = StandardScaler(   )

proba = scaler.fit_transform(proba)

---

现在可以使用验证集上的预测概率来训练线性元学习器：

---

from sklearn.linear_model import LogisticRegression

blender = LogisticRegression(solver='liblinear')

blender.fit(proba, y_holdout)

print(blender.coef_)

---

最终得到的系数为：

## [[0.78911314 0.47202077 0.75115854]]

通过观察系数，我们可以判断哪个模型对元集成贡献更大。但需注意，当概率未经过良好校准时，系数也会重新调整概率尺度，因此某个模型的较大系数未必意味着它是最重要的。若想通过系数分析各模型在混合中的作用，首先需通过标准化重新调整系数（在我们的代码示例中，已使用Scikit-learn的StandardScaler完成此操作）。

输出结果显示，SVC和\( k \)-最近邻模型在混合中的权重高于随机森林模型；它们的系数几乎相当，且都大于随机森林的系数。

元模型训练完成后，我们只需对测试数据进行预测并评估其性能：

---

test_proba = np.stack([model_1.predict_proba(X_test)[:, 1],

model_2.predict_proba(X_test)[:, 1],

model_3.predict_proba(X_test)[:, 1]]]).T

blending = blender.predict_proba(test_proba)[:, 1]

ras = roc_auc_score(y_true=y_test, y_score=blending)

print(f"线性混合模型\{model\}的ROC-AUC值为：\{ras:0.5f\}")

---

我们可以尝试使用非线性元学习器（例如随机森林）进行相同操作：

---

blender = RandomForestClassifier(   )

blender.fit(proba, y_holdout)

test_proba = np.stack([model_1.predict_proba(X_test)[:, 1],

model_2.predict_proba(X_test)[:, 1],

model_3.predict_proba(X_test)[:, 1]]]).T

blending = blender.predict_proba(test_proba)[:, 1]

ras = roc_auc_score(y_true=y_test, y_score=blending)

print(f"非线性混合模型\{model\}的ROC-AUC值为: \{ras:0.5f\}")

---

Caruana、Niculescu-Mizil、Crew和Ksikes提出的集成选择技术，为使用线性或非线性模型作为元学习器提供了替代方案。

若需了解更多细节，请阅读他们的著名论文：Caruana, R., Nicules-cu-Mizil, A., Crew, G., and Ksikes, A. 《从模型库中进行集成选择》（第二十一届国际机器学习会议论文集，2004年）。

集成选择本质上是加权平均，因此可简单视作线性组合。但这是受约束的线性组合（因其属于爬山优化过程），不仅会筛选模型，且仅对预测结果施加正权重。该机制通过模型选择降低了过拟合风险，并确保解决方案更紧凑。鉴于这种特性，在过拟合风险较高（如训练样本不足或模型过于复杂）的场景及实际应用中，推荐采用集成选择——因其解决方案既简洁又高效。

使用元学习器时，其优化目标函数可能与竞赛评估指标不一致。集成选择的另一大优势是可针对任意评估函数进行优化，故特别适用于竞赛指标与机器学习模型常规优化标准不同的场景。根据前述论文，实施集成选择需遵循以下步骤：

1. 从训练好的模型和保留样本开始

2. 在保留样本上测试所有模型，根据评估指标保留效果最佳的模型（即集成选择）

3. 持续测试可加入集成选择的其他模型，使新组合的平均表现优于前次。可采用替换或非替换方式：非替换方式下，每个模型仅入选一次，此时过程类似于前向选择后的简单平均（前向选择指迭代加入最能提升性能的模型，直至性能不再改善）；替换方式则允许模型多次入选，形成加权平均效果。

4. 当无法获得进一步改进时停止，使用当前集成选择

以下是集成选择的简单代码示例。我们首先从原始训练数据中划分出混合集和保留集，拟合模型并获取保留集预测结果（如同元学习器混合时的操作）：

---

X_blend, X_holdout, y_blend, y_holdout = train_test_split

(X_train, y_train, 测试集比例=0.5, 随机种子=0)

模型_1.拟合(X_blend, y_blend)

模型_2.拟合(X_blend, y_blend)

模型_3.拟合(X_blend, y_blend)

概率矩阵 = np.堆叠([模型_1.预测概率(X_holdout)[:, 1],

模型_2.预测概率(X_holdout)[:, 1],

模型_3.预测概率(X_holdout)[:, 1]]]).转置

---

在接下来的代码片段中，集成模型通过一系列迭代创建。每次迭代时，我们尝试将所有模型依次加入当前集成，并检验它们是否能提升模型性能。若任何新增模型在保留样本上表现优于当前集成，则更新集成组合并将性能阈值提升至当前水平。

若无法通过新增模型改进集成，则终止循环并返回最终集成组合：

---

迭代次数 = 100

概率矩阵 = np.堆叠([模型_1.预测概率(X_holdout)[:, 1],

模型_2.预测概率(X_holdout)[:, 1],

模型_3.预测概率(X_holdout)[:, 1]]]).转置

基线值 = 0.5

打印(f"初始基线值为 \{baseline:0.5f\}")

模型集合 = []

循环次数范围内执行：

挑战者列表 = list(   )

在概率矩阵列数范围内循环：

新概率矩阵 = np.stack(概率矩阵[:, 模型集合 + [当前列]])

得分 = roc_auc_score(真实值=y_保留集,

预测值=np.mean(新概率矩阵, axis=1))

挑战者列表.append([得分, 当前列])

挑战者列表 = sorted(挑战者列表, key=lambda x: x[0],

降序=True)

最佳得分, 最佳模型 = 挑战者列表[0]

若最佳得分 > 基线值：

打印(f"将模型_\{最佳模型+1\}加入集成",

结尾=' : ')

打印(f"ROC-AUC分数提升至\{最佳得分:0.5f\}")

模型集合.append(最佳模型)

基线值 = 最佳得分

否则：

打印("无法进一步改进 - 停止")

---

最后，我们统计每个模型被纳入平均值的次数，并计算测试集上的加权系数：

---

从集合模块导入计数器

频次 = 计数器(模型列表)

权重 = \{键: 频次/模型总数 for 键, 频次 in 频次表.条目(   )\}

打印(权重)

---

可通过多种方式优化该流程。由于此方法可能过拟合（尤其在初始阶段），可从随机初始化的集成集开始，或如作者建议，直接使用集合中\( n \)个表现最佳的模型（将\( n \)值作为超参数）。另一种变体是对每轮迭代参与选择的模型进行抽样，即随机排除部分模型。这不仅能为过程注入随机性，还能防止特定模型主导选择。

## 模型堆叠

堆叠法最早见于David Wolpert的论文（Wolpert, D. H. 堆叠泛化. 神经网络5.2-1992），但历经多年才被广泛接受（例如Scikit-learn直到2019年12月的0.22版才实现堆叠封装器）。这主要归功于Netflix竞赛的推动，以及后续的Kaggle竞赛。

堆叠法始终需要元学习器。但不同于留出法，此次训练使用全训练集，这得益于折外预测策略。第6章《设计优质验证》已讨论该策略。折外预测始于可复现的\( k \)折交叉验证分割——可复现指通过记录每轮训练/测试集案例，或通过随机种子保证可重复性，能为每个待堆叠模型复制相同验证方案。

Netflix竞赛中"堆叠"与"混合"常混用，但Wolpert最初提出的方法基于\( k \)折交叉验证而非留出集。实际上，堆叠的核心不是像平均法那样降低方差，而主要是减少偏差，因为预期每个参与堆叠的模型都能捕捉数据中的部分信息，最终在元学习器中重组。

回顾训练数据折外预测原理：验证模型时，每轮用部分训练数据建模，在未参与训练的留出部分验证。记录验证预测后重新排序以匹配原始训练案例顺序，即可获得模型对所用训练集的预测。由于使用多个模型且每个模型都在未训练案例上预测，训练集预测不会有过拟合效应。

获得所有模型的折外预测后，可构建基于一级预测（折外预测）的元学习器，也可在现有折外预测上继续生成二级或更高级预测，形成多层堆叠。这与Wolpert提出的理念一致：使用多个元学习器实质是在模仿无反向传播的全连接前馈神经网络结构，其中各层权重单独优化以最大化预测性能。实践证明，多层堆叠对复杂问题非常有效，能突破单一算法的性能瓶颈。

值得注意的是，堆叠不要求模型具有可比预测力（平均法和混合法通常需要）。实际上，性能较差的模型在堆叠中也可能发挥作用。\( k \)-近邻模型虽不及梯度提升方案，但其折外预测可能正向贡献集成模型的整体性能。

完成所有堆叠层训练后进入预测阶段。关于各阶段预测生成方式，需注意两种途径：Wolpert原论文建议用全训练数据重新训练模型后预测测试集；实践中许多Kaggle选手直接使用各折模型对测试集进行多次预测后取平均。

根据我们的经验，当使用较少数量的\( k \)折交叉验证时，在预测测试集前对所有可用数据进行完整重新训练的堆叠方法通常更有效。这种情况下，样本一致性会显著影响预测质量——因为训练数据较少会导致估计值波动更大。如第六章所述，生成袋外预测时建议采用10至20折的高折数方案。这能减少被保留的样本数量，无需重新训练全部数据，只需对交叉验证模型得到的预测结果取平均值即可获得测试集预测。在接下来的示例中，为便于说明我们仅使用5折交叉验证，并进行了两次堆叠。下图展示了数据和模型在堆叠流程各阶段的流转关系：请注意：

<!-- Media -->

<!-- figureText: \( {1}^{\text{st }} \) level 2° level CV loop Train on CV folds and predict on validation fold Re-train on all training data Predict Mean preds preds CV loop train OOF Train on CV folds and predict on validation fold Re-train on all training data test Predict OOF -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_349.jpg?x=246&y=406&w=1394&h=717&r=0"/>

图9.1：带有最终预测平均的双层堆叠流程示意图

<!-- Media -->

- 训练数据同时输入堆叠的两个层级（第二层级的袋外预测会与训练数据合并）

- 从交叉验证循环获得袋外预测后，需在整个训练数据集上重新训练模型

- 最终预测是所有堆叠预测器所得预测的简单平均值

现在让我们通过代码理解该示意图如何转化为Python指令，从第一层训练开始：

---

from sklearn.model_selection import KFold

kf = KFold(n_splits=5, shuffle=True, random_state=0)

scores = list(   )

first_lvl_oof = np.zeros((len(X_train), 3))

fist_lvl_preds = np.zeros((len(X_test), 3))

for k, (train_index, val_index) in enumerate(kf.split(X_train)):

model_1.fit(X_train[train_index, :], y_train[train_index])

first_lvl_oof[val_index, 0] = model_1.predict_proba(   )

X_train[val_index, :])[:, 1]

model_2.fit(X_train[train_index, :], y_train[train_index])

first_lv1_oof[val_index, 1] = model_2.predict_proba(   )

X_train[val_index, :])[:, 1]

model_3.fit(X_train[train_index, :], y_train[train_index])

first_lv1_oof[val_index, 2] = model_3.predict_proba(   )

X_train[val_index, :])[:, 1]

---

第一层训练完成后，我们在完整数据集上重新训练：

---

model_1.fit(X_train, y_train)

fist_lvl_preds[:, 0] = model_1.predict_proba(X_test)[:, 1]

model_2.fit(X_train, y_train)

fist_lvl_preds[:, 1] = model_2.predict_proba(X_test)[:, 1]

model_3.fit(X_train, y_train)

fist_lvl_preds[:, 2] = model_3.predict_proba(X_test)[:, 1]

---

在第二层堆叠中，我们将复用第一层的相同模型，并将堆叠的OOF预测添加到现有变量中：

---

second_lvl_oof = np.zeros((len(X_train), 3))

second_lvl_preds = np.zeros((len(X_test), 3))

for k, (train_index, val_index) in enumerate(kf.split(X_train)):

skip_X_train = np.hstack([X_train, first_lvl_oof])

model_1.fit(skip_X_train[train_index, :],

y_train[train_index])

second_lvl_oof[val_index, 0] = model_1.predict_proba(   )

skip_X_train[val_index, :])[:, 1]

model_2.fit(skip_X_train[train_index, :],

y_train[train_index])

second_lv1_oof[val_index, 1] = model_2.predict_proba(   )

skip_X_train[val_index, :])[:, 1]

model_3.fit(skip_X_train[train_index, :],

y_train[train_index])

second_lvl_oof[val_index, 2] = model_3.predict_proba(   )

skip_X_train[val_index, :])[:, 1]

---

我们再次在完整数据上重新训练第二层模型：

---

skip_X_test = np.hstack([X_test, fist_lvl_preds])

model_1.fit(skip_X_train, y_train)

second_lvl_preds[:, 0] = model_1.predict_proba(skip_X_test)[:, 1]

model_2.fit(skip_X_train, y_train)

second_lvl_preds[:, 1] = model_2.predict_proba(skip_X_test)[:, 1]

model_3.fit(skip_X_train, y_train)

second_lvl_preds[:, 2] = model_3.predict_proba(skip_X_test)[:, 1]

---

堆叠法的最后一步是对第二层所有堆叠的OOF结果取平均值：

---

arithmetic = second_lvl_preds.mean(axis=1)

ras = roc_auc_score(y_true=y_test, y_score=arithmetic)

scores.append(ras)

print(f"堆叠法ROC-AUC值为: \{ras:0.5f\}")

---

最终ROC-AUC得分约为0.90424，优于先前在同一数据和模型上进行的混合与平均尝试。

## 堆叠法变体

堆叠法的主要变体包括：改变测试数据在各层的处理方式、是否仅使用堆叠OOF预测或在所有堆叠层保留原始特征、选择何种模型作为最终层，以及防止过拟合的各种技巧。以下是我们亲身验证过的高效方案：

- 可选择是否进行优化。有些方案不太关注单一模型优化；有些仅优化最后几层；还有些优先优化初始层。根据我们的经验，单一模型优化很重要，我们倾向于在堆叠集成早期完成。

- 不同堆叠层可使用不同模型，也可在各层重复相同模型序列。这需视具体问题而定，没有通用规则。梯度提升方案与神经网络的组合从未让我们失望。

- 在第一层堆叠时，尽可能创建多样化模型。例如分类问题可尝试回归模型，反之亦然。通过不同超参数设置生成模型群，无需过度优化，堆叠法会自主筛选。对于神经网络，仅改变随机初始化种子即可生成差异化模型池。还可尝试不同特征工程方案，甚至引入无监督学习（如Mike Kim在Otto产品分类挑战中应用t-SNE维度的方法：https://www.kaggle.com/c/otto-group-product-classification-challenge/discussion/14295）。关键在于第二层堆叠会完成这些贡献度的筛选，这意味着后续无需再实验，只需聚焦于表现更优的模型子集。堆叠法能复用所有实验成果，并自动决定它们在建模流程中的适用程度。

- 某些堆叠实现会携带全部特征或部分特征进入后续阶段，这让人联想到神经网络中的跳跃层。我们注意到，在堆叠后期引入特征可以提升效果，但需谨慎：这同时会带来更多噪声和过拟合风险。

- 理想情况下，您的OOF（Out-of-Fold）预测应通过高折数交叉验证方案生成，换言之，折数应介于10至20之间。但我们也观察到采用较低折数（例如5折）的解决方案同样有效。

- 对于每一折，对同一模型多次进行数据装袋（有重复的重新采样），然后对模型的所有结果（袋外预测和测试预测）取平均值，有助于避免过拟合并最终获得更好的结果。

- 警惕堆叠模型中的早停机制。直接在验证折叠上使用可能导致一定程度的过拟合，这种过拟合最终未必能被堆叠流程缓解。建议采取保守策略，始终基于训练折叠中的验证样本（而非验证折叠本身）来实施早停。

可能性是无限的。一旦掌握了这种集成技术（ensembling technique）的基本概念，您只需将创造力应用于当前问题即可。我们将在本章最后一节讨论这一关键概念，届时将分析一个Kaggle竞赛的堆叠（stacking）解决方案。

## 创建复杂的堆叠与混合解决方案

在本章的这个阶段，您可能想知道应该在多大程度上应用我们讨论的这些技术。理论上，您可以在Kaggle的任何竞赛中使用我们介绍的所有集成技术，而不仅限于表格类竞赛，但您需要考虑几个限制因素：

- 有时，数据集非常庞大，训练单个模型需要很长时间。

- 在图像识别竞赛中，您仅限于使用深度学习方法。

- 即便在深度学习竞赛中能够成功堆叠模型，您对组合不同模型的选择也相当有限。由于受限于深度学习解决方案，您只能调整网络的小部分设计细节和某些超参数（有时仅能改变初始化种子），以免性能下降。最终，给定相同类型的模型以及架构上相似性远大于差异性的情况下，各预测结果往往会过于相似且相关性超出应有范围，从而限制了集成学习的有效性。

在这些条件下，复杂的堆叠机制通常难以实现。相比之下，当拥有大型数据集时，平均化和混合方法通常是可行的。

在早期竞赛以及近期所有表格类比赛中，复杂的堆叠(stacking)与融合(blending)解决方案占据主导地位。为了让您了解竞赛中堆叠方法所需的复杂性与创造力，本节最后我们将讨论Gilberto Titericz(https://www.kaggle.com/titericz)与Stanislav Semenov(https://www.kaggle.com/stasg7)为Otto集团产品分类挑战赛(https://www.kaggle.com/c/otto-group-product-classification-challenge)提供的解决方案。该竞赛于2015年举办，任务要求根据93个特征将超过20万种产品划分到9个不同类别。Gilberto和Stanislav提出的解决方案包含三个层级：

1. 在第一层级中，共有33个模型。除了一组仅\( k \)参数不同的\( k \)-最近邻算法外，所有模型采用差异显著的算法。这些模型还运用了无监督的t-SNE技术。此外，研究团队基于维度操作（对最近邻与聚类距离的计算）和行统计（每行非零元素的数量）构建了八个特征。所有OOF预测结果和特征均被传递至第二层级。

2. 在第二阶段，他们开始优化超参数并进行模型选择与装袋法（通过重采样创建同一模型的多个版本，并对每个模型的结果取平均值）。最终仅保留三个模型进行全量数据重训练：XGBoost算法、AdaBoost算法和神经网络。

3. 在第三层级，他们通过先对XGBoost和神经网络的结果取几何平均数，再与AdaBoost的结果进行平均，计算出了加权平均值。

我们可以从该解决方案中学到很多，且不仅限于本次比赛。除了复杂度（在第二层级，每个模型的重采样次数达到数百次量级），值得注意的是本章讨论的方案存在多种变体。创造力与反复试验明显主导了这个解决方案。这在Kaggle竞赛中相当典型——问题很少在不同比赛间重复出现，每个解决方案都独一无二且不易复现。

许多自动机器学习引擎（如AutoGluon）或多或少都明确尝试从这些流程中汲取灵感，通过堆叠和混合提供预定义的自动化步骤序列，确保您获得最佳结果。

请参阅https://arxiv.org/abs/2003.06505了解AutoGluon用于构建堆叠模型的算法列表。该列表相当长，您会从中获得许多构建自己堆叠解决方案的灵感。

然而，尽管它们实现了当前最佳实践，但与优秀Kaggle团队所能达到的效果相比，其结果始终略逊一筹，因为实验方法和集成组合的创造力才是成功关键。本章亦是如此——我们已展示集成的最佳实践，请以此为起点，根据您参与的Kaggle竞赛或实际业务问题，通过混合创意与创新来打造专属方案。

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_355.jpg?x=247&y=236&w=350&h=353&r=0"/>

<!-- Media -->

## 泽维尔·科诺特

https://www.kaggle.com/xavierconort

作为章节收尾，我们采访了2012-2013年度排名第一的竞赛宗师泽维尔·科诺特。这位Kaggle早期历史中激励无数选手的传奇人物，如今是数据测绘与工程公司的创始人兼CEO，向我们分享了他在Kaggle的经历、职业生涯等见解。

## 您最青睐哪类竞赛？原因是什么？在技术方法和解决路径方面，您在Kaggle上的专长是什么？

我特别享受需要通过多表特征工程才能取得好成绩的竞赛。热衷于挖掘优质特征，尤其是面对陌生的商业问题时——这极大增强了应对新挑战的信心。除特征工程外，堆叠法助我屡创佳绩：既用于混合多模型，也将文本或高基数分类变量转化为数值特征。虽然梯度提升机(GBM)是我的首选算法，但为增强融合多样性，我测试过大量其他算法。

## 您如何规划Kaggle竞赛策略？这与日常工作方法有何不同？

我的首要目标是从每场竞赛中最大化学习。参赛前会评估可提升的技能维度，主动突破舒适区。排行榜的即时反馈能加速纠错——这种学习机遇在日常工作中极为罕见，因为我们难以评估解决方案的真实质量，往往选择保守重复既有方案。可以说，没有Kaggle就没有我如今的成长。

## 请分享一场特别具有挑战性的竞赛经历，以及您破局的关键洞察

我最钟爱的是GE飞行挑战赛，需预测美国国内航班抵达时间。该竞赛巧妙设计了私有排行榜——通过评估截止日期后真实航班数据的预测准确性，考验我们对未来事件的预测能力。鉴于仅有3-4个月历史数据（如记忆无误），过拟合风险极高。为此我只构建与航班延误有明确因果关系的特征（如天气、交通指标），并刻意避免直接使用机场名称——因为某些机场在有限历史期内未经历恶劣天气，担心GBM算法会将其误判为天气良好的代理变量。最终为略微提升分数，我以残差效应形式在第二层模型中引入机场名称（作为第一层预测值的偏移量），这种两阶段提升法借鉴了保险精算师捕捉地理空间残差效应的技术。

## Kaggle是否对您的职业生涯有所帮助？具体体现在哪些方面？

这段经历无疑对我的数据科学家职业生涯大有裨益。在转型数据科学之前，我本是保险行业的精算师，对机器学习一无所知，也不认识任何数据科学家。得益于Kaggle丰富多样的竞赛，我的学习曲线得以加速。凭借优异成绩，我能够展示实力履历，让雇主相信39岁的精算师也能自主掌握新技能。更因Kaggle的社区平台，我与全球众多充满激情的数据科学家建立了联系。起初在与他们合作或对抗中获得了无穷乐趣，最终更获得与其中佼佼者共事的机会——DataRobot创始人杰里米·阿钦和汤姆·德戈多伊，正是在邀请我加入公司前与我并肩作战的竞赛队友。若非Kaggle的助力，我想至今我仍会留在保险行业从事精算工作。

你是否曾将在Kaggle竞赛中的成果纳入作品集，用以向潜在雇主展示？

坦白说，我确实参加过几场旨在打动雇主或潜在客户的竞赛。效果虽佳，却少了乐趣，多了压力。

## 根据你的经验，新手Kaggle用户常会忽视什么？现在的你希望刚入门时就知道哪些事？

建议新手不要查看竞赛期间公布的解决方案，而应尝试独立寻找优质方案。我很庆幸Kaggle早期参赛者不共享代码——这迫使我在艰难摸索中获得真知。

## 你在过往竞赛中犯过哪些错误？

常见错误是持续参加存在数据泄露的设计缺陷竞赛。这纯粹浪费时间，从中几乎学不到东西。

# 在数据分析或机器学习领域，有哪些特别推荐的工具或库？

梯度提升机(GBM)是我最钟爱的算法。我先后使用过R的gbm、Scikit-learn的GBM、

XGBoost以及最终的LightGBM。多数时候，它都是我夺冠方案的核心要素。若要理解GBM的学习机制，推荐使用SHAP工具包。

参加竞赛时最需要牢记或践行的重要事项是什么？

为学习而竞赛，为结识志同道合的数据科学家而竞赛，不要仅为获胜而竞赛。

## 本章小结

本章探讨了集成多解决方案的工作原理，并提供基础代码示例助你构建自己的方案。我们从随机森林、梯度提升等集成模型的核心思想出发，进而研究不同集成方法——从简单的测试结果平均，到多层次堆叠模型的元建模。

如结尾所述，集成更像基于共同实践的艺术形式。当我们剖析某个Kaggle夺冠的复杂堆叠方案时，其与数据及问题本身的高度适配令人惊叹。你无法直接套用某个堆叠方案到其他问题并指望它成为最佳解，唯有遵循指导原则，通过大量实验和计算，自行寻找包含平均/堆叠/混合多种模型的最佳方案。

下一章我们将深入深度学习竞赛领域，从计算机视觉的分类与分割任务开始。

## 加入我们的书籍Discord空间

加入本书的Discord工作区，每月参与作者问答会：

https://packt.link/KaggleDiscord 10

## 计算机视觉建模

计算机视觉任务是机器学习实际应用中最热门的问题之一；对于许多Kaggle竞赛参与者（包括笔者Konrad在内），它们正是进入深度学习领域的敲门砖。近年来该领域取得巨大进展，新的SOTA（State Of The Art）库不断涌现。本章将概述计算机视觉中最常见的竞赛类型：- 图像分类 - 目标检测 - 图像分割

我们将从图像增强的简要章节开始，这是一组与任务无关的技术，可应用于不同问题以提高模型的泛化能力。

## 增强策略

尽管深度学习技术在图像识别、分割或目标检测等计算机视觉任务中取得了极大成功，但底层算法通常具有极高的数据依赖性：它们需要大量数据来避免过拟合。然而并非所有目标领域都能满足这一需求，这正是数据增强技术的用武之地。这类图像处理技术通过创建图像的修改版本，从而扩大训练数据集的规模并提升质量，最终提高深度学习模型的性能。增强后的数据通常能呈现更全面的可能数据点分布，从而最小化训练集与验证集之间、以及未来测试集之间的差距。本节我们将回顾一些常见增强技术及其软件实现方案。最常用的变换包括：

- 翻转：沿水平或垂直轴翻转图像

- 旋转：按给定角度（顺时针或逆时针）旋转图像

- 裁剪：随机选取图像的局部区域

- 亮度：调整图像亮度

- 缩放：将图像放大（向外）或缩小（向内）

下面我们以美国传奇演员兼喜剧演员贝蒂·怀特的照片为例，演示这些变换的实际效果：

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_360.jpg?x=678&y=790&w=530&h=707&r=0"/>

图10.1：贝蒂·怀特原图

<!-- Media -->

我们可以沿垂直或水平轴翻转图像：

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_361.jpg?x=418&y=287&w=1055&h=707&r=0"/>

图10.2：贝蒂·怀特图像 - 垂直翻转（左）与水平翻转（右）

<!-- Media -->

旋转操作不言自明；请注意背景中自动填充的图像边缘：

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_361.jpg?x=673&y=1169&w=538&h=706&r=0"/>

图10.3：贝蒂·怀特图像 - 顺时针旋转

<!-- Media -->

我们还可以对图像进行兴趣区域裁剪：

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_362.jpg?x=692&y=280&w=501&h=505&r=0"/>

图10.4：贝蒂·怀特图像 - 裁剪版

<!-- Media -->

从宏观层面看，增强技术可通过两种方式实现：

- 离线增强：通常适用于较小数据集（图像数量较少或尺寸较小，但"小"的定义取决于硬件配置）。其核心思想是作为数据集的预处理步骤，生成原始图像的修改版本，随后与"原始"图像共同使用。

- 在线增强：适用于大型数据集。增强后的图像不会存储在磁盘上，而是在小批量处理时实时应用并输入模型。

接下来几节将概述两种最常用的图像数据集增强方法：Keras内置功能和albumentations包。其他可选方案（skimage、OpenCV、imgaug、Augmentor、SOLT）虽存在，但我们将聚焦主流工具。

本章讨论的方法专注于GPU驱动的图像分析。虽然张量处理单元(TPU)的应用正在兴起，但目前仍属细分领域。建议对TPU驱动分析与图像增强结合的读者参考Chris Deotte(@cdeotte)的卓越成果：

https://www.kaggle.com/cdeotte/triple-stratified-kfold-with-tfrecords

Chris是四度Kaggle大师，通过其创建的Notebook和参与的讨论展现了卓越的教育才能；无论经验水平如何，他都是所有Kaggle用户值得关注的对象。

我们将使用木薯叶病害分类竞赛(https://www.kaggle.com/c/cassava-leaf-disease-classification)数据。依照惯例，我们从基础

---

工作开始：首先加载必要包：

import os

import glob

import numpy as np

import scipy as sp

import pandas as pd

import cv2

from skimage.io import imshow, imread, imsave

#图像增强库

导入图像处理库

导入imgaug库

导入imgaug增强器模块

#Albumentations库

导入albumentations库

#Keras框架

#从keras预处理模块导入图像生成器、数组转换、

图像转数组、加载图像

#可视化工具

导入matplotlib绘图模块

导入matplotlib图像模块

%matplotlib内联显示

导入seaborn库

从IPython导入HTML和图像显示功能

#警告处理

导入警告模块

设置忽略警告

---

接下来定义辅助函数以简化后续展示。我们需要将图像加载为数组：

---

定义图像加载函数：

文件路径 = 图像ID

图像 = 读取图像(图像数据路径 + 文件路径)

返回图像

---

为以画廊形式展示多张图像，创建函数接收图像数组和列数，输出按指定列数重排的网格数组：

---

定义画廊布局函数：

索引数、高度、宽度、强度 = 数组形状

行数 = 索引数//列数

断言索引数等于行列乘积

结果 = (数组重塑(行数, 列数, 高度, 宽度, 强度)

交换轴(1,2)

重塑(高度*行数, 宽度*列数, 强度))

返回结果

---

完成基础设置后，我们可以加载待增强的图像：

---

data_dir = '../input/cassava-leaf-disease-classification/'

Image_Data_Path = data_dir + '/train_images/'

train_data = pd.read_csv(data_dir + '/train.csv')

#我们将前10张图像加载到内存中以加快访问速度

train_images = train_data["image_id"][:10].apply(load_image)

---

让我们加载单张图像作为参考基准：

---

curr_img = train_images[7]

plt.figure(figsize = (15,15))

plt.imshow(curr_img)

plt.axis('off')

---

参考图像如下：

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_365.jpg?x=533&y=285&w=821&h=626&r=0"/>

图10.5：参考图像

<!-- Media -->

后续章节将演示如何通过Keras内置功能和albumentations库从该参考图像生成增强图像。

## Keras内置增强功能

Keras库内置了图像增强功能，虽不及专业工具包全面，但能轻松集成到现有代码中。我们无需单独定义增强变换，可直接将其整合到ImageDataGenerator中——这个功能模块很可能已被使用。

我们研究的第一个Keras方法基于ImageDataGenerator类。顾名思义，它可用于生成带有实时数据增强的批量图像数据。

## ImageDataGenerator方法

我们首先通过以下方式实例化ImageDataGenerator类的对象：

---

import tensorflow as tf

from tensorflow.keras.preprocessing.image import ImageDataGenerator,

array_to_img, img_to_array, load_img

datagen = ImageDataGenerator(   )

rotation_range = 40,

shear_range = 0.2,

zoom_range = 0.2,

horizontal_flip = True,

brightness_range = (0.5,1.5))

curr_img_array = img_to_array(curr_img)

curr_img_array = curr_img_array.reshape((1,) + curr_img_array.shape)

---

我们将所需增强定义为ImageDataGenerator的参数。官方文档似乎未涉及此主题，但实际结果表明增强是按照参数定义的顺序应用的。

上述示例中仅使用了有限的可选参数子集；完整列表建议读者查阅官方文档：https://keras.io/api/preprocessing/image/。

接下来，我们通过ImageDataGenerator对象的.flow方法遍历图像。该类提供了三种不同的函数将图像数据集加载到内存中并生成增强数据批次：

- flow

- flow_from_directory

- flow_from_dataframe 它们都实现相同目标，但指定文件位置的方式不同。在我们的示例中，图像已在内存中，因此可以使用最简单的方法进行迭代：

---

i = 0

for batch in datagen.flow(   )

curr_img_array,

batch_size=1,

save_to_dir='.',

save_prefix='增强图像',

save_format='jpeg'):

	i += 1

#硬编码停止条件 - 若无此条件，生成器将进入无限循环

if i > 9 :

break

---

我们可以使用先前定义的辅助函数检查增强后的图像：

---

aug_images = []

for img_path in glob.glob("*.jpeg"):

增强图像列表.append(mpimg.读取图片(img_path))

plt.创建图形(尺寸=(20,20))

plt.关闭坐标轴()

plt.显示图像(画廊(np.数组(增强图像[0:9]), 列数=3))

plt.标题('数据增强示例')

---

结果如下：

<!-- Media -->

<!-- figureText: Augmentation examples -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_367.jpg?x=410&y=862&w=1066&h=847&r=0"/>

图10.6：增强后的图像集合

<!-- Media -->

数据增强是非常有用的工具，但高效使用需要专业判断。首先，可视化增强效果以感知数据变化是明智之举。一方面，我们需要引入数据变异来提升模型泛化能力；另一方面，过度改变图像会导致信息损失并损害模型性能。此外，增强方法的选择需结合具体问题——对比不同竞赛可见差异。观察图10.6（木薯叶病害分类竞赛的参考图像），由于植物形态和拍摄角度差异，待识别的病叶可能存在尺寸不一、角度各异等情况，因此垂直/水平翻转、裁剪、旋转等变换在此场景都适用。

相比之下，Severstal钢铁缺陷检测竞赛的样本图像（https://www.kaggle.com/c/severstal-steel-defect-detection）则呈现不同特点。该竞赛要求定位和分类钢板缺陷，所有图像尺寸和方向一致。此时若进行旋转或裁剪，反而会产生不真实的噪声图像，损害算法的泛化能力。

<!-- Media -->

<!-- figureText: 5a8203514.jpg has defect 3 28a3f7928.jpg has defect 2 6e7bace88.jpg has defect 3 acc4098ce.jpg has defect 1 -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_368.jpg?x=246&y=798&w=1394&h=1163&r=0"/>

图10.7：Severstal竞赛样本图像

<!-- Media -->

## 预处理层

另一种原生Keras风格的数据增强方案是使用预处理层API。该功能极具灵活性：这些管道既可结合Keras模型使用，也能像ImageDataGenerator那样独立运作。

以下简要展示预处理层配置方法。首先导入模块：

---

from tensorflow.keras.layers.experimental import preprocessing

from tensorflow.keras import layers

---

我们以标准Keras方式加载预训练模型：

---

预训练基模型 = tf.keras.models.load_model(   )

'../input/cv-course-models/cv-course-models/vgg16-pretrained-base',

)

预训练基模型.可训练 = 假

---

预处理层可以像其他层一样在Sequential构造函数中使用；唯一的要求是它们需要在模型定义的最开始、其他所有层之前被指定：

---

模型 = tf.keras.Sequential([

#预处理层

预处理.随机翻转('水平'), # 左右翻转

预处理.随机对比度(0.5), # 对比度变化最高达50%

#基模型

预训练基模型,

#模型头部定义

层.展平(   ),

层.全连接(6, 激活='relu'),

层.全连接(1, 激活='sigmoid'),

])

---

## 图像增强库

albumentations包是一个快速的图像增强库，它是作为对其他库的某种封装而构建的。

该软件包是经过多场Kaggle竞赛高强度编码的成果（详见https://medium.com/@iglovikov/the-birth-of-albumentations-fe38c1411cb3），其核心开发者和贡献者中包含多位知名Kaggle选手，包括Eugene Khvedchenya（https://www.kaggle.com/bloodaxe）、Vladimir Iglovikov（https://www.kaggle.com/iglovikov）、Alex Parinov（https://www.kaggle.com/creafz）以及ZFTurbo（https://www.kaggle.com/zfturbo）。

完整文档请访问：https://albumentations.readthedocs.io/en/latest/

以下列出其主要特性：

- 面向不同数据类型的统一API

- 支持所有常见计算机视觉任务

- 兼容TensorFlow和PyTorch框架

使用albumentations进行图像变换非常简单。首先初始化所需变换：

---

import albumentations as A

horizontal_flip = A.HorizontalFlip(p=1)

rotate = A.ShiftScaleRotate \( \left( {p = 1}\right) \)

gaus_noise = A.GaussNoise(   )

bright_contrast = A.RandomBrightnessContrast(p=1)

gamma = A. RandomGamma(p=1)

blur = A.Blur(   )

---

接着将变换应用到基准图像：

---

img_flip = horizontal_flip(image = curr_img)

高斯噪声图像 = gaus_noise(图像=当前图像)

旋转图像 = rotate(图像=当前图像)

亮度对比度图像 = bright_contrast(图像=当前图像)

伽马校正图像 = gamma(图像=当前图像)

模糊图像 = blur(图像=当前图像)

---

可通过'image'键访问增强后的图像并可视化结果：

---

图像列表 = [翻转图像['image'],高斯图像['image'], 旋转图像['image'],

亮度对比图像['image'], 伽马图像['image'], 模糊图像['image']]

plt.figure(画布尺寸=(20,20))

plt.axis('关闭')

plt.imshow(画廊(np.array(图像列表), 列数=3))

plt.title('增强示例')

---

## 结果展示：

<!-- Media -->

<!-- figureText: Augmentation examples -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_371.jpg?x=423&y=737&w=1040&h=566&r=0"/>

图10.8：使用albumentations库增强的图像

<!-- Media -->

在将数据增强作为计算机视觉问题关键预处理步骤讨论后，我们现在可以将其应用于后续章节，从最常见的图像分类任务开始。

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_371.jpg?x=240&y=1629&w=359&h=364&r=0"/>

于2019年加入Kaggle。

<!-- Media -->

## 克里斯·德奥特

https://www.kaggle.com/cdeotte

在继续之前，让我们回顾一下与克里斯·德奥特的简短对话——我们在本书中多次提及他（包括本章前文），这绝非偶然。作为四度Kaggle大师赛冠军得主、NVIDIA高级数据科学家兼研究员，

# 您最青睐哪类竞赛？为什么？在技术方法和解决思路上，您在Kaggle的专长是什么？

我钟爱数据极具吸引力的竞赛，以及需要构建创新模型的竞赛。

我的专长是分析训练好的模型，评估其优劣。之后我喜欢改进模型和/或开发后处理技术来提升交叉验证下限(CVLB)。

您如何规划Kaggle竞赛策略？这与日常工作有何不同？

每项竞赛我都从探索性数据分析(EDA)开始，建立本地验证集，构建简单模型，提交Kaggle获取排行榜分数。这能培养直觉，明确构建精准竞争力模型所需步骤。

请分享一个您参与过的极具挑战性的竞赛，以及您用来解决问题的洞见。

Kaggle的Shopee价格匹配挑战赛需要同时运用图像模型和自然语言模型。关键突破是从两类模型中提取嵌入特征，再融合图像与文本信息来匹配商品。

## Kaggle对您的职业发展有帮助吗？具体体现在？

当然。Kaggle通过提升我的技能和简历竞争力，助我成为NVIDIA高级数据科学家。

许多雇主会细读Kaggle作品来寻找具备特定技能的员工。正因如此，我收到了众多工作邀约。

## 根据您的经验，新手Kaggle选手常忽视什么？您现在希望初入行时就明白的是什么？

我认为新手常低估本地验证的重要性。看到名字出现在排行榜令人兴奋，但人们容易只关注提升排行榜分数而非交叉验证分数。

## 您过去在竞赛中犯过哪些错误？

我曾多次错误地相信排行榜分数胜过交叉验证分数，从而选择了错误的最終提交方案。

# 对于数据分析或机器学习，您推荐使用哪些特定的工具或库？

当然。在优化表格数据模型时，特征工程和快速实验非常重要。为了加速实验和验证周期，使用NVIDIA RAPIDS cuDF和cuML GPU加速库至关重要。

# 参加竞赛时最需要牢记或做到的重要事项是什么？

最重要的是享受乐趣并学习。不必担心最终排名。如果专注于学习和享受过程，随着时间的推移，你的最终排名会越来越好。

## 您是否使用其他竞赛平台？与Kaggle相比如何？

是的，我参加过Kaggle以外的竞赛。像Booking.com或Twitter.com这样的公司偶尔会举办竞赛。这些竞赛很有趣，涉及高质量的实时数据。

## 分类

本节将演示一个端到端的流程模板，用于处理图像分类问题。我们将逐步介绍从数据准备、模型设置与评估到结果可视化的必要步骤。最后一步除了具有信息性（且很酷）外，若需深入检查代码以更好地理解性能，也将非常有用。

我们将继续使用木薯叶病害分类竞赛的数据(https://www.kaggle.com/c/cassava-leaf-disease-classification)。

照例，我们首先加载必要的库：

---

import numpy as np

import pandas as pd

import matplotlib.pyplot as plt

import datetime

from sklearn.model_selection import train_test_split

from sklearn.metrics import accuracy_score

导入 tensorflow 库（简写为 tf）

从 tensorflow.keras 导入 models 和 layers 模块

从 tensorflow.keras.preprocessing 导入 image 模块

从 tensorflow.keras.preprocessing.image 导入 ImageDataGenerator 类

从 tensorflow.keras.callbacks 导入 ModelCheckpoint, EarlyStopping,

ReduceLROnPlateau 回调函数

从 tensorflow.keras.applications 导入 EfficientNetB0 网络结构

从 tensorflow.keras.optimizers 导入 Adam 优化器

导入 os, cv2, json 库

从 PIL 库导入 Image 模块

---

定义辅助函数通常是明智之举，这能让代码更易读且便于调试。对于通用图像分类问题，采用EfficientNet系列模型是个不错的起点——该系列由谷歌研究大脑团队在2019年论文(https://arxiv.org/abs/1905.11946)中提出，其核心思想是通过平衡网络深度、宽度和分辨率，实现跨维度的高效缩放从而提升性能。本方案将使用该系列最简版本EfficientNet B0，这个移动端规模的网络包含1100万个可训练参数。

若需深入了解EfficientNet网络，建议以谷歌AI博客(https://ai.googleblog.com/2019/05/efficientnet-improving-accuracy-and.html)作为入门参考。

我们以B0为基础构建模型，后接提升平移不变性的池化层，以及配备适用于多分类问题激活函数的全连接层：

---

class CFG:

#配置项

WORK_DIR = '../input/cassava-leaf-disease-classification'

批次大小 = 8

训练轮次 = 5

目标尺寸 = 512

def 创建模型(   ):

卷积基 = EfficientNetB0(包含顶层 = 否, 权重 = 无,

输入形状 = (配置.目标尺寸,

配置.目标尺寸, 3))

模型 = 卷积基.输出

模型 = 层.全局平均池化2D(   )(模型)

模型 = 层.全连接层(5, 激活 = "softmax")(模型)

模型 = 模型.模型(卷积基.输入, 模型)

模型.编译(优化器 = Adam(学习率 = 0.001),

损失函数 = "稀疏分类交叉熵",

评估指标 = ["准确率"])

返回 模型

---

关于传递给EfficientNetB0函数的参数简要说明：

- include_top参数用于决定是否包含最终的全连接层。由于我们需要将预训练模型作为特征提取器使用，默认策略是跳过这些层并自行定义头部结构。

- 若需从头开始训练模型，可将weights设为None；若想使用基于大型图像集预训练的权重，则可设为'imagenet'或'noisy-student'。

以下辅助函数可帮助我们可视化激活层，从而从视觉角度评估网络性能。这在开发直觉时尤为有用，特别是在这个以不透明性著称的领域：

---

def activation_layer_vis(img, activation_layer = 0, layers = 10):

layer_outputs = [layer.output for layer in model.layers[:layers]]

activation_model = models.Model(inputs = model.input,

outputs = layer_outputs)

activations = activation_model.predict(img)

rows = int(activations[activation_layer].shape[3] / 3)

cols = int(activations[activation_layer].shape[3] / rows)

fig, axes = plt.subplots(rows, cols, figsize = (15, 15 * cols))

axes = axes.flatten(   )

for i, ax in zip(range(activations[activation_layer].shape[3]), axes):

ax.matshow(activations[activation_layer][0, :, :, i],

cmap = 'viridis')

ax.axis('off')

plt.tight_layout(   )

plt.show(   )

---

我们通过基于"受限"模型生成预测来产生激活值，换句话说，使用直到倒数第二层的整个架构；这部分代码对应到激活变量之前的部分。函数的其余部分确保我们展示与相应卷积层中滤波器形状匹配的激活布局。

接下来，我们处理标签并设置验证方案；数据中没有特殊结构（例如时间维度或跨类别重叠），因此可以采用简单的随机分割：

---

train_labels = pd.read_csv(os.path.join(CFG.WORK_DIR, "train.csv"))

STEPS_PER_EPOCH = len(train_labels)*0.8 / CFG.BATCH_SIZE

VALIDATION_STEPS = len(train_labels)*0.2 / CFG.BATCH_SIZE

---

如需了解更复杂的验证方案，请参阅第6章《设计良好的验证》。

现在我们可以建立数据生成器，这是基于TF的算法循环处理图像数据所必需的。

首先实例化两个ImageDataGenerator对象，此时我们将图像增强方法整合进来。本次演示将使用Keras内置增强方法。随后通过flow_from_dataframe()方法创建生成器，该方法用于生成带有实时数据增强的张量图像数据批次：

---

train_labels.label = train_labels.label.astype('str')

train_datagen = ImageDataGenerator(   )

validation_split = 0.2, preprocessing_function = None,

rotation_range = 45, zoom_range = 0.2,

horizontal_flip = True, vertical_flip = True,

fill_mode = 'nearest', shear_range = 0.1,

高度偏移范围 = 0.1, 宽度偏移范围 = 0.1)

训练生成器 = 训练数据生成器.从数据框生成流(   )

训练标签,

目录 = os.path.join(配置.工作目录, "训练图像"),

子集 = "训练",

x列 = "图像ID",y列 = "标签",

目标尺寸 = (配置.目标尺寸, 配置.目标尺寸),

批次大小 = 配置.批次大小,

分类模式 = "稀疏")

验证数据生成器 = 图像数据生成器(验证分割 = 0.2)

验证生成器 = 验证数据生成器.从数据框生成流(   )

训练标签,

目录 = os.path.join(配置.工作目录, "训练图像"),

子集 = "验证",

x列 = "图像ID",y列 = "标签",

目标尺寸 = (配置.目标尺寸, 配置.目标尺寸),

batch_size = CFG.BATCH_SIZE, class_mode = "sparse")

---

数据结构定义完成后，即可创建模型：

---

model = create_model(   )

model.summary(   )

---

模型创建后，可快速查看摘要。这主要用于完整性校验，因为除非拥有照相记忆，否则很难记住像EffNetBO这类复杂模型的层级结构。实践中，可通过摘要检查输出滤波器维度是否正确，或参数数量（可训练/不可训练）是否符合预期。为简洁起见，下文仅展示输出前几行；参考B0架构图即可了解完整输出的长度。

<!-- Media -->

<!-- figureText: Model: "functional_1" Param # Connected to [(None, 512, 512, 3) 0 input_1[0][0] rescaling[0][0] normalization[0] Layer (type) Output Shape input_1 (InputLayer) rescaling (Rescaling) stem_conv_pad (ZeroPadding2D) (None, 513, 513, 3) 0 [0] -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_377.jpg?x=259&y=1484&w=1377&h=622&r=0"/>

<!-- figureText: (None 256, 256, 32) 864 stem_conv_ 256, 256 32) 128 stem conv[0][0] 256, 256 32) 0 stem_bn[0][0] 256, 256 32) 288 stem 32) 128 block1a pad[0][0] stem bn (BatchNormalization) (None, stem activation (Activation) (None (None, activation[0][0] dwconv[0][0] -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_378.jpg?x=256&y=196&w=1377&h=713&r=0"/>

<!-- Media -->

完成上述步骤后，即可开始模型拟合。此阶段还可便捷地定义回调函数，首当其冲的是ModelCheckpoint：

---

model_save = ModelCheckpoint('./EffNetB0_512_8_best_weights.h5',

save_best_only = True,

save_weights_only = True,

monitor = 'val_loss',

mode = 'min', verbose = 1)

---

该检查点包含几个值得详解的参数：

- 设置save_best_only = True可保留最优模型权重

- 仅保存权重而非完整优化器状态，可减小模型体积

- 通过验证损失最小值确定最优模型

接下来采用防止过拟合的常用方法——早停机制。监测模型在验证集上的表现，若指标连续5个epoch未提升（本例设定值）则终止训练：

---

early_stop = EarlyStopping(监控指标 = 'val_loss', 最小变化量 = 0.001,

耐心值 = 5, 模式 = 'min',

详细输出 = 1, 恢复最佳权重 = True)

---

ReduceLROnPlateau回调函数会监控验证集的损失值，若连续经过指定耐心周期数（此处为2个周期）仍无改善，学习率将降低（本例中降低系数为0.3）。虽然这不是万能解决方案，但往往能有效促进模型收敛：

---

reduce_lr = ReduceLROnPlateau(监控指标 = 'val_loss', 降低系数 = 0.3,

耐心值 = 2, 最小变化量 = 0.001,

模式 = 'min', 详细输出 = 1)

---

现在可以开始训练模型：

---

history = model.fit(   )

train_generator,

每周期步数 = STEPS_PER_EPOCH,

训练周期数 = CFG.EPOCHS,

验证数据 = validation_generator,

验证步数 = VALIDATION_STEPS,

回调函数 = [model_save, early_stop, reduce_lr]

)

---

以下简要说明两个首次出现的参数：

- 训练生成器每个训练周期产生steps_per_epoch个批次。

- 当周期结束时，验证生成器会生成validation_steps个验证批次。

调用model.fit()后的示例输出如下：

---

周期00001：val_loss从inf提升至0.57514，模型已保存至./

EffNetB0_512_8_best_weights.h5

---

模型拟合完成后，可通过最初编写的辅助函数检查样本图像的激活情况。虽然这对模型成功运行并非必需，但有助于了解在顶部应用分类层之前模型提取的特征类型：

---

activation_layer_vis(img_tensor, 0)

---

我们可能会看到如下结果：

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_380.jpg?x=245&y=282&w=1396&h=470&r=0"/>

图10.9：拟合模型的样本激活示例

<!-- Media -->

可通过model.predict()生成预测结果：

---

ss = pd.read_csv(os.path.join(CFG.WORK_DIR, "sample_submission.csv"))

preds = []

for image_id in ss.image_id:

image = Image.open(os.path.join(CFG.WORK_DIR, "test_images",

image_id))

image = image.resize((CFG.TARGET_SIZE, CFG.TARGET_SIZE))

image = np.expand_dims(image, axis = 0)

preds.append(np.argmax(model.predict(image)))

ss['label'] = preds

---

我们通过遍历图像列表构建预测结果。对每张图像，先调整其维度至指定尺寸，再选取信号最强的通道（模型会输出各类别的概率分布，我们通过argmax选取概率最大的类别）。最终预测结果是类别编号，与竞赛采用的评估标准保持一致。

至此我们已演示了图像分类的最小端到端流程。当然还有诸多改进空间——例如增加数据增强、采用更大模型架构、自定义回调函数等——但这个基础模板能为后续开发提供良好起点。

现在我们将转向计算机视觉的第二个热门问题：目标检测。

## 目标检测

目标检测是计算机视觉/图像处理任务，需识别图像或视频中特定类别的语义对象实例。与前一节讨论的分类问题不同（仅需为图像分配类别标签），目标检测任务需要在感兴趣物体周围绘制边界框以定位其位置。

本节将使用全球小麦检测竞赛（https://www.kaggle.com/c/global-wheat-detection）数据。该竞赛要求检测麦穗（即小麦植株顶端含谷粒的穗状结构），通过植物图像中的麦穗检测来估算不同品种小麦的穗粒大小和密度。我们将演示如何使用Yolov5（目标检测领域的成熟模型，在2021年末被YoloX架构超越前保持领先）训练解决方案。Yolov5在该竞赛中表现极具竞争力，虽最终因许可问题被组委会禁用，但仍是本演示的理想选择。

<!-- Media -->

<!-- figureText: 0 0 50 100 150 200 250 0 50 100 150 200 250 50 100 150 200 250 50 100 150 200 250 -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_381.jpg?x=281&y=1088&w=1311&h=622&r=0"/>

图10.10：检测到的麦穗样本图像可视化

<!-- Media -->

开始前需重点说明边界框标注的不同格式：描述矩形坐标存在多种（数学等效但形式不同的）方式。

最常见的有coco、voc-pascal和yolo三种格式，下图清晰展示了它们的区别：

<!-- Media -->

<!-- figureText: COCO voc-pascal yolo [x1,y1,x2,y2] \( \left\lbrack  {x,y,w,h}\right\rbrack \) width height \( x,y \) x2, y2 \( \left\lbrack  {x,y,w,h}\right\rbrack \) \( x,y \) x1, y1 width height -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_382.jpg?x=237&y=329&w=1404&h=422&r=0"/>

图10.11：边界框标注格式对比

<!-- Media -->

还需定义网格结构：Yolo通过在图像上放置网格来检测对象，检查各单元格中是否存在目标对象（本例为麦穗）。边界框会被重塑为相对于所在单元格的偏移量，其(x,y,w,h)参数会缩放至单位区间：

<!-- Media -->

<!-- figureText: width -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_382.jpg?x=630&y=1084&w=625&h=630&r=0"/>

图10.12：Yolo标注定位示意图

<!-- Media -->

我们首先加载训练数据的标注文件：

---

df = pd.read_csv('../input/global-wheat-detection/train.csv')

df.head(3)

---

让我们检查几个样本：

<!-- Media -->

<table><tbody><tr><td></td><td>图像ID</td><td>宽度</td><td>高度</td><td>边界框</td><td>来源</td></tr><tr><td>0</td><td>b6ab77fd7</td><td>1024</td><td>1024</td><td>[834.0, 222.0, 56.0, 36.0]</td><td>usask_1</td></tr><tr><td>1</td><td>b6ab77fd7</td><td>1024</td><td>1024</td><td>[226.0, 548.0, 130.0, 58.0]</td><td>usask_1</td></tr><tr><td>2</td><td>b6ab77fd7</td><td>1024</td><td>1024</td><td>[377.0, 504.0, 74.0, 160.0]</td><td>usask_1</td></tr></tbody></table>

图10.13：带标注的训练数据

<!-- Media -->

我们从bbox列提取边界框的实际坐标：

---

bboxs = np.stack(df['bbox'].apply(lambda x: np.fromstring(x[1:-1],

\[\text{sep=',')))}\]

bboxs

---

查看该数组：

---

array([[834., 222., 56., 36.],

	[226., 548., 130., 58.],

	[377., 504., 74., 160.],

	\( \ldots , \)

	[134., 228., 141., 71.],

	[430., 13., 184., 79.],

	[875., 740., 94., 61.]]]

---

下一步是将Yolo格式的坐标提取到单独的列中：

---

for i, column in enumerate(['x', 'y', 'w', 'h']):

df[column] = bboxs[:,i]

df.drop(columns=['bbox'], inplace=True)

df['x_center'] = df['x'] + df['w']/2

df['y_center'] = df['y'] + df['h']/2

df['classes'] = 0

df = df[['image_id','x', 'y', 'w', 'h','x_center','y_center','classes']]

df.head(3)

---

Ultralytics的实现对数据集结构有特定要求，特别是标注存储位置及训练/验证数据的文件夹结构。

下方代码中创建文件夹的操作相当直观，但鼓励求知欲更强的读者查阅官方文档(https://github.com/ultralytics/yolov5/wiki/Train-Custom-Data)：

#按数据源分层

---

source = 'train'

#为演示选取单个折叠集

fold = 0

val_index = set(df[df['fold'] == fold]['image_id'])

#遍历每张图像的边界框

for name,mini in tqdm(df.groupby('image_id')):

#文件保存路径

if name in val_index:

path2save = 'valid/'

else:

path2save = 'train/'

#标签存储路径

if not os.path.exists('convertor/fold\{\}/labels/'.

format(fold)+path2save):

os.makedirs('convertor/fold\{\}/labels/'.format(fold)+path2save)

with open('convertor/fold\{\}/labels/'.format(fold)+path2save+name+".

txt", 'w+') as f:

#根据Yolo格式要求标准化坐标

row = mini[['classes','x_center','y_center','w','h']].

astype(float).values

row = row/1024

row = row.astype(str)

for j in range(len(row)):

text = ' '.join(row[j])

f.write(text)

f.write("\\n")

if not os.path.exists('convertor/fold\{\}/images/\{\}'.

format(fold,path2save)):

os.makedirs('convertor/fold\{\}/images/\{\}'.format(fold,path2save))

#图像无需预处理 => 批量复制

sh.copy("../input/global-wheat-detection/\{\}/\{\}.jpg".

format(source,name),

'convertor/fold\{\}/images/\{\}/\{\}.jpg'.

format(fold,path2save,name))

---

接下来我们安装Yolo包本身。若在Kaggle Notebook或Colab中运行，请确保已启用GPU；虽然Yolo安装无需GPU也能完成，但CPU与GPU性能差异可能导致各种超时和内存问题。

---

!git clone https://github.com/ultralytics/yolov5 && cd yolov5 &&

pip install -r requirements.txt

---

此处省略冗长的输出日志。最后需要准备YAML配置文件，用于指定训练集/验证集路径和类别数量。我们仅检测麦穗（不区分种类），故设一个类别（名称仅为标记一致性，此处可为任意字符串）：

---

yaml_text = """train: /kaggle/working/convertor/fold0/images/train/

val: /kaggle/working/convertor/fold0/images/valid/

nc: 1

names: ['wheat']"""

with open("wheat.yaml", 'w') as f:

f.write(yaml_text)

%cat wheat.yaml

---

至此，我们可以开始训练模型：

---

!python ./yolov5/train.py --img 512 --batch 2 --epochs 3 --workers 2

----data wheat.yaml --cfg "./yolov5/models/yolov5s.yaml" --name yolov5x_

fold0 --cache

---

除非您习惯使用命令行操作，否则上述命令看起来相当晦涩，让我们详细解析其构成：

- train.py 是用于训练YoloV5模型的核心脚本，从预训练权重开始训练。

- - img 512 表示我们希望将原始图像（如您所见未做任何预处理）缩放至\( {512} \times  {512} \)。要获得有竞争力的结果，应使用更高分辨率，但此代码在Kaggle Notebook中运行，该环境对资源有一定限制。

- - batch 指训练过程中的批次大小。

- - epochs 3 表示模型将训练三个周期。

- - workers 2 指定数据加载器的工作线程数。增加此数值可能提升性能，但6.0版本（本文撰写时Kaggle Docker镜像中的最新版）存在已知缺陷：当工作线程数过高时，即使机器资源充足也会出现问题。

- - data wheat.yaml 指向我们之前定义的数据规范YAML文件。

- - cfg "./yolov5/models/yolov5s.yaml" 指定模型架构及用于初始化的对应权重集。您可使用安装包提供的配置（详见官方文档），也可自定义并保持.yaml格式。

- - name 指定训练结果的存储位置。

下面我们将分解训练命令的输出。首先是基础准备：

<!-- Media -->

---

下载预训练权重，设置Weights&Biases https://

wandb.ai/site集成，执行GitHub完整性检查。

正在下载 https://ultralytics.com/assets/Arial.ttf 至 /root/.config/

Ultralytics/Arial.ttf...

wandb: (1) 创建W&B账户

wandb: (2) 使用现有W&B账户

wandb: (3) 不可视化我的结果

wandb: 输入您的选择：(30秒超时)

wandb: 由于登录超时，W&B功能已禁用。

训练配置：权重=yolov5/yolov5s.pt，配置文件=./yolov5/models/yolov5s.yaml，

数据=wheat.yaml，超参数=yolov5/data/hyps/hyp.scratch-low.yaml，训练轮数=3，

批次大小=2，图像尺寸=512，矩形训练=False，恢复训练=False，不保存=False，

无验证=False，自动锚点=False，进化=None，存储桶=，缓存=内存，

图像加权=False，设备=，多尺度=False，单类别=False，

优化器=SGD，同步BN=False，工作进程=2，项目目录=yolov5/runs/train，

名称=yolov5x_fold0，允许覆盖=False，四倍=False，余弦学习率=False，标签

平滑=0.0，早停耐心=100，冻结层=[0]，保存周期=-1，本地排名=-1，

实体=None，上传数据集=False，边界框间隔=-1，模型别名=latest

---

---

github: 与https://github.com/ultralytics/yolov5保持同步

YOLOv5 & v6.1-76-gc94736a torch 1.9.1 CUDA:0 (Tesla P100-PCIE-16GB,

16281MiB)

超参数：学习率lr0=0.01，最终学习率lrf=0.01，动量=0.937，权重衰减=0.0005,

预热周期=3.0，预热动量=0.8，预热偏置学习率=0.1，框损失权重=0.05,

分类损失=0.5，分类正样本权重=1.0，目标损失=1.0，目标正样本权重=1.0，IoU阈值=0.2，锚框阈值=4.0，

焦距损失gamma=0.0，HSV色调增强=0.015，HSV饱和度增强=0.7，HSV明度增强=0.4，旋转角度=0.0，平移=0.1,

缩放=0.5，剪切=0.0，透视=0.0，垂直翻转=0.0，水平翻转=0.5，马赛克增强=1.0,

混合增强=0.0，复制粘贴增强=0.0

Weights & Biases：运行'pip install wandb'以自动跟踪并

可视化YOLOv5训练过程（推荐）

TensorBoard：使用'tensorboard --logdir yolov5/runs/train'启动，查看地址

http://localhost:6006/

正在下载 https://github.com/ultralytics/yolov5/releases/download/v6.1/

yolov5s.pt 至 yolov5/yolov5s.pt...

100% 14.1M/14.1M [00:00<00:00,

40.7MB/s \( \rbrack \)

---

<!-- Media -->

随后加载模型。我们将看到架构摘要、优化器配置及所用数据增强方案：

<!-- Media -->

---

将model.yaml中的nc=80覆盖为nc=1

参数

0 -1 1 3520 models.common. Conv

\( \left\lbrack  {3,{32},6,2,2}\right\rbrack \)

1 -1 1 18560 models.common. Conv

[32, 64, 3, 2]

	2

\( \left\lbrack  {{64},{64},1}\right\rbrack \)

	3

\( \left\lbrack  {{64},{128},3,2}\right\rbrack \)

4 -1 2 115712 models.common.C3

\( \left\lbrack  {{128},{128},2}\right\rbrack \)

	5

[128, 256, 3, 2]

---

<table><tbody><tr><td>6 -1 [256] 256, 3] -1 -1 -1 -1 -1 [-1, 6] -1 -1 -1 [-1,4] -1 -1 - 1 -1 -1</td><td>3</td><td>625152</td><td>模型通用组件.C3模块</td></tr><tr><td>7 [256,512,3, 2]</td><td>1</td><td>1180672</td><td>模型通用组件.卷积层</td></tr><tr><td>8 [512,512,1]</td><td>1</td><td>1182720</td><td>模型通用组件.C3模块</td></tr><tr><td>9</td><td>1</td><td>656896</td><td>模型通用组件.空间金字塔快速池化(SPPF)</td></tr><tr><td>[512, 512, 5 5] 10 [512]1, 1]</td><td>1</td><td>131584</td><td>模型通用组件.卷积层</td></tr><tr><td>11 [空值, 2, '最近邻插值']</td><td>1</td><td>0</td><td>torch.nn模块.上采样层</td></tr><tr><td>12 [1]</td><td>1</td><td>0</td><td>模型通用组件.拼接层</td></tr><tr><td>13 [512, 256, 1, 关闭]</td><td>1</td><td>361984</td><td>模型通用组件.C3模块</td></tr><tr><td>14 1, 1]</td><td>1</td><td>33024</td><td>模型通用组件.卷积层</td></tr><tr><td>15</td><td>1</td><td>0</td><td>torch.nn模块.上采样层</td></tr><tr><td>16 [1]</td><td>1</td><td>0</td><td>模型通用组件.拼接层</td></tr><tr><td>17 [256]</td><td>1</td><td>90880</td><td>模型通用组件.C3模块</td></tr><tr><td>18 [128]</td><td>1</td><td>147712</td><td>模型通用组件.卷积层</td></tr><tr><td>19 [-1, 14] [1]</td><td>1</td><td>0</td><td>模型通用组件.拼接层</td></tr><tr><td>20 256,256, 1, 关闭]</td><td>1</td><td>296448</td><td>模型通用组件.C3模块</td></tr><tr><td>21 [256]256, 3, 2]</td><td>1</td><td>590336</td><td>模型通用组件.卷积层</td></tr><tr><td>22 [-1, 10] [1]</td><td>1</td><td></td><td>模型通用组件.拼接层</td></tr><tr><td>23 [512,512, 1, 关闭]</td><td>1</td><td>1182720</td><td>模型通用组件.C3模块</td></tr><tr><td>2417, 20, 23]</td><td>1</td><td>16182</td><td>模型.YOLO检测层</td></tr></tbody></table>

\( \left\lbrack  {1,\left\lbrack  {\lbrack {10},{13},{16},{30},{33},{23}}\right\rbrack  ,\left\lbrack  {{30},{61},{62},{45},{59},{119}}\right\rbrack  ,\left\lbrack  {{116},{90},{156}}\right\rbrack  }\right\rbrack \) 198, 373, 326]], [128, 256, 512]]

<!-- Media -->

<!-- Media -->

YOLOv5s模型概要：270层网络结构，7,022,326个参数，7,022,326个梯度值，15.8

GFLOPS

从yolov5/yolov5s.pt迁移了342/349个项目

已调整权重衰减系数\( = {0.0005} \)

优化器：采用SGD算法，参数分组为57个权重（无衰减）、60个权重、60个

偏置项

图像增强：模糊处理（非强制应用，概率0.01，模糊范围(3,7)）

中值模糊（非强制应用，概率0.01，模糊范围(3,7)），灰度化（非强制

应用，概率0.01），CLAHE增强（非强制应用，概率0.01，对比度限制(1,

4.0)，网格尺寸(8,8)）

训练集：正在扫描'/kaggle/working/convertor/fold0/labels/train'目录的图片与

标签

训练集：已创建新缓存：/kaggle/working/convertor/fold0/labels/train.

cache

训练集：缓存图片中（内存占用0.0GB）：100%L _____L_____

76.00次/

验证集：正在扫描'/kaggle/working/convertor/fold0/labels/valid'目录的图片与

标签..

验证集：新建缓存路径：/kaggle/working/convertor/fold0/labels/valid.cache

总计：缓存图像处理中(2,668,mm)：1018% | 3,222/3322，108.47/018.47/018.60

70.51i

正在将标签绘制到 yolov5/runs/train/yolov5x_fold0/labels.jpg...

自动锚点：每个目标6.00个锚点，0.997最佳可能召回率(BPR)。当前

锚点与数据集匹配良好

图像尺寸 训练512，验证512

使用2个数据加载工作线程

<!-- Media -->

后续为实际训练日志：可查看训练和验证阶段结果，这些数据存储在./yolov5/runs/train/yolov5x_fold0目录下：

<!-- Media -->

开始3个epoch的训练...

轮次 GPU显存 边界框 目标 类别 标签数

0.371G 0.1196 0.05478 0 14 100%

精确率 平均精度@.5 平均精度@警告：NMS时间限制0.120秒已超时

精确率 平均精度@.5 平均精度@

总计 3322 147409 0.00774 0.0523

0.00437 3.000952

轮次 GPU显存 边界框 目标 类别 标签数 图像尺寸

1/2 0.474G 0.1176 0.05625 0 5 512:

100%

类别 图像数 标签数 精确率 召回率

mAP@.5 0.120s 已超限

类别 图像数 标签数 精确率 召回率

5 mAP@警告：非极大抑制时间超限

类别 图像数 标签数 精确率 召回率

mAP@.5 mAP@

全部 3322 147409 0.00914 0.0618

0.00493 0.00108

训练轮次 显存占用 边界框 目标检测 分类 标签数

2/2 0.474G 0.1146 0.06308 0 12 512:

100%

类别 图像数 标签数 精确率 召回率

mAP@.5 mAP@

全部 3322 147409 0.00997 0.0674

0.00558 0.00123 3个训练轮次已完成，耗时0.073小时。优化器已从yolov5/runs/train/yolov5x_fold0/weights/last.pt移除，14.4MB

优化器已从yolov5/runs/train/yolov5x_fold0/weights/best.pt移除

14.4MB

正在验证yolov5/runs/train/yolov5x_fold0/weights/best.pt...结果已保存至yolov5/runs/train/yolov5x_fold0

<table><tbody><tr><td>融合层中... 类别mAP@.5 mAP@警告：非极大值抑制 类别mAP@.5 mAP@警告：非极大值抑制 类别mAP@.5 mAP@警告：非极大值抑制 类别mAP@.5 mAP@警告：非极大值抑制 类别mAP@.5 mAP@警告：非极大值抑制 类别mAP@.5 mAP@警告：非极大值抑制 类别mAP@.5 mAP@警告：非极大值抑制 类别mAP@.5 mAP@警告：非极大值抑制 类别mAP@.5 mAP@警告：非极大值抑制 类别mAP@.5 mAP@警告：非极大值抑制 类别mAP@.5 mAP@全部 0.005560.00122</td><td>7012822张图像 时间限制 图像时间限制 图像时间限制 图像时间限制 图像时间限制 图像时间限制 图像时间限制 图像时间限制 图像时间限制 图像时间限制 图像3322</td><td>参数，0梯度，标签P 0.120秒超限 标签P 0.120秒超限 标签P 0.120秒超限 标签P 0.120秒超限 标签P 0.120秒超限 标签P 0.120秒超限 标签P 0.120秒超限 标签P 0.120秒超限 标签P 0.120秒超限 标签P 0.120秒超限 标签P 1474090.00997</td><td>15.8千兆浮点运算 R R R R R R R R R R R 0.0673</td></tr></tbody></table>

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_392.jpg?x=365&y=339&w=1160&h=1157&r=0"/>

图10.14：带标注的验证数据

<!-- Media -->

模型训练完成后，我们可以使用性能最佳模型的权重（Yolov5具有自动保存最优和最终周期模型的功能，分别存储为best.pt和last.pt）对测试数据进行预测：

---

!python ./yolov5/detect.py --weights ./yolov5/runs/train/yolov5x_fold0/

weights/best.pt --img 512 --conf 0.1 --source /kaggle/input/global-wheat-

detection/test --save-txt --save-conf --exist-ok

---

我们将讨论推理阶段特有的参数：

- - weights指向上述训练模型中最佳权重的存储路径

- - conf 0.1指定模型生成的候选边界框保留阈值。这始终是精确率与召回率的权衡（阈值过低会导致大量误检，而阈值过高可能导致完全检测不到麦穗）

- - source是测试数据的存储位置

可在本地查看为测试图像生成的标签：

---

!ls ./yolov5/runs/detect/exp/labels/

---

可能显示如下内容：

---

2fd875eaa.txt 53f253011.txt aac893a91.txt f5a1f0358.txt

348a992bb.txt 796707dd7.txt cc3532ff6.txt

---

查看单个预测结果示例：

---

!cat 2fd875eaa.txt

---

其格式如下：

---

	0 0.527832 0.580566 0.202148 0.838867 0.101574

0 0.894531 0.587891 0.210938 0.316406 0.113519

---

这意味着在图像2fd875eaa中，我们训练好的模型检测到两个边界框（其坐标对应行内第2-5项），行末给出了置信度分数超过0.1的结果。

如何将预测结果合并成规定格式的提交文件？我们首先定义一个辅助函数，用于将坐标从yolo格式转换为coco格式（本次比赛要求）：只需简单调整顺序，并通过乘以图像尺寸将分数值归一化到原始取值范围：

---

def convert(s):

x = int(1024 * (s[1] - s[3]/2))

y = int(1024 * (s[2] - s[4]/2))

w = int(1024 * s[3])

h = int(1024 * s[4])

return(str(s[5]) + ' ' + str(x) + ' ' + str(y) + ' ' + str(w)

+ ' ' + str(h))

---

接着我们生成提交文件：

1. 遍历上述列出的文件

2. 每个文件的所有行都转换为规定格式的字符串（每行代表检测到的一个边界框）

3. 将这些行拼接成该文件对应的单个字符串

代码如下：

---

with open('submission.csv', 'w') as myfile:

##准备提交文件

wfolder = './yolov5/runs/detect/exp/labels/'

for f in os.listdir( wfolder ) :

fname = wfolder + f

xdat = pd.read_csv(fname, sep = ' ', header = None)

outline = f[:-4] + ' ' + ' '.join(list(xdat.apply(lambda s:

convert(s), axis = 1)))

myfile.write(outline + '\\n')

myfile.close(   )

---

让我们看看效果：

<!-- Media -->

---

!cat submission.csv

	\( \left\lbrack  \begin{matrix} {53} \\  f \\  {25} \\  {30} \\  {11} \end{matrix}\right\rbrack  \left\lbrack  \begin{matrix} {0.1004} & & & & \\  {72} & {61} & {669} & {961} & {57} \end{matrix}\right\rbrack  \left\lbrack  \begin{matrix} {0.1062} & & & & & & & & \\  {23} & 0 & {125} & {234} & {183} & {0.1082} & {96} & {696} & {928} \end{matrix}\right\rbrack \)

\( \begin{array}{llllllllllllllll} {126} & {0.108863} & {515} & {393} & {86} & {161} & {0.11459} & {31} & 0 & {167} & {209} & {0.120246} & {517} & {466} & {89} & {147} \end{array} \)

aac893a91 0.108037 376 435 325 188

796707dd7 0.235373 684 128 234 113

	\( \begin{matrix}  & {cc} & {35} & {32} \\  {ff6} & {0.100} & {443} & {406} \\  \;{752} & {144} & {108} & {0.102} \\  {479} & {405} & {87} & 4 \\  \;{89} & {0.107} & {173} & {576} \\  \;{537} & & &  \end{matrix} \)

		\( \left\lbrack  \begin{matrix} {138} & {94} & {0.11345} \\  9 & {256} & {498} \end{matrix}\right\rbrack  \left\lbrack  \begin{matrix} {179} & {211} & {0.11484} \\  7 & {836} & {618} \end{matrix}\right\rbrack  \left\lbrack  \begin{matrix} {186} & {65} & {0.12112} \\  1 & {154} & {544} \end{matrix}\right\rbrack \)

	248 115 0.125105 40 567 483 199

2fd875eaa 0.101398 439 163 204 860 0.112546 807 440 216 323

348a992bb 0.100572 0 10 440 298 0.101236 344 445 401 211

f5a1f0358 0.102549 398 424 295 96

---

<!-- Media -->

生成的submission.csv文件标志着我们流程的完成。

本节我们演示了如何运用YoloV5解决目标检测问题：处理不同格式的标注数据、针对特定任务定制模型、训练模型及评估结果。

基于这些知识，您应当能够着手处理目标检测问题。

现在我们将转向计算机视觉第三大类任务：语义分割。

## 语义分割

理解分割最直观的方式是：它对图像中每个像素进行分类，将其归入对应类别；这些像素共同构成感兴趣区域，例如医学影像中器官的病变区域。相比之下，目标检测（前文所述）将图像区块分类为不同物体类别，并生成其边界框。

我们将使用Sartorius细胞实例分割竞赛数据（https://www.kaggle.com/c/sartorius-cell-instance-segmentation）演示建模方法。该竞赛要求参赛者利用显微图像集训练神经细胞实例分割模型。

我们的解决方案将基于Detectron2构建，这是Facebook AI Research开发的库，支持多种检测与分割算法。

Detectron2是原始Detectron库（https://github.com/ facebookresearch/Detectron/）和Mask R-CNN项目（https://github.com/facebookresearch/maskrcnn-benchmark/）的继承者。首先安装额外包：

---

!pip install pycocotools

!pip install 'git+https://github.com/facebookresearch/detectron2.git'

---

安装pycocotools（https://github.com/cocodataset/cocoapi/tree/master/PythonAPI/ pycocotools）用于格式化标注数据，以及本任务的核心工具Detectron2（https://github.com/facebookresearch/detectron2）。

训练模型前需进行预处理：将主办方提供的游程编码（RLE）格式标注转换为Detectron2所需的COCO格式。RLE的核心思想是空间压缩：通过特定方式标记像素组来创建分割。由于图像可视为数组，该区域可用系列直线（行向或列向）表示。

可通过列出索引或指定起始位置及连续块长度来编码每条直线。示例如下：

<!-- Media -->

<!-- figureText: top 0 8 16 24 32 40 48 56 64 72 33 41 49 57 65 73 34 42 50 58 66 74 35 43 51 59 67 75 36 44 52 60 68 76 37 45 53 61 69 77 38 46 54 62 70 78 39 47 63 71 79 right 1 9 17 25 2 10 18 26 3 11 19 27 4 12 20 28 5 13 21 6 14 22 30 7 15 23 31 bottom left -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_396.jpg?x=404&y=344&w=1061&h=853&r=0"/>

图10.15：RLE可视化示意图

<!-- Media -->

微软通用上下文对象（COCO）格式是规定图像数据集标签与元数据存储方式的特定JSON结构。接下来我们将演示如何将RLE转换为COCO格式，并结合\( k \)折交叉验证拆分，从而为每折生成所需的训练/验证JSON文件对。

## 开始：

---

#从pycocotools.coco导入COCO

导入skimage.io为io

导入matplotlib.pyplot为plt

从pathlib导入Path

从PIL导入Image

导入pandas为pd

导入numpy为np

从tqdm.notebook导入tqdm

导入json,itertools

从sklearn.model_selection导入GroupKFold

#配置

类配置:

数据路径 = '../input/sartorius-cell-instance-segmentation/'

折叠数 = 5

---

我们需要三个函数来实现从RLE到COCO的转换。首先，需要将RLE转换为二进制掩码：

---

#源自 https://www.kaggle.com/stainsby/fast-tested-rle

def rle_decode(mask_rle, shape):

	...

mask_rle: 以字符串格式表示的游程编码（起始位置 长度）

shape: 返回数组的（高度，宽度）维度

返回numpy数组，1代表掩码区域，0代表背景

	...

s = mask_rle.split(   )

starts, lengths = [np.asarray(x, dtype=int)

for x in (s[0:][::2], s[1:][::2])]

starts -= 1

ends = starts + lengths

img = np.zeros(shape[0]*shape[1], dtype=np.uint8)

for lo, hi in zip(starts, ends):

img[lo:hi] = 1

return img.reshape(shape) # 需对齐RLE方向

---

## 第二个函数将二值掩码转换为RLE：

---

#源自 https://newbedev.com/encode-numpy-array-using-uncompressed-rle-for-

#COCO数据集

def 二进制掩码转游程编码(binary_mask):

游程编码 = {'counts': [], 'size': list(binary_mask.shape)}

计数 = 游程编码.get('counts')

for i, (值, 元素) in enumerate(   )

itertools.groupby(binary_mask.ravel(order='F'))):

if i == 0 and 值 == 1:

计数.append(0)

计数.append(len(list(元素)))

return 游程编码

---

最后将两者结合生成COCO格式输出：

---

def 构建COCO结构(train_df):

类别ID = {名称: id+1 for id, 名称 in enumerate(   )

train_df.cell_type.unique(   ))}

类别 = [{'name': 名称, 'id': id} for 名称, id in 类别ID.items(   )]

图像 = [{'id': id, 'width': 行.width, 'height': 行.height,

'文件名':f'train/\{id\}.png'\} 用于id,

行在train_df.groupby('id').agg('first').iterrows(   )]

标注列表 = []

对于idx, 行在tqdm(train_df.iterrows(   ))中:

mk = rle解码(行.标注, (行.高度, 行.宽度))

ys, xs = np.非零位置(mk)

x1, x2 = 最小值(xs), 最大值(xs)

y1, y2 = 最小值(ys), 最大值(ys)

enc =二值掩码转rle(mk)

分割 = \{

'分割区域':enc,

'边界框': [整型(x1), 整型(y1), 整型(x2-x1+1), 整型(y2-y1+1)],

'面积': 整型(np.求和(mk)),

'图像id':行.id,

'类别id':类别id映射[行.细胞类型],

'是否拥挤':0,

'id':索引

			\}

标注列表追加(分段)

返回{'类别':分类, '图像':图像集,'标注':标注列表}

---

我们将数据划分为互不重叠的折：

---

训练数据框 = 读取csv文件(配置.数据路径 + '训练集.csv')

分组折分器 = 组折分(折数 = 配置.折数)

训练数据框["折号"] = -1

目标值 = 训练数据框.宽度值

for 折号, (训练集_, 验证集_) in 枚举(分组折分器.划分(X=训练数据框, y=目标值,

分组=训练数据框.id值)):

训练数据框.定位[验证集_, "折号"] = 折号

折号 = 训练数据框.折号.复制(   )

---

现在可以遍历各折数据：

---

所有id = 训练数据框.id.去重(   )

#for 折 in 范围(配置.折数):

for 折 in 范围(4,5):

训练样本 = 训练数据框.loc[折叠标识 != 当前折叠]

根节点 = coco结构(训练样本)

以写入模式打开('训练集标注_f' + str(当前折叠) +

'.json', 'w', encoding='utf-8') 文件对象:

json导出(根节点, 文件对象, 确保ascii=True, 缩进=4)

验证样本 = 训练数据框.loc[折叠标识 == 当前折叠]

print('折叠 ' + str(当前折叠) + ': 已生成')

循环范围 (4,5):

训练样本 = 训练数据框.loc[折叠标识 == 当前折叠]

根节点 = coco结构(训练样本)

以写入模式打开('验证集标注_f' + str(当前折叠) +

'.json', 'w', encoding='utf-8') 文件对象:

json导出(根节点, 文件对象, 确保ascii=True, 缩进=4)

验证样本 = 训练数据框.loc[折叠标识 == 当前折叠]

print('折叠 ' + str(当前折叠) + ': 已生成')

---

必须分段执行循环的原因是Kaggle环境的大小限制：笔记本输出的最大尺寸被限制在\( {20}\mathrm{\;{GB}} \)，而5折交叉验证每组产生2个文件（训练/验证）意味着总共10个JSON文件，会超出该限制。在Kaggle笔记本中运行代码时，这类实际考量值得注意，当然对于此类"准备性"工作，您也可以在其他环境生成结果后，以Kaggle数据集形式上传。

数据集划分完成后，我们可以着手为数据集训练一个Detectron2模型。如

往常一样，我们首先加载必要的包：

---

from datetime import datetime

import os

import pandas as pd

import numpy as np

import pycocotools.mask as mask_util

import detectron2

from pathlib import Path

import random, cv2, os

import matplotlib.pyplot as plt

#导入一些常用的detectron2工具

from detectron2 import model_zoo

from detectron2.engine import DefaultPredictor, DefaultTrainer

from detectron2.config import get_cfg

from detectron2.utils.visualizer import Visualizer, ColorMode

从detectron2.data导入MetadataCatalog（元数据目录）、DatasetCatalog（数据集目录）

从detectron2.data.datasets导入register_coco_instances（注册COCO实例）

从detectron2.utils.logger导入setup_logger（设置日志器）

从detectron2.evaluation.evaluator导入DatasetEvaluator（数据集评估器）

从detectron2.engine导入BestCheckpointer（最佳检查点）

从detectron2.checkpoint导入DetectionCheckpointer（检测检查点）

setup_logger(   )

导入torch（PyTorch）

---

虽然Detectron2的导入数量起初令人望而生畏，但随着任务定义的推进，它们的功能将逐渐明晰；我们首先指定输入数据文件夹、标注文件夹的路径，以及定义首选模型架构的YAML文件：

---

class CFG（配置类）:

wfold = 4

data_folder = '../input/sartorius-cell-instance-segmentation/'（数据文件夹路径）

anno_folder = '../input/sartoriusannotations/'（标注文件夹路径）

model_arch = 'mask_rcnn_R_50_FPN_3x.yaml'（模型架构文件）

nof_iters = 10000（迭代次数）

seed = 45（随机种子）

---

此处值得提及的是迭代次数参数（即上文的nof_iters）。通常模型训练以epoch（完整遍历训练数据的次数）作为参数单位，但Detectron2采用了不同设计：一次迭代对应一个迷你批次，且模型不同部分会使用不同规模的迷你批次。

为确保结果可复现，我们固定了模型各组件使用的随机种子：

---

def seed_everything(seed):

random.seed(seed)

os.environ['PYTHONHASHSEED'] = str(seed)

np.random.seed(seed)

torch.manual_seed(seed)

torch.cuda.manual_seed(seed)

torch.backends.cudnn.deterministic = True

seed_everything(CFG.seed)

---

竞赛指标采用不同交并比(IoU)阈值下的平均精度均值(mAP)。回顾第5章"竞赛任务与指标"可知，某组提议目标像素与真实目标像素的IoU计算公式为：

\[\operatorname{IoU}\left( {A,B}\right)  = A \cap  B/A \cup  B\]

该指标扫描一系列IoU阈值（从0.5到0.95，步长0.05），在每个阈值点计算平均精度值。

每个阈值下，通过比较预测目标与所有真实目标，根据真阳性(TP)、假阴性(FN)和假阳性(FP)数量计算精度值。最终竞赛指标返回的分数是测试数据集每张图像单独平均精度的均值。

下文定义计算该指标所需的函数，并将其直接作为目标函数用于模型内部：

---

#引自https://www.kaggle.com/theoviel/competition-metric-map-iou

def precision_at(threshold, iou):

匹配项 = 交并比 > 阈值

真阳性 = np.sum(匹配项, axis=1) == 1 # 正确检测对象

假阳性 = np.sum(匹配项, axis=0) == 0 # 漏检对象

假阴性 = np.sum(匹配项, axis=1) == 0 # 误检对象

return np.sum(真阳性), np.sum(假阳性),

np.sum(假阴性)

def 评分(预测, 目标):

预测掩码 = 预测['实例'].预测掩码.cpu(   ).numpy(   )

编码预测 = [掩码工具.encode(np.asarray(p, order='F'))

for p in 预测掩码]

编码目标 = list(map(lambda x:x['分割'], 目标))

交并比 = 掩码工具.iou(编码预测, 编码目标, [0]*len(编码目标))

精度 = []

for \( t \) in np.arange(0.5,1.0,0.05):

tp, fp, fn = 精度计算(t, 交并比)

精度 = tp / (tp + fp + fn)

prec.append(p)

return np.mean(prec)

---

定义完该指标后，我们可以在模型中使用它：

---

class MAPIOUEvaluator(DatasetEvaluator):

def _init_(self, dataset_name):

dataset_dicts = DatasetCatalog.get(dataset_name)

self.annotations_cache = \{item['image_id']:item['annotations']

for item in dataset_dicts\}

def reset(self):

self.scores = []

def process(self, inputs, outputs):

for inp, out in zip(inputs, outputs):

if len(out['instances']) == 0:

self.scores.append(0)

else:

targ = self.annotations_cache[inp['image_id']]

self.scores.append(score(out, targ))

def evaluate(self):

return \{"MaP IoU": np.mean(self.scores)\}

---

这为我们创建Trainer对象奠定了基础，该对象是我们基于Detectron2构建解决方案的核心：

---

class Trainer(DefaultTrainer):

@classmethod

def build_evaluator(cls, cfg, dataset_name, output_folder=None):

return MAPIOUEvaluator(dataset_name)

def build_hooks(self):

#复制cfg配置

cfg = self.cfg.clone(   )

#构建原始模型钩子

hooks = super(   ).build_hooks(   )

#添加最佳检查点钩子

hooks.insert(-1, BestCheckpointer(cfg.TEST.EVAL_PERIOD,

DetectionCheckpointer(self.model,

cfg.OUTPUT_DIR),

"平均精度交并比(MaP IoU)",

"最大值",

											))

return hooks

---

现在我们将以Detectron2框架的方式加载训练/验证数据：

---

dataDir=Path(CFG.data_folder)

register_coco_instances('sartorius_train',\{\}, CFG.anno_folder +

'annotations_train_f' + str(CFG.wfold) +

'.json', dataDir)

register_coco_instances('sartorius_val',\{\}, CFG.anno_folder +

'annotations_valid_f' + str(CFG.wfold) +

'.json', dataDir)

metadata = MetadataCatalog.get('sartorius_train')

train_ds = DatasetCatalog.get('sartorius_train')

---

在实例化Detectron2模型前，需完成配置工作。多数参数可保留默认值（至少首次运行时）；如需调优，建议从BATCH_SIZE_PER_IMAGE（提升泛化性能）和SCORE_THRESH_TEST（降低误检率）开始调整：

---

cfg = get_cfg(   )

cfg.INPUT.MASK_FORMAT='位掩码'

cfg.merge_from_file(model_zoo.get_config_file('COCO-实例分割/' +

CFG.model_arch))

cfg.DATASETS.TRAIN = ("萨托利乌斯训练集",)

cfg.DATASETS.TEST = ("萨托利乌斯验证集",)

cfg.DATALOADER.NUM_WORKERS = 2

cfg.MODEL.WEIGHTS = model_zoo.get_checkpoint_url('COCO-实例分割/'

+ CFG.model_arch)

cfg.SOLVER.IMS_PER_BATCH = 2

cfg.SOLVER.BASE_LR = 0.001

cfg.SOLVER.MAX_ITER = CFG.nof_iters

cfg.SOLVER.STEPS = []

cfg.MODEL.ROI_HEADS.BATCH_SIZE_PER_IMAGE = 512

cfg.MODEL.ROI_HEADS.NUM_CLASSES = 3

cfg.MODEL.ROI_HEADS.SCORE_THRESH_TEST = .4

cfg.TEST.EVAL_PERIOD = len(DatasetCatalog.get('萨托利乌斯训练集'))

// cfg.SOLVER.IMS_PER_BATCH

---

训练模型的操作流程如下：

---

os.makedirs(cfg.OUTPUT_DIR, exist_ok=True)

trainer = Trainer(cfg)

trainer.resume_or_load(resume=False)

trainer.train(   )

---

您会注意到训练过程中输出的信息详细记录了整个流程的进展：

<!-- Media -->

<!-- figureText: [01/06 22:26:36 d2.data.datasets.coco]: Loading ../input/sartorius-annotations/annotations_t rain_f4.json takes 1.16 seconds. [01/06 22:26:36 d2.data.datasets.coco]: Loaded 485 images in COCO format from .../input/sartc rius-annotations/annotations_train_f4.json [01/06 22:26:38 d2.data.build]: Removed 0 images with no usable annotations. 485 images lef t. [01/06 22:26:38 d2.data.build]: Distribution of instances among all 3 categories: category | #instances | category | #instances | category | #instances | :------------- | :------------- | :----------- : | :------------- | :---------- : | :---------- [01/06 22:26:38 d2.data.dataset_mapper]: [DatasetMapper] Augmentations used in training: [Re sizeShortestEdge(short_edge_length=(640, 672, 704, 736, 768, 800), max_size=1333, sample_sty le='choice'), RandomFlip(   )] [01/06 22:26:38 d2.data.build]: Using training sampler TrainingSampler [01/06 22:26:38 d2.data.common]: Serializing 485 elements to byte tensors and concatenating them all ... [01/06 22:26:38 d2.data.common]: Serialized dataset takes 6.79 MiB model_final_f10217.pkl: 178MB [00:04, 35.8MB/s] -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_405.jpg?x=246&y=335&w=1395&h=914&r=0"/>

图10.16：Detectron2的训练输出示例

<!-- Media -->

模型训练完成后，我们可以保存权重并用于推理（可能是在另一个Notebook中——参见本章前面的讨论）以及提交准备。首先添加新参数来规范预测，设置置信度阈值和最小掩码尺寸：

---

THRESHOLDS = [.18, .35, .58]

MIN_PIXELS = [75, 150, 75]

---

我们需要一个辅助函数将单个掩码编码为RLE格式：

---

def rle_encode(img):

	...

img: numpy数组, 1 - 掩码, 0 - 背景

返回格式化后的游程编码字符串

	...

pixels = img.flatten(   )

像素数组 = np.concatenate([[0], 像素数组, [0]])

游程 = np.where(像素数组[1:] != 像素数组[:-1])[0] + 1

游程[1::2] -= 游程[::2]

return ' '.join(str(x) for x in 游程)

---

以下是生成每张图像所有掩模的主函数，会过滤掉置信度低于阈值(THRESHOLDS)且面积过小(像素数少于MIN_PIXELS)的不可靠掩模：

---

def 获取掩模(文件名, 预测器):

图像 = cv2.imread(str(文件名))

预测结果 = 预测器(图像)

预测类别 = torch.mode(预测结果['instances'].pred_classes)[0]

有效索引 = 预测结果['instances'].scores >= 阈值表[预测类别]

预测掩模 = 预测结果['instances'].pred_masks[有效索引]

预测掩模 = 预测掩模.cpu(   ).numpy(   )

结果列表 = []

已用区域 = np.zeros(图像.shape[:2], dtype=int)

for 掩模 in 预测掩模:

掩模 = 掩模 * (1-已用区域)

#跳过面积过小的预测区域

if mask.sum(   ) >= MIN_PIXELS[pred_class]:

used += mask

res.append(rle_encode(mask))

return res

---

随后我们初始化存储图像ID和掩码的列表：

---

dataDir=Path(CFG.data_folder)

ids, masks=[],[]

test_names = (dataDir/'test').ls(   )

---

处理大规模图像集的竞赛——如本节讨论的案例——通常需要超过9小时的模型训练时间，这已超出代码竞赛的时限要求（参见https://www.kaggle.com/docs/competitions）。这意味着无法在同一个Notebook中完成模型训练和推理。常规解决方案是先在Kaggle、Google Colab、GCP或本地环境中运行训练Notebook/脚本作为独立流程，然后将首个Notebook的输出（训练好的权重）作为第二个Notebook的输入，即用于定义预测模型。

我们按照此方式加载训练好的模型权重：

---

cfg = get_cfg(   )

cfg.merge_from_file(model_zoo.get_config_file("COCO-InstanceSegmentation/"+

CFG.arch+".yaml"))

cfg.INPUT.MASK_FORMAT = 'bitmask'

cfg.MODEL.ROI_HEADS.NUM_CLASSES = 3

cfg.MODEL.WEIGHTS = CFG.model_folder + 'model_best_f' +

str(CFG.wfold)+'.pth'

cfg.MODEL.ROI_HEADS.SCORE_THRESH_TEST = 0.5

cfg.TEST.DETECTIONS_PER_IMAGE = 1000

predictor = DefaultPredictor(cfg)

---

我们可以可视化部分预测结果：

---

encoded_masks = get_masks(test_names[0], predictor)

_, axs = plt.subplots(1,2, figsize = (40, 15))

axs[1].imshow(cv2.imread(str(test_names[0])))

for enc in encoded_masks:

dec = rle_decode(enc)

axs[0].imshow(np.ma.masked_where(dec == 0, dec))

---

示例如下：

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_407.jpg?x=242&y=1349&w=1391&h=501&r=0"/>

图10.17：将Detectron2的样本预测结果与源图像并排可视化

<!-- Media -->

利用上述定义的辅助函数，生成用于提交的RLE格式掩码十分简便：

---

for fn in test_names:

encoded_masks = 获取掩码(fn, predictor)

for enc in 编码后的掩码:

ids.append(文件名主干)

掩码列表.append(编码)

数据框 = pd.DataFrame({'id':编号列表, 'predicted':预测掩码}).输出为csv('提交文件.csv',

索引=False)

pd.读取csv('提交文件.csv').头部(   )

---

以下是最终提交文件的前几行：

<!-- Media -->

<table><tbody><tr><td></td><td>标识符</td><td>预测值</td></tr><tr><td>0</td><td>7ae19de7bc2a</td><td>139541 4 140244 7 140948 8 141652 8 142356 9 1...</td></tr><tr><td>1</td><td>7ae19de7bc2a</td><td>96418 4 97121 6 97825 7 98529 8 99233 8 99937...</td></tr><tr><td>2</td><td>7ae19de7bc2a</td><td>26627 14 27329 17 28031 19 28733 21 29435 23 3...</td></tr><tr><td>3</td><td>7ae19de7bc2a</td><td>148230 2 148931 6 149633 9 150336 11 151039 13…</td></tr><tr><td>4</td><td>7ae19de7bc2a</td><td>224918 2 225620 7 226324 9 227027 12 227731 13…</td></tr></tbody></table>

图10.18：经过训练的Detectron2模型生成的格式化提交结果

<!-- Media -->

本节内容到此结束。上述流程展示了如何搭建语义分割模型并进行训练。我们使用了较少的迭代次数，但要获得具有竞争力的结果，需要更长时间的训练。

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_408.jpg?x=240&y=1623&w=360&h=364&r=0"/>

<!-- Media -->

## 劳拉·芬克

https://www.kaggle.com/allunia

作为本章总结，让我们听听Kaggle大师劳拉·芬克对这个平台的感悟。她不仅是Notebooks特级大师，创作了许多精湛的Notebook，还担任MicroMata公司的数据科学主管。

## 你最喜欢哪种类型的竞赛？为什么？在技术方法和解决思路上，你在Kaggle的专长是什么？

我最钟爱那些能为人类带来益处的竞赛，尤其热衷所有与医疗健康相关的挑战。不过每场比赛对我而言都是充满谜题的冒险，我真正享受的是学习新技能、探索新数据集或问题的过程。因此我不拘泥于特定技术，而是专注于学习新事物。我想大家认可的是我在探索性数据分析(EDA)方面的专长。

## 你如何着手参加Kaggle竞赛？这种方式与日常工作有何不同？

参赛时，我首先阅读问题陈述和数据描述。浏览论坛和公开Notebook收集思路后，通常从开发自己的解决方案开始。初期我会花时间做EDA，寻找隐藏分组并建立直觉，这对制定合理的验证策略大有裨益——我认为这是所有后续步骤的基础。然后我会迭代改进机器学习流程的各个环节：特征工程、预处理、优化模型架构、研究数据收集问题、寻找数据泄漏、深化EDA或构建集成模型。我以贪婪算法般的方式不断优化方案。Kaggle竞赛充满变数，必须尝试多元思路和不同方案才能坚持到最后。

这与我的日常工作截然不同，后者更注重从数据中获取洞见，寻找简单有效的方案来优化业务流程。工作中的任务往往比所用模型更复杂，需要明确定义待解决问题，这意味着要与不同背景的专家讨论目标设定、流程设计及数据采集融合方案。相比Kaggle竞赛，日常工作中沟通能力比机器学习技能更重要。

## 请分享你参加过最具挑战性的竞赛，以及你用来解决问题的洞见

G2Net引力波探测竞赛是我的挚爱之一，目标是检测隐藏在探测器组件噪声和地球引力噪声中的模拟引力波信号。这次竞赛的重要启示是：应该批判性看待标准数据分析方法，勇于尝试自己的思路。在我阅读的论文中，数据预处理通常采用傅立叶变换或恒Q变换，配合白化处理和带通滤波。但很快发现白化处理弊大于利——它采用功率谱密度的样条插值法，而该谱密度本身噪声极大。对噪声数据子集进行多项式拟合又会因过拟合引入额外误差源。

放弃白化处理后，我尝试调整恒Q变换的超参数，这个方法长期占据论坛和公开Notebook的主流。由于存在两种引力波源，其\( Q \)值范围各异，我尝试集成不同超参数的模型组合，这确实提升了分数，但很快遇到瓶颈。恒Q变换通过系列滤波器将时域信号转为频域，这让我开始思考：是否存在更灵活优越的滤波方法？此时社区恰好兴起使用一维CNN的思潮，我立即被吸引。众所周知，二维CNN的滤波器能识别图像中的边缘、线条和纹理，类似效果也可通过拉普拉斯或索贝尔等经典滤波器实现。于是我思考：为何不让一维CNN自主学习最重要的滤波器，而非要使用预设的固定变换？

虽然我最终未能成功实现一维CNN方案，但许多顶尖团队做到了。G2Net竞赛虽未达成夺牌目标，仍是我最珍视的经历——过程中获得的知识以及对所谓标准方法的反思，都是无价之宝。

## Kaggle是否对你的职业发展有所帮助？如果有，具体体现在哪些方面？

我大学毕业后第一份工作是Java软件开发，尽管硕士论文阶段就已接触机器学习。当时虽对数据分析更感兴趣，但数据科学岗位几乎不存在，甚至这个职位名称都尚未普及。初次接触Kaggle时，我立即被其吸引。此后常在晚间登录Kaggle进行趣味性探索，当时并无转岗打算。直到某研究项目需要机器学习技能时，我凭借在Kaggle积累的知识证明了自己是该项目的合适人选——这成为我数据科学职业生涯的起点。

Kaggle始终是我验证想法、学习新方法工具、获取实战经验的绝佳平台。通过这些途径掌握的技能对工作中的数据科学项目大有裨益。它如同知识加速器，提供无风险的沙盒环境供你尝试各种创意。竞赛失败意味着至少获得一次教训，而项目失败可能对自身和他人造成重大负面影响。除参赛外，撰写Notebooks也是构建作品集的好方法——既能展示问题解决思路，又能体现洞察力与结论传达能力，后者在与管理层、客户及跨领域专家协作时尤为重要。

## 根据你的经验，新手Kaggle用户常忽视哪些要点？你现在掌握的哪些知识希望初学时就知道？

许多竞赛新手容易被公开排行榜迷惑，在缺乏合理验证策略的情况下构建模型。他们追逐排行榜名次时，往往对公开测试数据过拟合。竞赛结束后，这些模型无法泛化到未公开的测试数据，排名常暴跌数百位。我仍记得参加梅赛德斯-奔驰绿色制造竞赛时的挫败感——始终无法提升公开排名。但最终结果公布时，大量参赛者排名剧烈波动的情形令人震惊。自此我深刻认识到：完善的验证方案对解决欠拟合与过拟合问题至关重要。

## 你在过往竞赛中犯过哪些错误？

迄今最大错误是在竞赛初期过度纠结方案细节。事实上，建立合理验证框架后，快速迭代各种差异化思路更为有效。这样能更高效地发现改进方向，且不易陷入局部困境。

## 有哪些特别推荐的数据分析或机器学习工具/库？

Kaggle社区活跃着大量可学习实践的主流工具和库，我推荐全部掌握。关键保持灵活性，了解各自优劣——这样你的解决方案将取决于创意而非工具。

## 参加竞赛时最需要牢记的要点是什么？

数据科学的核心不在于建模，而在于理解数据及其采集方式。我参与的多数竞赛都存在数据泄露，或测试数据里可通过探索性分析发现的隐藏分组。

## 本章小结

本章从Kaggle竞赛视角概述了计算机视觉核心主题：首先介绍增强算法泛化能力的重要技术——数据增强，随后针对图像分类、目标检测、语义分割三大高频问题，演示了端到端解决方案。

下章我们将转向自然语言处理领域，这是另一个极其广泛且热门的问题类别。

## 加入本书Discord空间

欢迎加入本书Discord工作区，每月参与作者问答专场：

https://packt.link/KaggleDiscord

## 11 自然语言处理建模

自然语言处理（NLP）是语言学、计算机科学和人工智能的交叉领域，主要研究处理与分析海量自然语言数据的算法。近年来已成为Kaggle竞赛日益热门的话题。虽然该领域涵盖聊天机器人和机器翻译等热门方向，本章将聚焦Kaggle竞赛频繁涉及的特定子领域。

情感分析作为简单分类问题已广为人知，因此我们将从更有趣的变体入手：识别推文中支撑情感的关键短语。接着阐述开放域问答问题的示例解决方案，最后讨论NLP数据增强策略——这个受关注度远低于计算机视觉同类话题的领域。

本章内容概要：

- 情感分析

- 开放域问答

- 文本增强策略

## 情感分析

Twitter是最受欢迎的社交媒体平台之一，也是个人和企业的重要沟通工具。语言情感捕捉对企业尤为重要：积极推文可能病毒式传播，而极端负面内容可能造成伤害。鉴于人类语言的复杂性，不仅需要判断情感倾向，更要解析情感来源——究竟是哪些词汇导致了该情感判定？

我们将通过"推文情感提取竞赛"(https://www.kaggle.com/c/tweet-sentiment-extraction)数据演示解决方法。为简洁起见省略了代码中的导入语句，完整代码可参阅本章GitHub仓库的Notebook文件。先通过数据观察理解问题：

---

df = pd.read_csv('/kaggle/input/tweet-sentiment-extraction/train.csv')

df.head(   )

---

数据预览如下：

<!-- Media -->

<table><tbody><tr><td></td><td>文本ID</td><td>文本</td><td>选中文本</td><td>情感倾向</td></tr><tr><td>0</td><td>cb774db0d1</td><td>我本会回应，如果我要去的话</td><td>我本会回应，如果我要去的话</td><td>中立</td></tr><tr><td>1</td><td>549e992a42</td><td>太难过啦 我会想念你在圣地亚哥的时光！！！</td><td>太难过啦</td><td>消极</td></tr><tr><td>2</td><td>088c60f138</td><td>我老板在欺负我...</td><td>欺负我</td><td>消极</td></tr><tr><td>3</td><td>9642c003ef</td><td>什么面试！别来烦我</td><td>别来烦我</td><td>消极</td></tr><tr><td>4</td><td>358bd9e861</td><td>混蛋儿子们，为什么不能把他们放在...</td><td>混蛋儿子们，</td><td>消极</td></tr></tbody></table>

图11.1：训练数据中的示例行

<!-- Media -->

实际推文存储在text列中，每条推文都带有相关情感标签，以及存储在selected_text列中的支持短语（该短语是决定情感标注的依据）。

我们首先定义基础清洗函数：第一步需要清除网址链接和非字母字符，并将人们用来替代脏话的星号替换为统一标记"swear"。通过正则表达式实现如下：

---

def basic_cleaning(text):

text=re.sub(r'https?://www\\.\\S+\\.com','',text)

text=re.sub(r'[^A-Za-z|\\s]','',text)

text=re.sub(r'\\*+','swear',text) # 将****形式的脏话替换为swear标记

return text

---

接下来清除推文内容中的HTML标签和表情符号：

---

def remove_html(text):

html=re.compile(r'<.*?>')

return html.sub(r'',text)

def remove_emoji(text):

emoji_pattern = re.compile("["

u"\\U0001F600-\\U0001F64F" #表情符号

u"\\U0001F300-\\U0001F5FF" #符号与象形图

u"\\U0001F680-\\U0001F6FF" #交通与地图符号

u"\\U0001F1E0-\\U0001F1FF" #旗帜符号(iOS)

u"\\U00002702-\\U000027B0"

u"\\U000024C2-\\U0001F251"

"]+", flags=re.UNICODE)

return emoji_pattern.sub(r'', text)

---

最后，我们需要能够移除重复字符（例如将"waaaayyyyy"简化为"way"）：

---

def remove_multiplechars(text):

text = re.sub(r'(.)\\1\{3,\}',r'\\1', text)

return text

---

为方便起见，我们将四个功能整合为一个清理函数：

---

def clean(df):

for col in ['text']:#,'selected_text']:

df[col]=df[col].astype(str).apply(lambda x:basic_cleaning(x))

df[col]=df[col].astype(str).apply(lambda x:remove_emoji(x))

df[col]=df[col].astype(str).apply(lambda x:remove_html(x))

df[col]=df[col].astype(str).apply(lambda x:remove_multiplechars(x))

return df

---

最后的准备工作涉及编写基于预训练模型（tokenizer参数）创建嵌入向量的函数：

---

def fast_encode(texts, tokenizer, chunk_size=256, maxlen=128):

tokenizer.enable_truncation(max_length=maxlen)

tokenizer.enable_padding(max_length=maxlen)

all_ids = []

for i in range(0, len(texts), chunk_size):

text_chunk = texts[i:i+chunk_size].tolist(   )

encs = tokenizer.encode_batch(text_chunk)

all_ids.extend([enc.ids for enc in encs])

return np.array(all_ids)

---

接着我们创建预处理函数以便处理整个语料库：

---

def preprocess_news(df,stop=stop,n=1,col='text'):

'''该函数用于预处理并创建语料库'''

new_corpus=[]

stem=PorterStemmer(   )

lem=WordNetLemmatizer(   )

for text in df[col]:

words=[w for w in word_tokenize(text) if (w not in stop)]

words=[lem.lemmatize(w) for w in words if(len(w)>n)]

new_corpus.append(words)

new_corpus=[word for l in new_corpus for word in l]

return new_corpus

---

利用我们预先准备好的函数，可以清洗并准备训练数据。情感列是我们的目标变量，为了提高性能，我们将其转换为虚拟变量（独热编码）：

---

df.dropna(inplace=True)

df_clean = clean(df)

df_clean_selection = df_clean.sample(frac=1)

X = df_clean_selection.text.values

y = pd.get_dummies(df_clean_selection.sentiment)

---

接下来的必要步骤是对输入文本进行分词，并将其转换为序列（同时进行填充，以确保整个数据集中的长度一致）：

---

tokenizer = text.Tokenizer(num_words=20000)

tokenizer.fit_on_texts(list(X))

list_tokenized_train = tokenizer.texts_to_sequences(X)

X_t = sequence.pad_sequences(list_tokenized_train, maxlen=128)

---

我们将使用DistilBERT（蒸馏版BERT）为模型创建嵌入向量并直接使用。该模型是BERT的轻量级版本：以3%的性能损失换取参数量减少40%。虽然训练嵌入层可提升性能，但会大幅增加训练时间。

<!-- Media -->

---

tokenizer = transformers.AutoTokenizer.from_pretrained("distilbert-base-

uncased")

#将加载的分词器保存到本地

save_path = '/kaggle/working/distilbert_base_uncased/'

if not os.path.exists(save_path):

os.makedirs(save_path)

tokenizer.save_pretrained(save_path)

#使用huggingface tokenizers库重新加载

fast_tokenizer = BertWordPieceTokenizer(   )

'distilbert_base_uncased/vocab.txt', lowercase=True)

fast_tokenizer

---

<!-- Media -->

我们可以使用之前定义的fast_encode函数和上述fast_tokenizer来编码推文：

---

X = 快速编码(df_clean_selection.text.astype(str),

快速分词器,

最大长度=128)

---

数据准备就绪后，我们可以构建模型。出于演示目的，我们将采用这类应用中相当标准的架构：结合LSTM层（通过全局池化和dropout进行归一化），顶部再加一个密集层。若要实现真正具有竞争力的解决方案，需对架构进行微调：更"厚重"的模型、更大的嵌入维度、LSTM层中更多的单元等。

---

transformer_layer = transformers.TFDistilBertModel.from_

预训练('distilbert-base-uncased')

嵌入维度 = 128

输入 = 输入(形状=(100,))

输入 = 输入(形状=(128,))

嵌入矩阵=transformer_layer.weights[0].numpy(   )

x = 嵌入(嵌入矩阵.shape[0],

嵌入矩阵.shape[1],

嵌入初始化器=常数(嵌入矩阵),

可训练=假)(输入)

x = 双向(LSTM(50, 返回序列=真))(x)

x = 双向(LSTM(25, 返回序列=真))(x)

x = 全局最大池化1D(   )(x)

x = 随机失活层(0.5)(x)

x = 全连接层(50, 激活函数='relu', 核正则化器='L1L2')(x)

x = 随机失活层(0.5)(x)

x = 全连接层(3, 激活函数='softmax')(x)

蒸馏BERT模型 = 模型(输入=[inp], 输出=x)

蒸馏BERT模型.compile(损失函数='分类交叉熵',

优化器='adam',

评估指标=['准确率'])

---

无需特别关注数据的时间维度，因此直接随机划分为训练集和验证集即可，这可通过fit方法的调用实现：

---

蒸馏BERT模型.fit(X,y,批次大小=32,训练轮数=10,验证集比例=0.1)

---

以下是示例输出：

---

第1轮/共10轮

27480/27480 [==================================] - 480秒 17毫秒/步 - 损失值：

0.5100 - 准确率: 0.7994

第2轮/共10轮

0.4956 - 准确率: 0.8100

第3轮/共10轮

27480/27480 475秒 每步17毫秒 - 损失:

0.4740 - 准确率: 0.8158

第4轮/共10轮

<!-- Media -->

<!-- figureText: 27480/27480 475s 17ms/step - loss: 0.4528 - accuracy: 0.8275 Epoch 5/10 0.4318 - accuracy: 0.8364 Epoch 6/10 27480/27480 0.4069 - accuracy: 0.8441 Epoch 7/10 0.3839 - accuracy: 0.8572 -->

	<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_419.jpg?x=259&y=194&w=1385&h=563&r=0"/>

<!-- Media -->

---

从拟合模型生成预测的过程非常直观。为充分利用所有可用数据，我们首先在整个数据集上重新训练模型（因此不设验证集）：

---

df_clean_final = df_clean.sample(frac=1)

X_train = fast_encode(df_clean_selection.text.astype(str),

fast_tokenizer,

maxlen=128)

y_train = y

---

在生成预测前，我们在完整数据集上重新拟合模型：

---

Adam_name = adam(学习率=0.001)

model_DistilBert.compile(损失函数='分类交叉熵',优化器=Adam_

name,评估指标=['准确率'])

history = model_DistilBert.fit(X_train,y_train,批次大小=32,训练轮数=10)

---

下一步是将测试数据处理成与输入模型的训练数据相同的格式：

---

df_test = pd.read_csv('/kaggle/input/tweet-sentiment-extraction/test.csv')

df_test.dropna(inplace=True)

df_clean_test = clean(df_test)

X_test = fast_encode(df_clean_test.text.values.astype(str),

fast_tokenizer,

maxlen=128)

y_test = df_clean_test.sentiment

---

最后生成预测结果：

---

y_preds = model_DistilBert.predict(X_test)

y_predictions = pd.DataFrame(y_preds,

columns=['negative','neutral','positive'])

y_predictions_final = y_predictions.idxmax(axis=1)

accuracy = accuracy_score(y_test,y_predictions_final)

print(f"最终模型在测试集上的准确率为\{accuracy:.2f\}。")

---

最终模型在测试集上的准确率为0.74。下方展示了输出样例；仅从这几行就可看出，存在人类读者能明显判断情感倾向而模型未能捕捉的情况：

<!-- Media -->

<table><tbody><tr><td></td><td>文本ID</td><td>文本</td><td>情感</td><td>预测为负面</td><td>预测为中性</td><td>预测为正面</td></tr><tr><td>0</td><td>f87dea47db</td><td>今天的最后一节 httptwitpiccomezh</td><td>中性</td><td>0.022949</td><td>0.967165</td><td>0.009886</td></tr><tr><td>1</td><td>96d74cb729</td><td>上海也确实令人兴奋 特别是S...</td><td>正面</td><td>0.000075</td><td>0.012165</td><td>0.987760</td></tr><tr><td>2</td><td>eee518ae67</td><td>经济衰退冲击了Veronique Branquinho 她不得不...</td><td>负面</td><td>0.993622</td><td>0.006364</td><td>0.000014</td></tr><tr><td>3</td><td>01082688c6</td><td>生日快乐</td><td>正面</td><td>0.000020</td><td>0.005859</td><td>0.994122</td></tr><tr><td>4</td><td>33987a8ee5</td><td>httptwitpiccomwp 我喜欢这个</td><td>正面</td><td>0.006184</td><td>0.119946</td><td>0.873870</td></tr><tr><td>5</td><td>726e501993</td><td>太棒了 哇哦 访客们</td><td>正面</td><td>0.000165</td><td>0.019434</td><td>0.980401</td></tr><tr><td>6</td><td>261932614e</td><td>我觉得这里每个人都讨厌我 哈哈</td><td>负面</td><td>0.916203</td><td>0.081649</td><td>0.002148</td></tr><tr><td>7</td><td>afa11da83f</td><td>真希望我能去 但我还在上学 而且MySpace...</td><td>负面</td><td>0.877504</td><td>0.116624</td><td>0.005871</td></tr><tr><td>8</td><td>e64208b4ef</td><td>在上一条线索出现后不久 所有...</td><td>中性</td><td>0.116272</td><td>0.859304</td><td>0.024424</td></tr><tr><td>9</td><td>37bcad24ca</td><td>你买了什么 我这一天还行 还没做...</td><td>中性</td><td>0.223977</td><td>0.756474</td><td>0.019550</td></tr></tbody></table>

图11.2：预测结果中的示例行

<!-- Media -->

我们已演示了解决情感归因问题（识别文本中导致标注者做出情感分类决策的部分）的示例流程。若想获得具有竞争力的性能，可按以下可能影响程度排序进行改进：

- 更大的嵌入维度：这使我们在（预处理后的）输入数据层面就能捕获更多信息

- 更大的模型：LSTM层中增加更多单元

- 更长的训练时间：即更多训练轮次 虽然上述改进无疑会提升模型性能，但流程中的核心要素均可复用：

- 数据清洗与预处理

- 创建文本嵌入

- 在目标模型架构中加入循环层和正则化

接下来我们将讨论开放域问答——NLP竞赛中常见的问题类型。

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_421.jpg?x=240&y=717&w=359&h=361&r=0"/>

<!-- Media -->

## 阿布舍克·塔库尔

https://www.kaggle.com/abhishek

我们采访了全球首位四重Kaggle大师得主阿布舍克·塔库尔。他现任职于Hugging Face，正在开发AutoNLP项目；他还撰写了几乎堪称英语世界唯一（除本书外！）的Kaggle专著《Approaching (Almost) Any Machine Learning Problem》。

## 你在Kaggle上的专长领域是？

没有专长。每项比赛都独一无二，都能从中汲取新知。若真有专长，我就能包揽该领域所有赛事冠军了。

## 你如何着手应对Kaggle比赛？这与日常工作有何不同？

我的第一步总是查看数据并尝试理解。若参赛较晚，会借助公开的EDA内核。

处理Kaggle内外问题时，我首先会建立基准模型。这至关重要，因为它提供了与后续模型比较的基线。若起步较晚，我会避免参考公开笔记来建立基线——那样容易陷入单向思维，至少这是我的切身感受。

完成基准测试后，我会在不进行堆叠或混合等复杂操作的前提下尽可能压榨性能。接着\( I \)重新审视数据和模型，逐步优化基线指标。日常工作往往与此相似——多数情况下先确立基准，然后需要构思能超越该基准的技术方案、特征工程或模型架构。

## 你参加过最有趣的竞赛是哪场？是否获得过独特洞见？

每场竞赛都独具魅力

## Kaggle对你的职业发展有帮助吗？

当然有帮助。近年来Kaggle在数据科学家和机器学习工程师招聘领域建立了极高声誉。平台排名和丰富数据集经验总会以各种形式助力职业发展。处理多样化问题的经验越丰富，迭代速度就越快——这正是企业最看重的素质。没人愿意耗费数月做毫无商业价值的事。

## 根据你的观察，新手Kaggle用户常忽视什么？现在掌握的哪些知识是你希望初学时就知道的？

多数初学者太容易放弃。刚加入竞赛时很容易被顶尖选手吓退。想成功就必须保持毅力——在我看来这是关键。许多新手还惯于依赖公开内核，这会限制思维模式。我的建议是：先独立参赛，自行分析数据、构建特征和模型，再参考他人方案寻找差异点，最后将学习成果融入自己的解决方案。

## 开放领域问答环节

本节将探讨Google QUEST问答标注竞赛(https://www.kaggle.com/c/google-quest-challenge/overview/description)。该竞赛要求人类评估员根据"问题对话性"、"问题事实性"或"答案实用性"等多维标准对问答对评分。任务目标是预测每个标准对应数值列（由于标签来自多位评估者，本质上是输出归一化至单位区间的多元回归问题）。在采用NLP transformer等先进技术建模前，先用简单方法建立基准线仍是明智之举。与前文相同，为简洁起见我们省略了导入语句，具体可参阅GitHub仓库中的Notebook。

我们首先定义若干辅助函数来提取文本特征。首个函数用于计算字符串词数：

---

def word_count(xstring):

return xstring.split(   ).str.len(   )

---

竞赛采用的评估指标是斯皮尔曼等级相关系数（基于排序计算的线性相关：https://en.wikipedia.org/wiki/Spearman%27s_rank_correlation_coefficient）

由于需要构建Scikit-learn流程管道，将指标定义为评分器很有必要（make_scorer是Scikit-learn中的包装器，可将评分函数如准确率或MSE转换为可调用对象）：

---

def spearman_corr(y_true, y_pred):

if np.ndim(y_pred) == 2:

corr = np.mean([stats.spearmanr(y_true[:, i],

y_pred[:, i])[0]

for i in range(y_true.shape[1])])

else:

corr = stats.spearmanr(y_true, y_pred)[0]

return corr

custom_scorer = make_scorer(spearman_corr, greater_is_better=True)

---

接下来是一个辅助函数，用于从1中提取大小为\( n \)的连续块。这将帮助我们后续为文本主体生成嵌入向量时避免内存问题：

---

def chunks(l, n):

for i in range(0, len(l), n):

yield l[i:i + n]

---

我们将使用的部分特征集来自预训练模型的嵌入向量。请注意，本节的核心思想是在不训练复杂模型的情况下构建基线，但这并不妨碍我们使用现有模型。

# 首先导入分词器和模型，然后分块处理语料库，将每个问题/答案编码为固定大小的嵌入向量：

def fetch_vectors(string_list, batch_size=64):

---

#灵感来源于 https://jalammar.github.io/a-visual-guide-to-using-bert-

for-the-first-time/

设备 = torch.device("cuda")

分词器 = transformers.DistilBertTokenizer.from_pretrained

("../input/distilbertbaseuncased/")

模型 = transformers.DistilBertModel.from_pretrained

("../input/distilbertbaseuncased/")

模型迁移到(设备)

最终特征 = []

对于 数据块 在 分块(字符串列表, 批次大小):

已分词 = []

对于 x 在 数据块:

x = " ".join(x.strip(   ).split(   )[:300])

分词 = 分词器.encode(x, 添加特殊标记=True)

已分词.append(分词[:512])

最大长度 = 512

填充 = np.array([i + [0] * (最大长度 - len(i)) 对于 i 在 已分词])

注意力掩码 = np.where(填充 != 0, 1, 0)

input_ids = torch.tensor(padded).to(DEVICE)

attention_mask = torch.tensor(attention_mask).to(DEVICE)

with torch.no_grad(   ):

last_hidden_states = model(input_ids,

attention_mask=attention_mask)

features = last_hidden_states[0][:, 0, :].cpu(   ).numpy(   )

fin_features.append(features)

fin_features = np.vstack(fin_features)

return fin_features

---

现在可以开始加载数据：

---

xtrain = pd.read_csv(data_dir + 'train.csv')

xtest = pd.read_csv(data_dir + 'test.csv')

xtrain.head(4)

---

以下是前几行数据：

<!-- Media -->

<table><tbody><tr><td>问题标题</td><td>问题正文</td><td>提问者用户名</td><td>提问者主页</td><td>回答</td></tr><tr><td>使用近摄接环时会损失什么...</td><td>在尝试微距摄影后发现...</td><td>ysap</td><td>https://photo.stackexchange.com/users/1024</td><td>我刚拿到近摄接环，这是实测情况...</td></tr><tr><td>城市与定居点的区别是什么...</td><td>我想了解哪些地方会被归类为...</td><td>russellpierce</td><td>https://rpg.stackexchange.com/users/8774</td><td>查阅相关定义或许会有帮助...</td></tr><tr><td>通孔元件最大突出长度...</td><td>我正在设计带有通孔元件的PCB...</td><td>Joe Baker</td><td>https://electronics.stackexchange.com/users/10157</td><td>真的需要开槽吗？我们生产的多个产品...</td></tr><tr><td>宣誓书能否用于犹太法庭？</td><td>据我理解，宣誓书本质上是...</td><td>Scimonster</td><td>https://judaism.stackexchange.com/users/5151</td><td>提交"宣誓书"属于双方争议...</td></tr></tbody></table>

图11.3：训练数据中的样本行

<!-- Media -->

## 我们指定感兴趣的30个目标列：

<!-- Media -->

---

<!-- Media -->

<table><tbody><tr><td>目标列 = ['提问者意图理解度',</td></tr><tr><td>'问题主体批判性',</td></tr><tr><td>'问题对话性', '期望简短回答',</td></tr><tr><td>'事实求证型问题',</td></tr><tr><td>'问题有公认答案',</td></tr><tr><td>'问题对他人有趣度',</td></tr><tr><td>'问题对自身有趣度',</td></tr><tr><td>'多意图问题', '非实质性问题',</td></tr><tr><td>'寻求观点型问题', '选择题型问题',</td></tr><tr><td>'比较型问题', '结果型问题',</td></tr><tr><td>'定义型问题', '实体型问题',</td></tr></tbody></table>

<!-- Media -->

---

<!-- Media -->

---

'问题类型_说明', '问题类型_步骤',

'问题类型_原因解释',

'问题类型_拼写',

'问题_表述良好', '回答_有帮助',

'回答_信息量', '回答_可信度',

'回答_相关性', '回答_满意度',

'回答类型_说明', '回答类型_步骤',

'回答类型_原因解释', '回答_表述良好']

---

如需了解这些指标的含义和解读方法，请参阅竞赛数据页：https://www.kaggle.com/c/google-quest-challenge/data。

接下来进行特征工程。我们首先统计问题标题、正文及回答中的单词数量，这个简单特征在许多应用中效果显著：

---

for colname in ['question_title', 'question_body', 'answer']:

newname = colname + '_word_len'

xtrain[newname] = xtrain[colname].str.split(   ).str.len(   )

xtest[newname] = xtest[colname].str.split(   ).str.len(   )

---

接下来创建词汇多样性特征，计算文本片段中独特词汇的占比：

---

colname = 'answer'

xtrain[colname+'_div'] = xtrain[colname].apply

(lambda s: len(set(s.split(   ))) / len(s.split(   )) )

xtest[colname+'_div'] = xtest[colname].apply

(lambda s: len(set(s.split(   ))) / len(s.split(   )) )

---

处理网络来源信息时，可通过分析网址组成部分（此处定义为以点号分隔的地址元素）提取潜在信息特征：统计组件数量，并将各组件存储为特征：

---

for df in [xtrain, xtest]:

df['domcom'] = df['question_user_page'].apply

(lambda s: s.split('://')[1].split('/')[0].split('.'))

#统计组件数量

df['dom_cnt'] = df['domcom'].apply(lambda s: len(s))

#填充长度以防某些域名组件较少

df['domcom'] = df['domcom'].apply(lambda s: s + ['none', 'none'])

#组件

for ii in range(0,4):

df['dom_'+str(ii)] = df['domcom'].apply(lambda s: s[ii])

---

大量目标列涉及答案与问题的相关度。量化这种关系的可行方法是评估字符串对中的共享词汇：

---

#共享元素

对于数据集df in [xtrain, xtest]:

df['q_words'] = df['question_body'].apply(lambda s: [f for f in

s.split(   ) if \( f \) not in eng_stopwords] )

df['a_words'] = df['answer'].apply(lambda s: [f for f in s.split(   ) if

f not in eng_stopwords] )

df['qa_word_overlap'] = df.apply(lambda s: len(np.intersect1d(s['q_

words'], s['a_words'])), axis = 1)

df['qa_word_overlap_norm1'] = df.apply(lambda s: s['qa_word_overlap']/

(1 + len(s['a_words'])), axis = 1)

df['qa_word_overlap_norm2'] = df.apply(lambda s: s['qa_word_overlap']/

(1 + len(s['q_words'])), axis = 1)

df.drop(['q_words', 'a_words'], axis = 1, inplace = True)

---

停用词与标点符号的出现模式可揭示文本风格与意图：

---

对于数据集df in [xtrain, xtest]:

##文本字符数##

df["question_title_num_chars"] = df["question_title"].apply(lambda x:

len(str(x)))

df["question_body_num_chars"] = df["question_body"].apply(lambda x:

len(str(x)))

df["answer_num_chars"] = df["answer"].apply(lambda x: len(str(x)))

##文本中的停用词数量##

df["question_title_num_stopwords"] = df["question_title"].apply(lambda

x: len([w for w in str(x).lower(   ).split(   ) if w in eng_stopwords]))

df["question_body_num_stopwords"] = df["question_body"].apply(lambda

x: len([w for w in str(x).lower(   ).split(   ) if w in eng_stopwords]))

df["answer_num_stopwords"] = df["answer"].apply(lambda x: len([w for w

in str(x).lower(   ).split(   ) if w in eng_stopwords]))

##文本中的标点符号数量##

df["question_title_num_punctuations"] =df['question_title'].

apply(lambda x: len([c for c in str(x) if c in string.punctuation]) )

df["question_body_num_punctuations"] =df['question_body'].apply(lambda

x: 统计字符串x中标点符号的数量

df["answer_num_punctuations"] = df['answer'].apply(lambda x: 统计字符串中

标点符号的数量

##文本中首字母大写单词的数量##

df["question_title_num_words_upper"] = df["question_title"].

apply(lambda x: 统计以空格分隔的全大写单词数量)

df["question_body_num_words_upper"] = df["question_body"].apply(lambda

x: 统计以空格分隔的全大写单词数量)

df["answer_num_words_upper"] = df["answer"].apply(lambda x: 统计字符串中

以空格分隔的全大写单词数量)

---

完成"复古"特征准备后——这些特征聚焦于文本的简单统计量，不涉及语义结构——我们可以开始为问题和答案创建嵌入向量。理论上可以在数据集上训练单独的word2vec类模型（或微调现有模型），但本次演示将直接使用预训练模型。推荐选用谷歌的通用语句编码器(https://tfhub.dev/google/universal-sentence-encoder/4)。该模型基于多源数据训练，输入英文文本后输出512维向量。

---

module_url = "../input/universalsentenceencoderlarge4/"

embed = hub.load(module_url)

---

文本转嵌入向量的代码如下：我们分批处理训练集/测试集条目，逐批进行嵌入（出于内存效率考虑），然后将结果追加至原始列表。

最终数据框通过垂直堆叠各批次嵌入向量列表构建：

---

embeddings_train = \{\}

嵌入测试 = \{\}

遍历文本字段['问题标题', '问题正文', '答案']:

训练文本 = 训练集[文本字段].字符串替换('?', '.').字符串替换('!', '.').

转为列表(   )

测试文本 = 测试集[文本字段].字符串替换('?', '.').字符串替换('!', '.').

转为列表(   )

当前训练嵌入 = []

当前测试嵌入 = []

批次大小 = 4

索引 = 0

当 索引*批次大小 < 训练文本长度时:

当前训练嵌入.append(嵌入(训练文本[索引*批次大小: (索引 +

1)*批次大小])["输出"].转为numpy数组(   ))

索引 += 1

索引 = 0

当 索引*批次大小 < 测试文本长度时:

curr_test_emb.append(embed(test_text[ind*batch_size: (ind +

1)*batch_size])["outputs"].numpy(   ))

ind += 1

embeddings_train[text + '_embedding'] = np.vstack(curr_train_emb)

embeddings_test[text + '_embedding'] = np.vstack(curr_test_emb)

print(text)

---

在获得问题和答案的向量表示后，我们可以通过对向量对采用不同的距离度量来计算字段间的语义相似度。尝试不同度量方法的初衷是为了捕捉多样化的特征类型；类比分类场景中同时使用准确率和熵值来全面把握状况：

---

12_dist = lambda x, y: np.power(x - y, 2).sum(axis=1)

cos_dist = lambda x, y: (x*y).sum(axis=1)

dist_features_train = np.array([

12_dist(embeddings_train['question_title_embedding'], embeddings_

train['answer_embedding']),

l2_dist(embeddings_train['question_body_embedding'], embeddings_

train['answer_embedding']),

l2_dist(embeddings_train['question_body_embedding'], embeddings_

train['question_title_embedding']),

余弦距离(embeddings_train['问题标题向量'], embeddings_

train['答案向量']),

余弦距离(embeddings_train['问题正文向量'], embeddings_

train['答案向量']),

余弦距离(embeddings_train['问题正文向量'], embeddings_

train['问题标题向量'])

]). T

dist_features_test = np.array([

12_dist(embeddings_test['问题标题向量'], embeddings_

test['答案向量']),

l2距离(embeddings_test['问题正文向量'], embeddings_

test['答案向量']),

l2距离(embeddings_test['问题正文向量'], embeddings_

test['问题标题向量']),

余弦距离(embeddings_test['问题标题向量'], embeddings_

test['答案向量']),

余弦距离(embeddings_test['问题正文向量'], embeddings_

测试['answer_embedding']),

余弦距离(embeddings_test['question_body_embedding'], embeddings_

测试['question_title_embedding'])

]). T

---

让我们将距离特征分别存储到不同列中：

---

for ii in range ( 0 , 6 ):

xtrain['dist'+str(ii)] = dist_features_train[:,ii]

xtest['dist'+str(ii)] = dist_features_test[:,ii]

---

最后，我们还可以创建文本字段的TF-IDF表示；总体思路是基于输入文本的多种转换创建多个特征，然后将其输入相对简单的模型。这样，我们无需拟合复杂的深度学习模型就能捕捉数据特征。

我们可以通过分析单词级和字符级文本来实现这一点。为了限制内存消耗，我们对两种特征的最大数量设置了上限（实际效果可能因环境而异；内存越大，这些限制可以放宽）：

---

limit_char = 5000

limit_word = 25000

---

我们实例化字符级和单词级向量化器。问题的设置便于使用Scikit-learn的Pipeline功能，允许在模型拟合过程中组合多个步骤。我们首先为标题列（单词级和字符级）创建两个独立的转换器：

---

title_col = 'question_title'

title_transformer = Pipeline([

('tfidf', TfidfVectorizer(lowercase = False, max_df = 0.3, min_df = 1,

binary = False, use_idf = True, smooth_idf =

错误，

ngram范围 = (1,2), 停用词 = '英文',

token模式 = '(?u)\\\\b\\\\w+\\\\b' , 最大_

特征数 = 限制词数 ))

])

标题转换器2 = 流水线([

('tfidf2', Tfidf向量化器(子线性tf=真,

去除重音='统一码', 分析器='字符',

停用词='英文', ngram范围=(1, 4), 最大特征数= 限制字符))

])

---

我们对正文采用相同逻辑（两个不同的流水线转换器）：

---

正文列 = '问题正文'

正文转换器 = 流水线([

('tfidf',Tfidf向量化器(小写 = 假, 最大文档频率 = 0.3, 最小文档频率 = 1,

二进制 = 假, 使用idf = 真, 平滑idf =

假,

ngram范围 = (1,2), 停用词 = '英文',

token模式 = '(?u)\\\\b\\\\w+\\\\b' , 最大_

特征数 = 限制词数 ))

])

正文转换器2 = 流水线([

('tfidf2', Tfidf向量化器( 亚线性TF=True,

去除重音='unicode', 分析器='字符',

停用词='英语', 词元范围=(1,4), 最大特征数=限制字符))

])

---

最后针对答案列：

---

答案列 = 'answer'

答案转换器 = 流水线([

('tfidf', Tfidf向量化器(小写=False, 最大文档频率=0.3, 最小文档频率=1,

二进制=False, 使用逆文档频率=True, 平滑逆文档频率=

False,

词元范围=(1,2), 停用词='英语',

词元模式='(?u)\\\\b\\\\w+\\\\b', 最大

特征数 = 限制词数 ))

])

答案转换器2 = 流水线([

('tfidf2', Tfidf向量化器( 亚线性TF=True,

strip_accents='unicode', analyzer='char',

stop_words='english', ngram_range=(1, 4), max_features= limit_char))

])

---

我们通过处理数值特征来总结特征工程部分。仅采用简单方法：缺失值填补处理\( \mathrm{N}/\mathrm{A} \)值，以及使用幂变换器稳定分布使其更接近高斯分布（这在神经网络中使用数值特征时通常很有帮助）：

---

num_cols = [

'问题标题词长度', '问题正文词长度',

'回答词长度', '回答差异度',

'问题标题字符数','问题正文字符数',

'回答字符数',

---

第11章

---

'问题标题停用词数','问题正文停用词数',

'回答停用词数',

'问题标题标点数',

'问题正文标点数','回答标点数',

'问题标题大写词数',

'问题正文大写词数','回答大写词数',

'距离0', '距离1', '距离2', '距离3', '距离4', '距离5'

]

数值转换器 = 管道([

('缺失值填充', 简单填充器(策略='常量', 填充值=0)),

('标准化', 幂变换器(方法='yeo-johnson'))

])

---

管道的优势在于可组合嵌套使用。接下来我们将添加分类变量处理功能，并通过列转换器整合所有预处理与特征工程逻辑，使各部分输入数据都能得到针对性处理：

---

分类列 = [ 'dom_0', 'dom_1', 'dom_2',

'dom_3', '类别','匿名提问用户标识',

'匿名回答用户标识','域名计数'

]

分类转换器 = 管道([

('缺失值填充', 简单填充器(策略='常量', 填充值='')),

('编码', 独热编码器(未知值处理='忽略'))

])

预处理器 = 列转换器(   )

转换器列表 = [

('标题', 标题转换器, 标题列),

('标题2', 标题转换器2, 标题列),

('正文', 正文转换器, 正文列),

('正文2', 正文转换器2, 正文列),

('answer', answer_transformer, answer_col),

('answer2', answer_transformer2, answer_col),

('num', num_transformer, num_cols),

('cat', cat_transformer, cat_cols)

	]

)

---

最后，我们准备使用一个结合预处理和模型拟合的Pipeline对象：

---

pipeline = Pipeline([

('preprocessor', preprocessor),

('estimator',Ridge(random_state=RANDOM_STATE))

])

---

评估模型在样本外的性能始终是个好主意：实现这一目标的便捷方法是创建折外预测，我们在第6章讨论过。该流程包含以下步骤：

1. 将数据划分为若干折。本例中使用GroupKFold，因为一个问题可能对应多个答案（位于数据框的不同行）。为防止信息泄露，需确保每个问题仅出现在一个折中。

2. 对每一折，使用其他折的数据训练模型，并为选定折及测试集生成预测。

3. 对测试集的预测结果取平均值。

我们首先准备存储预测结果的"容器"矩阵。mvalid将存放折外预测，而mfull是整个测试集预测结果的占位符（各折预测的平均值）。由于多个问题包含不止一个候选答案，我们基于question_body进行KFold分层分割：

---

nfolds = 5

mvalid = np.zeros((xtrain.shape[0], len(target_cols)))

mfull = np.zeros((xtest.shape[0], len(target_cols)))

kf = GroupKFold(n_splits= nfolds).split(X=xtrain.question_body,

groups=xtrain.question_body)

---

我们遍历折叠并构建独立的模型：

---

for ind, (train_index, test_index) in enumerate(kf):

#将数据分割为训练集和验证集

x0, x1 = xtrain.loc[train_index], xtrain.loc[test_index]

y0, y1 = ytrain.loc[train_index], ytrain.loc[test_index]

for ii in range ( 0 , ytrain.shape[1] ) :

#拟合模型

be = clone(pipeline)

be.fit(x0, np.array(y0)[:,ii])

filename = 'ridge_f' + str(ind) + '_c' + str(ii) + '.pkl'

pickle.dump(be, open(filename, 'wb'))

#分别用于存储OOF预测和测试预测的矩阵

mvalid[test_index, ii] = be.predict(x1)

mfull[:,ii] += be.predict(xtest)/nfolds

print('---')

---

完成拟合部分后，我们可以根据竞赛指定的指标评估模型性能：

---

corvec = np.zeros((ytrain.shape[1],1))

for ii in range ( 0 , ytrain.shape[1] ) :

mvalid[:,ii] = rankdata(mvalid[:,ii])/mvalid.shape[0]

mfull[:,ii] = rankdata(mfull[:,ii])/mfull.shape[0]

corvec[ii] = stats.spearmanr(ytrain[ytrain.columns[ii]], mvalid[:,ii])

[0]

print ( corvec. mean (   ))

---

最终得分为0.34，作为起步阶段的成绩相当不错。

本节我们演示了如何构建文本描述性特征。虽然这并非NLP竞赛的制胜法宝（得分尚可但不足以保证获奖），却是工具箱里值得保留的实用工具。本章最后我们将概述文本增强技术。

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_436.jpg?x=247&y=232&w=351&h=351&r=0"/>

<!-- Media -->

## 石原翔太郎

https://www.kaggle.com/sishihara

本章第二位访谈对象是石原翔太郎（昵称u++），这位竞赛与笔记大师曾带领团队赢得PetFinder.my领养预测竞赛冠军。他目前在日本新闻媒体公司担任数据科学家兼研究员，还出版了多本Kaggle相关日文著作，包括翻译Abhishek Thakur的专著。他每周会发布日文版Kaggle动态简报(https://www.getrevue.co/profile/upura)。

## 您撰写/翻译的Kaggle书籍在哪里可以找到？

https://www.kspub.co.jp/book/detail/5190067.html 是基于泰坦尼克号入门竞赛的Kaggle初学者指南。

https://book.mynavi.jp/ec/products/detail/id=123641是Abhishek Thakur《Approaching (Almost) Any Machine Learning Problem》的日文译本。

您最青睐哪类竞赛？为什么？在技术方法和解决思路上，您在Kaggle的专长是什么？

在Kaggle平台上，我热衷于参加涉及表格或文本数据集的竞赛。这类数据集对我来说非常熟悉，因为它们在新闻媒体公司中被广泛使用。我对处理这些数据集的方法有着深入的了解。

你是如何着手参加Kaggle竞赛的？这种方式与你日常工作有何不同？

最初的流程是相同的：通过探索性数据分析来思考如何解决问题。Kaggle假设需要使用高级机器学习方法，但在商业场景中并非如此。实际工作中，我会尝试寻找避免使用机器学习的方法。即使必须使用，我也更倾向于采用TF-IDF和线性回归等经典方法，而非BERT这类先进技术。

我们很有兴趣了解如何在现实问题中避免使用机器学习。能否举例说明？

在工作中处理自动文章摘要时，我们采用了更直接的抽取式方法\( ( \)（https://www.jstage.jst.go.jp/article/pjsai/JSAI2021/0/JSAI2021_1D20S3a03/_article/-char/en），而非基于神经网络的方法（https://www.jstage.jst.go.jp/article/pjsai/JSAI2021/0/JSAI2021_1D40S3c02/_article/-char/en）。机器学习难以保证100%的性能表现，而人类易于理解和参与的简单方法有时更受青睐。

## 请分享你参加过最具挑战性的竞赛，以及你用来解决问题的洞察

在PetFinder.my宠物领养预测竞赛中，主办方提供了多模态数据集。许多参赛者尝试探索使用所有数据类型，主流做法是从图像和文本中提取特征，拼接后训练LightGBM。我也采用了相同策略。令人惊讶的是，我的队友takuoko（https://www.kaggle.com/takuok）开发了一个出色的端到端神经网络来处理所有数据集。设计精良的神经网络在多模态竞赛中有潜力超越LightGBM——这是我在201年学到的宝贵经验。

## 这个经验在当今仍然适用吗？

我认为答案是肯定的。与2019年相比，神经网络在处理多模态数据方面正变得越来越出色。

## Kaggle对你的职业发展有帮助吗？具体体现在哪些方面？

当然。Kaggle赋予了我丰富的数据分析经验，从中获得的机器学习知识极大提升了我的工作成效。我在Kaggle和商业领域的成就是获得国际新闻媒体协会2020年"30位30岁以下精英奖"和最高奖项的主要原因之一。通过Kaggle，我还结识了许多志同道合者，这些人脉无疑促进了我的职业发展。

## 你是如何借助Kaggle构建作品集的？

通过学习技能、取得竞赛成绩、发布Notebooks、书籍和新闻通讯等方式。

## 你如何进行作品推广？

我拥有多样化的传播渠道，会根据需要选择合适的推广工具，例如Twitter、个人博客和YouTube。

## 根据你的经验，新手Kaggle用户常会忽视什么？你现在掌握的哪些知识是你希望刚开始时就了解的？

探索性数据分析的重要性。在机器学习领域，存在一个"没有免费午餐"定理(No Free Lunch theorem)。我们不仅要学习算法，更要学会如何应对挑战。该定理阐明不存在能在所有问题上都表现优异的通用模型。在机器学习竞赛中，必须找到适合数据集特征和任务特性的模型才能提升分数。

## 你在往届比赛中犯过哪些错误？

过度拟合公开排行榜。在LANL地震预测比赛中，我在公开排行榜成绩优异并以第五名完赛。但最终排名却跌至\( {211}^{st} \)位，这意味着\( I \)过于相信有限数据集。过拟合是机器学习中的常见概念，我通过Kaggle深刻认识到其重要性。

## 你有什么避免过拟合的特殊建议吗？

关键要仔细观察训练集与评估集的划分方式。我会尝试构建能复现这种划分逻辑的验证集。

对于数据分析或机器学习，你推荐使用哪些特定工具或库？

我推荐Pandas，这是处理表格数据集的核心库。我通过提取、聚合和可视化等功能进行探索性数据分析。

## 对于掌握Pandas你有什么学习建议？

可以参考社区教程。Kaggle也提供关于Pandas和特征工程的学习课程。

## 你会使用其他竞赛平台吗？与Kaggle相比如何？

我偶尔使用Signate、Nishika等日本平台(https://upura.github.io/projects/ data_science_competitions/)。这些平台在功能和\( {UX}/{UX} \)方面明显逊于Kaggle，但接触日语等熟悉主题很有趣。

## 文本增强策略

前文详细讨论了计算机视觉问题的增强策略。相比之下，文本数据的类似方法研究较少（从缺乏类似albumentations的专用库可见一斑）。本节我们将展示几种可能的解决方案。

## 基础技术

按惯例，我们先研究基础方法，重点关注随机变更和同义词处理。Wei和Zou(2019)在https://arxiv.org/abs/1901.11196中对基础方法进行了系统研究。

我们从同义词替换开始。用同义词替换特定词汇可生成语义相近但略有差异的文本（若想了解同义词来源等细节，可访问项目页https:// wordnet.princeton.edu/）：

---

定义获取同义词函数(单词):

同义词集合 = 集合(   )

遍历词汇网中的同义词集(单词):

遍历同义词集的词元(   ):

同义词 = 词元名称(   ).替换("_", " ").替换("-", " ").小写(   )

同义词 = "".拼接([字符 for 字符 in 同义词 if 字符 in '

qwertyuiopasdfghjklzxcvbnm'])

同义词集合.添加(同义词)

若单词存在于同义词集合:

同义词集合.移除(单词)

返回列表化的同义词集合

---

我们在上述核心函数外创建简单封装，指定文本块(含多词的字符串)并最多替换\( n \)个单词:

---

定义同义词替换函数(单词列表, 替换数):

单词列表 = 单词列表.分割(   )

新单词列表 = 单词列表.复制(   )

随机单词列表 = 列表化(集合([单词 for 单词 in 单词列表 if 单词不在

停用词]))

random.shuffle(随机单词列表)

已替换数量 = 0

对于随机单词列表中的每个单词:

同义词 = 获取同义词(随机单词)

若同义词数量≥1:

同义词 = random.choice(同义词列表)

新单词列表 = [若单词等于随机单词则替换为同义词，否则保留原词

在新单词列表中]

已替换数量 += 1

若\( \mathsf{{num}\_ {replaced}} >  = \mathsf{n} : \) # 最多替换n个单词

终止循环

句子 = ' '.join(新单词列表)

返回句子

---

让我们观察该函数在实际中的运行效果：

---

打印(f"同义词替换示例：\{同义词替换('敏捷的

棕狐跃过懒狗',4)\}")

---

同义词替换示例：敏捷的棕色大学狐跃起

越过懒散的制动爪

虽称不上莎士比亚水准，但通过显著改变风格传达了相同信息。我们可以扩展这种方法，为每条推文创建多个新句子：

---

trial_sent = data['text'][25]

print(trial_sent)

我iPod上的免费填字游戏很有趣，我上瘾了

for n in range(3):

print(f" 同义词替换示例：\{synonym_replacement(trial_

sent,n)\}")

同义词替换示例：我iPod上的免费填字游戏很有趣，我

沉迷

同义词替换示例：我iPod上的天真填字游戏

很有趣，我上瘾了

同义词替换示例：我iPod上的放弃填字游戏

很有趣，我沉迷

---

如你所见，利用同义词生成文本变体相当简单直接。

接下来，词序替换是一种简单高效的方法：我们通过随机调换文本中单词顺序来创建修改后的句子。

若运用得当，这可被视为一种潜在有效的正则化手段，因为它扰乱了LSTM等模型所依赖的数据序列特性。首先需要定义词序替换函数：

---

def swap_word(new_words):

random_idx_1 = random.randint(0, len(new_words)-1)

random_idx_2 = random_idx_1

counter = 0

while random_idx_2 == random_idx_1:

random_idx_2 = random.randint(0, len(new_words)-1)

counter += 1

if counter > 3 :

return new_words

new_words[random_idx_1], new_words[random_idx_2] = new_words[random_

idx_2], new_words[random_idx_1]

return new_words

---

随后，我们为此函数编写封装器：

---

#n表示需要交换的单词数量

def random_swap(words, n):

words = words.split(   )

new_words = words.copy(   )

for _ in range(n):

new_words = swap_word(new_words)

sentence = ' '.join(new_words)

return sentence

---

同义词替换和单词交换不会改变待修改句子的长度。若具体应用场景需要调整该属性，可通过增删单词实现。最常见的随机删除实现方式如下：

---

def random_deletion(words, p):

words = words.split(   )

#显然，当仅剩一个单词时不应删除

if len (words) == 1:

return words

#以概率p随机删除单词

new_words = []

遍历词语列表中的每个词：

生成0到1之间的随机数

若随机数大于阈值p：

将词加入新列表

# 若最终删除所有词语，则返回随机一个词

若新列表为空：

随机生成列表索引

返回该索引对应的词

将新列表拼接成句子

返回句子

---

## 示例演示：

---

print(随机删除(trial_sent,0.2))

print(随机删除(trial_sent,0.3))

print(随机删除(trial_sent,0.4))

我手机上的免费填词游戏超有趣，让人上瘾

ipod上的免费填词应用让我沉迷其中

我iPod上的免费内容很有趣，我

---

既然能删除，自然也能添加。往句子里随机插入词语可被视为

自然语言处理(NLP)中相当于给图像添加噪点或模糊的操作：

def random_insertion(words, n):

---

words = words.split(   )

new_words = words.copy(   )

for _ in range(n):

add_word(new_words)

sentence = ' '.join(new_words)

return sentence

def add_word(new_words):

synonyms = []

counter = 0

while len ( synonyms ) < 1 :

random_word = new_words[random.randint(0, len(new_words)-1)]

synonyms = get_synonyms(random_word)

计数器 += 1

if 计数器 >= 10:

return

随机同义词 = 同义词表[0]

随机索引 = 随机数生成器.randint(0, len(新词表)-1)

新词表.insert(随机索引, 随机同义词)

---

函数运行示例如下：

---

print(随机插入(测试句,1))

print(随机插入(测试句,2))

print(随机插入(测试句,3))

我沉迷的iPod上那个免费填空应用超有趣，完全上瘾了

我iPod上那个免费的补充填空应用本身就很有趣，让人欲罢不能

那个免费的填空应用让我iPod成瘾，玩起来根本停不下来

---

我们可以将上述所有转换方法整合成单一函数，生成同一句子的四种变体：

---

def 增强(句子,数量,概率):

print(f"原始句子 : \{句子\}")

打印(f"SR增强句子：\{synonym_replacement(sent,n)\}")

打印(f"RD增强句子：\{random_deletion(sent,p)\}")

打印(f"RS增强句子：\{random_swap(sent,n)\}")

打印(f"RI增强句子：\{random_insertion(sent,n)\}")

增强(trial_sent,4,0.3)

原始句子：我iPod上的免费填字游戏应用很有趣，我上瘾了

SR增强句子：我iPod上那个解闷的填字游戏应用很有趣，我

沉迷

RD增强句子：我iPod上的免费应用很有趣，我上瘾了

RS增强句子：iPod上免费的填字游戏应用我的很有趣，我

上瘾

RI增强句子：我iPod上免费的填字游戏应用让人着迷

免费的补充乐趣，我上瘾了

---

上述增强方法未利用文本数据结构——举例而言，即使分析"词性"这类简单特征，也能帮助我们构建更有用的文本变换。这正是我们将要重点探讨的方法。

## nlpaug

最后我们通过展示nlpaug包(https://github.com/makcedward/nlpaug)的功能来总结本节。该工具集成了多种文本增强方法，设计轻量且易于融入工作流。下文将演示其中部分功能示例。

---

! pip 安装 nlpaug

---

我们导入字符级和单词级增强器，用于接入特定方法：

---

导入 nlpaug.augmenter.char 作为 nac

导入 nlpaug.augmenter.word 作为 naw

测试语句 = "我完全不知道这个序列的输出会是什么

这些单词会产生什么结果——发现nlpaug能对此做出什么处理将会很有趣

！"

---

当我们在测试语句中模拟打字错误时会发生什么？此转换可通过多种方式进行参数化；有关完整参数列表及其说明，建议读者查阅官方文档：https://nlpaug.readthedocs.io/en/ latest/augmenter/char/keyboard.html。

---

增强器 = nac.KeyboardAug(名称='Keyboard_Aug', 增强字符最小数=1,

增强字符最大数=10, 增强字符概率=0.3, 增强单词概率=0.3,

增强单词最小数=1, 增强单词最大数=10, 停用词=无,

分词器=无, 反向分词器=无,

包含特殊字符=是, 包含数字=是,

包含大写字母=是, 语言='en', 详细程度=0,

停用词正则表达式=无, 模型路径=无, 最小字符数=4)

测试语句增强版 = 增强器.增强(测试语句)

打印(测试句子)

打印(增强测试句子)

---

## 输出结果如下：

---

我完全不知道这串单词会输出什么结果

- 看看nlpaug能对此做出什么处理会很有趣！

我完&全:不 k懂Z 这 8串T 单s词nDr 会a生Vs 什么结果

- 看n看k nlpaug的j处理n方式会很有趣！

---

我们可以模拟OCR错误渗入输入的情况：

---

增强器 = nac.OcrAug(名称='OCR增强器', 字符增强最小值=1, 字符增强最大值=10,

字符增强概率=0.3, 词语增强概率=0.3, 词语增强最小值=1,

词语增强最大值=10, 停用词=None, 分词器=None,

反向分词器=None, 详细程度=0,

停用词正则=None, 最小字符数=1)

增强测试句子 = 增强器.增强(测试句子)

打印(测试句子)

打印(增强测试句子)

---

我们得到：

---

我完全不知道这串单词会输出什么结果

- 看看nlpaug能对此做出什么处理会很有趣！

我完全不知道这串单词会输出什么结果

- 看看nlpaug能对此做出什么处理会很有趣！

---

虽然字符级转换很有用，但在数据创意性变化方面作用有限。让我们看看nlpaug在单词级修改方面提供了哪些可能性。第一个示例是将固定比例的单词替换为其反义词：

---

aug = naw.AntonymAug(name='Antonym_Aug', aug_min=1, aug_max=10, aug_p=0.3,

lang='eng', stopwords=None, tokenizer=None,

reverse_tokenizer=None, stopwords_regex=None,

verbose=0)

test_sentence_aug = aug.augment(test_sentence)

print(test_sentence)

print(test_sentence_aug)

---

## 我们得到：

---

我完全不知道这串单词会输出什么结果

- 看看nlpaug能对此做出什么处理会很有趣！

我真心不知道这串单词会输出什么结果

不同——这种差异无趣到让人不想了解nlpaug能解构什么

用这个！

---

nlpaug还提供了例如替换同义词的可能性；这类转换也可以通过上文讨论的更基础技术实现。为求完整，我们在下面展示了一个小示例，其底层使用了BERT架构：

---

aug = naw.ContextualWordEmbsAug(model_path='bert-base-uncased',

model_type='', action='substitute',

#temperature=1.0,

top_k=100,

#top_p=None,

name='ContextualWordEmbs_Aug', aug_min=1,

aug_max=10, aug_p=0.3,

stopwords=None, device='cpu',

force_reload=False,

---

第十一章

---

#optimize=None,

stopwords_regex=None,

verbose=0, silence=True)

测试句子增强版 = aug.augment(测试句子)

打印(测试句子)

打印(测试句子增强版)

---

## 结果如下：

---

我完全不知道这串单词会输出什么结果

- 发现nlpaug能对此做什么会很有趣！

我真心不知道这个词串后面会说什么 -

要找出我们能用它做什么似乎不可能！

---

如您所见，nlpaug提供了多种修改文本输入以生成增强文本的选项。具体选择哪些选项很大程度上取决于上下文，需要结合特定应用场景的领域知识来做决定。

进一步探索的起点可以是"灾难推文自然语言处理"这类初学者竞赛（https://www.kaggle.com/c/nlp-getting-started），或是"Jigsaw恶意评论严重性评级"（https://www.kaggle.com/c/jigsaw-toxic-severity-rating）、"Google QUEST问答标注"（https://www.kaggle.com/c/google-quest-challenge）等中高级竞赛。在这些案例中，nlpaug都被广泛使用——包括获奖方案。

## 本章小结

本章我们探讨了NLP竞赛中的建模方法，展示了适用于Kaggle竞赛中各类问题的经典方法和前沿技术，同时还涉及了常被忽视的文本增强技术。

下一章我们将讨论模拟竞赛，这是近些年逐渐兴起的新型比赛类别。

## 加入本书Discord空间

加入本书的Discord工作区，每月可参与作者问答会：

https://packt.link/KaggleDiscord

## 12 模拟与优化竞赛

强化学习（RL）是机器学习各分支中一个有趣的特例。一方面，从技术角度看它要求颇高：监督学习中的许多直觉在此并不适用，相关数学工具也更为高阶；另一方面，它却最容易被外行或非专业人士理解。举个简单类比：就像训练宠物\( ( \)（我刻意避开猫狗之争）做动作时，表现好就给零食奖励，否则就不给。

强化学习虽较晚加入Kaggle竞赛阵营，但近年来随着模拟竞赛的推出已改变局面。本章将介绍Kaggle平台上这一激动人心的新领域。截至撰稿时，已举办过四场精选赛和两场练习赛；虽数量有限，但足以让我们全面了解其概况。

本章我们将展示针对多场模拟竞赛的解决方案：

- 从《连珠\( X \)》开始

- 接着是《石头剪刀布》，展示构建竞技智能体的双重策略

- 随后演示圣诞主题竞赛中基于多臂老虎机的解决方案

- 最后概述其他略超本章范围的竞赛。若强化学习对您全新，建议先掌握基础知识。Kaggle学习平台针对游戏AI的强化学习入门课程（https://www.kaggle.com/learn/intro-to-game-ai-and-reinforcement-learning）是绝佳起点，该课程讲解智能体与策略等基础概念，并简要介绍深度强化学习。所有案例均采用《连珠\( X \)》练习赛数据，目标训练能完成直线连珠的智能体（https://www.kaggle.com/c/connectx/overview）。

更宏观来看，模拟与优化竞赛的关键在于环境特性：由于问题本质，解决方案需具备比提交静态数字（如传统监督学习竞赛）更动态的特性。竞赛环境的详细说明参见：https://github.com/Kaggle/kaggle-environments/blob/master/README.md

## 连珠X

本节展示如何用启发式方法解决简单的连珠游戏问题。虽非深度学习方案，但这种概念基础讲解对RL初学者更具实用价值。

若对棋盘游戏AI概念陌生，Tom van de Wiele的演讲（https://tinyurl.com/36rdv5sa）值得参考：https://www.kaggle.com/tvdwiele

《连珠\( X \)》目标是在棋盘上先于对手形成X颗同色棋子的横、竖或斜线。玩家轮流从棋盘顶部列槽落子，这意味着每步棋可能包含进攻取胜或防守阻挠的双重意图。

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_451.jpg?x=551&y=210&w=782&h=693&r=0"/>

图12.1：连珠X棋盘

<!-- Media -->

《连珠\( X \)》是首个引入智能体的竞赛：参赛者需提交能与其他智能体对战的动态程序，而非静态提交物（或针对未知数据集评估的Notebook）。评估流程分步进行：

1. 提交后，程序先进行自我对战以确保运行正常

2. 若本次验证环节成功，系统将分配技能评级，该提交作品即会加入所有参赛者行列。

3. 每日会为每份提交作品进行多轮对局，随后更新排名。

基于上述设置，接下来我们将演示如何为Connect\( X \)竞赛构建提交方案。所示代码适用于\( X = 4 \)，但稍作修改即可适配其他\( X \)参数值。

首先安装Kaggle环境包：

!pip install kaggle-environments --upgrade

我们定义评估智能体的环境：

---

from kaggle_environments import evaluate, make

env = make("connectx", debug=True)

env.render(   )

---

虽然开发者常倾向于尝试复杂方法，但简单入手往往更有效——正如我们将采用基础启发式算法。配套代码中这些规则已整合为单一函数，但为便于说明，此处逐一讲解。

首条规则是检查任一方是否可能垂直连成四子，若存在则返回可行位置。通过简单变量作为输入参数即可实现，该参数可取两个值分别对应分析哪方机会：

---

def my_agent(observation, configuration):

from random import choice

#己方:me_or_enemy=1, 敌方:me_or_enemy=2

def check_vertical_chance(me_or_enemy):

for i in range ( 0 , 7 ):

如果 observation.board[i+7*5] == 我方或敌方 `

且 observation.board[i+7*4] == 我方或敌方 \\

且 observation.board[i+7*3] == 我方或敌方

且 observation.board[i+7*2] == 0:

返回 i

否则如果 observation.board[i+7*4] == 我方或敌方 \\

且 observation.board[i+7*3] == 我方或敌方 \\

且 observation.board[i+7*2] == 我方或敌方 \\

且 observation.board[i+7*1] == 0:

返回 i

否则如果 observation.board[i+7*3] == 我方或敌方 \\

且 observation.board[i+7*2] == 我方或敌方 \\

且 observation.board[i+7*1] == 我方或敌方

且 observation.board[i+7*0] == 0:

返回 i

#无机会

return -99

---

我们可以为水平机会定义一个类似的方法：

---

def check_horizontal_chance(me_or_enemy):

chance_cell_num = -99

for i in \( \left\lbrack  {0,7,{14},{21},{28},{35}}\right\rbrack \) :

for j in range(0, 4):

val_1 = i+j+0

val_2 = i+j+1

val_3 = i+j+2

val_4 = i+j+3

if sum([observation.board[val_1] == me_or_enemy, \\

observation.board[val_2] == me_or_enemy, \\

observation.board[val_3] == me_or_enemy, \\

observation.board[val_4] == me_or_enemy]) == 3:

for k in [val_1,val_2,val_3,val_4]:

if observation.board[k] == 0 :

机会单元格编号 = k

#底线

循环范围从35到42：

若机会单元格编号为1：

返回1减35

#其他情况

若观察面板[机会单元格编号+7]不为0：

返回机会单元格编号模7

#无机会

返回-99

---

我们对对角线组合采用相同方法：

---

#己方：me_or_enemy=1，敌方：me_or_enemy=2

定义检查斜向机会函数(敌我标识，偏移量，单元格列表)：

机会单元格编号 = -99

遍历单元格列表：

值1 = 当前项+偏移量*0

val_2 = i+lag*1

val_3 = i+lag*2

val_4 = i+lag*3

if sum([observation.board[val_1] == me_or_enemy, \\

observation.board[val_2] == me_or_enemy, \\

observation.board[val_3] == me_or_enemy, \\

observation.board[val_4] == me_or_enemy]) == 3:

for j in [val_1,val_2,val_3,val_4]:

if observation.board[j] == 0 :

chance_cell_num = j

#底行

for k in range(35, 42):

if chance_cell_num == k:

return k - 35

#其他

if chance_cell_num != -99 \\

且观察面板[机会单元格编号+7] != 0:

返回 机会单元格编号 % 7

#无机会

返回 -99

---

我们可以将逻辑整合到单一函数中检查机会（与对手对战时）：

---

def 检查我的机会(   ):

#检查我的纵向机会

结果 = 检查纵向机会(我的编号)

如果 结果 != -99 :

返回 结果

#检查我的横向机会

结果 = 检查横向机会(我的编号)

如果 结果 != -99 :

返回 结果

#检查我的斜向机会1（从右上到左下）

结果 = 检查斜向机会(我的编号, 6, [3,4,5,6,10,11,12,13,17,

18,19,20])

若结果不等于-99：

返回结果

#检查我的斜向机会2（左上至右下）

结果 = 检查斜向机会(我方编号, 8, [0,1,2,3,7,8,9,10,14,15,

16,17])

若结果不等于-99：

返回结果

#无机会

返回-99

---

这些代码块构成了逻辑基础。虽然表述略显繁琐，但这是将直觉转化为启发式规则的宝贵实践，可用于游戏对战智能体。

完整智能体定义请参阅代码库中的配套代码。

新定义智能体的性能可通过预定义智能体（如随机策略智能体）进行评估：

---

环境.重置()

环境.运行([我的智能体, "随机"])

环境.渲染(模式="ipython", 宽度=500, 高度=450)

---

上述代码展示了如何为相对简单的问题（Connect \( X \)被列为Playground而非Featured竞赛自有其道理）从头构建解决方案。有趣的是，这种简单问题也能用（近乎）最前沿的方法如AlphaZero处理：https://www.kaggle.com/connect4alphazero/alphazero-baseline-connectx。

完成入门示例后，您已具备能力参与更复杂（或至少非玩具示例级别的）竞赛。

## 石头剪刀布

模拟竞赛中多个问题涉及游戏并非偶然：在不同复杂度层级上，游戏提供了规则明确的环境，天然契合智能体-动作-奖励框架。除井字棋外，连珠棋是对抗性游戏中最简单的实例之一。沿着难度阶梯（游戏类型）上移，让我们观察石头剪刀布游戏，以及如何应对以该游戏为核心的Kaggle竞赛。

石头剪刀布竞赛(https://www.kaggle.com/c/rock-paper-scissors/code)的创意是对基础游戏（部分地区称为roshambo）的扩展：将常规的"三局两胜"改为"千局决胜"。我们将阐述两种解决思路：一种基于博弈论方法，另一种更侧重算法实现。

首先从纳什均衡谈起。维基百科将其定义为非合作博弈的解，该博弈涉及两个及以上玩家，每个玩家均知晓他人的均衡策略，且任何玩家都无法通过单方面改变策略获得优势。

关于博弈论框架下的石头剪刀布游戏，可通过https://www.youtube.com/watch?v=-1GDMXoMdaY观看精彩入门讲解。

将玩家标记为红蓝双方，结果矩阵中的每个单元格显示特定动作组合的结果：

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_456.jpg?x=627&y=934&w=630&h=576&r=0"/>

图12.2：石头剪刀布收益矩阵

<!-- Media -->

例如，若双方均出石头（左上角单元格），双方得0分；若蓝方出石头红方出布（首行第二列单元格），红方获胜——故红方得+1分，蓝方得-1分。

若我们以\( 1/3 \)的均等概率执行每个动作，对手也必须如此；反之若对手始终出石头，将有\( 1/3 \)概率（即三分之一次数）与石头平局、负于布、战胜剪刀。此时期望收益为0，我们可改为始终出布以必胜。同理可推导布对剪刀、剪刀对石头的策略，因重复性恕不展示结果矩阵。

要达到均衡，剩余选择是双方必须采用随机策略——此即纳什均衡。据此可构建简单智能体：

---

%%writefile submission.py

import random

def nash_equilibrium_agent(observation, configuration):

return random.randint(0, 2)

---

开头的魔法代码（从Notebook直接写入文件）是为满足本赛事提交要求而设。

我们的纳什智能体对阵其他策略表现如何？可通过性能评估得知：

---

!pip install -q -U kaggle_environments

from kaggle_environments import make

---

撰写本文时，该导入操作后会弹出错误（无法加载名为'gfootball'的模块）；Kaggle官方建议忽略此错误。实际上，它似乎对代码执行没有任何影响。

我们首先创建石头剪刀布游戏环境，并将每次模拟的回合数限制设为1,000次：

---

env = make(   )

"rps",

configuration=\{"episodeSteps": 1000\}

)

---

我们将利用本竞赛中创建的一个实现了多种基于确定性启发式智能体的Notebook（https://www.kaggle.com/ilialar/multi-armed-bandit-vs-deterministic-agents），并从中导入我们要对抗的智能体代码：

---

%%writefile submission_copy_opponent.py

def copy_opponent_agent(observation, configuration):

if observation.step > 0 :

return observation.lastOpponentAction

else:

return 0

#nash_equilibrium_agent vs copy_opponent_agent

env.run(   )

["submission.py", "submission_copy_opponent.py"]

)

环境渲染(模式="ipython", 宽度=500, 高度=400)

---

当我们执行前序代码块并运行环境时，可以观察到持续1000个训练周期的动态棋盘。其运行快照如下所示：

<!-- Media -->

<!-- figureText: Player 1 Player 2 2 Scissors ✘ Tie -5 160 / 1000 Action: 2 Name: Scissors Icon: 火 Result: Reward: 5 -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_458.jpg?x=472&y=843&w=947&h=721&r=0"/>

图12.3：评估智能体表现的渲染环境快照

<!-- Media -->

在监督学习（包括分类与回归）中，通常建议从简单基准模型入手，例如线性模型。虽然这些模型并非最先进技术，但能提供有价值的性能预期和衡量标准。强化学习领域也存在类似理念——多臂老虎机作为最简单的RL算法，同样值得尝试。下一节我们将演示如何将该方法应用于模拟竞赛。

## 2020年圣诞主题竞赛

近年来Kaggle平台形成了十二月举办圣诞主题竞赛的传统。虽然每年算法任务不同，但2020年竞赛（https://www.kaggle.com/c/santa-2020）对我们而言是个有趣案例。

该竞赛采用经典多臂老虎机(MAB)框架，通过自动售货机重复操作实现奖励最大化，但附加两个特殊机制：

- 奖励衰减：每操作一步，获得奖励的概率降低3%

- 竞争机制：不仅受尝试次数限制，还需与追求相同目标的对手竞争。虽然这个约束条件对我们的演示方案影响不大，但出于完整性仍在此说明。

关于多臂老虎机问题的通用解决方法，建议参阅：https://lilianweng.github.io/lil-log/2018/01/23/the-multi-armed-bandit-problem-and-its-solutions.html

我们的方案改编自Ilia Larchenko的代码（https://www.kaggle.com/ilialar/simple-multiarmed-bandit），基于奖励分布的迭代更新：每一步从Beta分布生成随机数，其参数\( \left( {a + 1,b + 1}\right) \)中：

- \( a \)代表该摇臂累计奖励（获胜次数）

- \( b \)代表历史失败次数

决策时选择生成值最大的摇臂，并将其作为下一步的先验分布。

<!-- Media -->

下图展示不同(a,b)参数组合下Beta分布的形态：

<!-- figureText: 14 a=0, b=0 a=2, b=8 a=10, b=40 a=20, b=80 a=40, b=160 0.6 12 10 -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_460.jpg?x=242&y=287&w=1396&h=763&r=0"/>

图12.4：不同(a,b)参数组合下的贝塔分布密度形状

<!-- Media -->

如图所示，初始时分布呈平坦形态\( (\operatorname{Beta}\left( {0,0}\right) \)即均匀分布），但随着信息不断积累，概率质量会向众数周围集中，这意味着不确定性降低且判断信心增强。我们可以通过每次使用臂杆时递减\( a \)参数来实现竞赛特有的奖励衰减机制。

我们通过编写提交文件开始创建智能体。首先是必要的导入和变量初始化：

---

%%写入文件 submission.py

导入 json

导入 numpy 为 np

导入 pandas 为 pd

老虎机状态 = 无

总奖励 = 0

上一步 = 无

---

我们定义描述多臂老虎机智能体的类。为保证阅读连贯性，此处重现完整代码并在其中以注释形式加入说明：

---

定义 多臂老虎机智能体 (观测值, 配置):

全局 历史记录, 老虎机历史

步长 = 1.0 # 平衡探索/利用

衰减率 = 0.97 # 每次调用后胜场数的衰减比例

全局 老虎机状态,总奖励,上一步

如果 observation.step == 0:

#初始化老虎机状态

bandit_state = [[1,1] for i in range(configuration["banditCount"])]

否则:

#根据上一步结果更新bandit_state

last_reward = observation["reward"] - total_reward

total_reward = observation["reward"]

#需要确定我们是玩家1还是2

player = int(last_step == observation.lastActions[1])

如果 last_reward > 0 :

bandit_state[observation.lastActions[player]][0] += last_

reward * step

否则:

bandit_state[observation.lastActions[player]][1] += step

bandit_state[observation.lastActions[0]][0] = (bandit_

state[observation.lastActions[0]][0] - 1) * decay_rate + 1

bandit_state[observation.lastActions[1]][0] = (bandit_

state[observation.lastActions[1]][0] - 1) * decay_rate + 1

#为每个智能体生成贝塔分布(Beta distribution)的随机数，并

选择最幸运的那个

最佳概率 = -1

最佳智能体 = 无

for k in range(configuration["banditCount"]):

概率 = np.random.beta(bandit_state[k][0],bandit_state[k][1])

if 概率 > 最佳概率:

最佳概率 = 概率

最佳智能体 = k

最后一步 = 最佳智能体

return 最佳智能体

---

如您所见，该函数的核心逻辑是MAB算法(多臂老虎机算法)的直观实现。针对本次竞赛的特殊调整体现在bandit_state变量上，我们在此应用了衰减乘数。

与前例类似，我们现在可以评估智能体在竞赛环境中的表现。以下代码片段展示了实现方式：

---

%%writefile random_agent.py

导入随机模块

定义随机智能体函数（observation, configuration）：

return 随机生成范围（configuration.banditCount）

从kaggle_environments导入make函数

环境 = 创建（"mab", 调试模式=True）

环境重置()

环境运行(["random_agent.py", "submission.py"])

环境渲染（模式="ipython", 宽度=800, 高度=700）

---

我们会看到类似这样的画面：

<!-- Media -->

<!-- figureText: Speed Adversarial Multi-armed Play Bandit Player 2 42 Win 342 681 / 2000 Player 1 Action: 2 Result: Reward: 261 -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_463.jpg?x=469&y=212&w=950&h=702&r=0"/>

图12.5：评估智能体性能的渲染环境截图

<!-- Media -->

本节展示了如何在Kaggle模拟竞赛中运用经典的多臂老虎机算法。虽然作为入门很有帮助，但这种方法不足以进入奖牌区——在那里深度强化学习方法更为流行。

后续我们将讨论基于其他方法的策略，涵盖各类竞赛场景。

## 游戏名称

相较于前文讨论的基础游戏，模拟竞赛往往包含更复杂的设定。本节将简要介绍这些案例。首个例子是Halite，竞赛页面（https://www.kaggle.com/c/halite）对其定义如下：

Halite [...] 是一款资源管理游戏，玩家需组建并操控小型舰队。通过算法指挥舰船采集光能矿物halite，比赛结束时持有最多halite者获胜。你需要制定高效行动策略，包括舰队调度、新舰建造、船坞设立以及开采地图上再生的halite资源。

游戏界面如图所示：

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_464.jpg?x=470&y=282&w=947&h=904&r=0"/>

图12.6：岩盐（Halite）游戏棋盘

<!-- Media -->

Kaggle围绕该游戏组织了两项赛事：一个Playground版本（https://www.kaggle.com/c/halite-iv-playground-edition）和常规Featured版本（https://www.kaggle.com/c/halite）。经典强化学习方法在此场景中效果有限，因为随着单位（舰船/基地）数量任意增长及动态对手池的存在，对于仅拥有"普通"计算资源的参与者而言，信用分配问题变得难以解决。

全面阐述信用分配问题超出了本书范畴，但建议感兴趣的读者从维基百科条目（https://en.wikipedia.org/wiki/Assignment_problem）入门，继而阅读Mesnard等人的精彩导论文章：https://proceedings.mlr.press/v139/mesnard21a.html。

Tom van de Wiele的获胜方案描述（https://www.kaggle.com/c/halite/discussion/183543）精彩概述了本案例中成功的改进方法（采用单位独立信用分配的深度强化学习）。另一项涉及复杂游戏的赛事是Lux AI（https://www.kaggle.com/c/lux-ai-2021），参赛者需设计智能体解决资源采集与分配的多变量优化问题，并与其他玩家对抗。优秀智能体还需分析对手行动并作出响应。该赛事有个有趣现象——模仿学习（https://paperswithcode.com/task/imitation-learning）这种"元"方法大受欢迎。作为RL领域较新颖的方法，它专注于从示范中学习行为策略，而无需描述状态-动作对生成的特定模型。Kaggle用户Ironbar提供了该理念的竞赛级实现（截至撰写时）：https://www.kaggle.com/c/lux-ai-2021/discussion/293911。

最后，谈及Kaggle模拟赛事就不得不提曼城足球俱乐部合作的Google Research Football竞赛（https://www.kaggle.com/c/google-football/overview）。该赛事旨在探索AI智能体在足球等复杂场景中的表现能力。竞赛概述章节如此定义问题：

这项运动需要短期控制、传球等习得概念与高层策略的平衡，这些对智能体而言都较难掌握。现有环境可用于训练测试智能体，但其他解决方案可能效果更佳。

与前述案例不同，本次竞赛由强化学习方法主导：

- Raw Beast团队\( \left( {3}^{\text{rd }}\right) \)采用受AlphaStar启发的方案：https://www.kaggle.com/c/google-football/discussion/200709

- Salty Fish\( \left( {2}^{\text{nd }}\right) \)运用了自博弈形式：https://www.kaggle.com/c/google-football/discussion/202977

- 冠军团队WeKick通过创造性特征工程和奖励结构调整的深度学习方案胜出：https://www.kaggle.com/c/google-football/discussion/202232

研究上述方案是学习如何运用RL解决此类问题的绝佳起点。

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_466.jpg?x=244&y=229&w=359&h=362&r=0"/>

<!-- Media -->

## 首访戈南

https://www.kaggle.com/frtgnn

本章访谈对象是Firat Gonen——数据集、Notebook和讨论板块三料特级大师，HP数据科学全球大使。他分享了Kaggle参赛心得及多年来的心态演变。

## 您最青睐哪类竞赛？原因何在？在技术方法层面，您在Kaggle的专长是什么？

我的偏好随时间而变。早期钟情通用表格竞赛，那时一台好笔记本加耐心就能把握趋势。我自认曾能较好识别训练集与测试集的异常趋势。后来随着\( Z \)授予大使称号及\( {HP} \)工作站设备的升级，我逐渐转向计算机视觉竞赛，尽管仍有诸多需要学习。

## 您如何规划Kaggle竞赛？这与日常工作方法有何不同？

我通常倾向于尽可能推迟建模环节，将时间用于探索性数据分析(EDA)、异常值处理、阅读论坛等，保持耐心。完成特征工程后，我会先建立基准模型来评估不同架构效果。这种工作方法同样适用于专业领域——我认为长时间追求完美是徒劳的，必须在时间投入与成果产出间取得平衡。

## 请分享你参加过最具挑战性的竞赛，以及你用来解决问题的关键洞察

François Chollet主办的竞赛极具挑战性，这是首个迫使我们涉足通用人工智能(AGI)的赛事。记得当时深感无力，但也掌握了多项新技术。这场竞赛让所有人意识到数据科学不仅限于机器学习，像混合整数规划这类技术也在Kaggle重现光芒。

## Kaggle对你的职业发展有帮助吗？具体体现在哪些方面？

当然：通过Kaggle我掌握了许多新技术并保持知识更新。现阶段我的主要职责偏向管理，因此Kaggle对我保持技术敏锐度至关重要。

## 你如何借助Kaggle构建个人作品集？

我认为优势体现在间接层面——人们既看到我的传统教育背景赋予的理论素养，也通过Kaggle见证了实践能力。

## 根据你的经验，新手Kaggle用户常忽视什么？你现在掌握了哪些希望初学时就知道的要领？

新手常犯两个错误：一是畏惧参加新比赛，担心糟糕成绩会被记录——这纯属多虑，所有人都有失利经历，关键看你投入多少。二是急于进入建模阶段，这种浮躁心态非常有害——他们迫切想看到基准分数，结果往往沮丧。我建议在特征生成、筛选及EDA环节保持耐心。

## 你在过往竞赛中犯过哪些错误？

遗憾的是，我的错误与新手如出一辙：在某些竞赛中因前期投入不足而急躁冒进，等到醒悟时往往为时已晚。

对于数据分析或机器学习，你有什么特别推荐的工具或库吗？

推荐使用PyCaret进行快速基准测试，选用PyTorch作为建模框架。

## 参加竞赛时最需要牢记或践行的重要事项是什么？

探索性数据分析和往届同类竞赛讨论。

## 你使用其他竞赛平台吗？它们与Kaggle相比如何？

说实话，我从未在Kaggle之外掷过骰子，但作为旁观者确实见识过不少。适应其他平台需要时间。

## 本章概要

本章讨论了模拟竞赛这一日益流行的新型赛事。与以视觉或自然语言处理为核心的比赛相比，模拟竞赛涉及的方法论范围更广（数学含量略高），这体现了监督学习与强化学习的本质差异。

本章是本书技术部分的收官之作。后续内容将探讨如何将Kaggle笔记本转化为项目作品集，并借此开拓职业机遇。

## 加入本书Discord社区

加入本书Discord工作区，每月参与作者问答会：

https://packt.link/KaggleDiscord ——————第三部分————

# 竞赛助力职业发展

## 第13章 创建项目与创意作品集

参与Kaggle的益处不仅体现在四个方面的高分表现及随之而来的社区声望——这固然能带来成就感和满足感，更重要的是它能产生超越平台的影响力，推动你的职业发展。这种价值既源于参赛过程中接触陌生数据集、尝试新技术获得的经验，也来自与其他数据科学家建立的联系，以及可能获得的企业关注。

虽然许多企业并未完全将Kaggle视为资质证明，但竞赛成果能充分展示你的能力，助你在人群中脱颖而出。本章将探讨如何通过适当方式在Kaggle及其他平台展示作品，包括以下内容：

- 用Kaggle构建作品集

- 拓展Kaggle之外的线上影响力

- 关注竞赛更新与行业资讯

下一章我们将探讨Kaggle如何通过扩展人脉网络和提供职业机会直接影响你的职业生涯，为全书作结。

## 用Kaggle构建作品集

需辩证看待Kaggle自称"数据科学之家"的定位。正如我们详细讨论过的，Kaggle向所有愿意根据给定评估指标竞逐预测任务最佳模型的人开放，不论你身处何地、教育背景如何或预测建模能力高低。有时也会举办非预测性质的竞赛，比如强化学习比赛、算法挑战和分析竞赛，这些活动面向的群体远不止数据科学家。但根据特定指标从数据中做出最佳预测，始终是Kaggle竞赛的核心宗旨。

而现实世界的数据科学则具有多面性。首先，你的首要任务是解决问题，模型评分指标只是对问题解决效果的粗略量化。你可能需要同时权衡多个指标，且解决路径往往不唯一——问题表述方式本身就会极大影响结果。

数据方面，你很少会获得必须使用的数据规范，可以任意修改现有数据集以满足需求，必要时甚至能从零创建全新数据集。数据整合与处理方式也全无指引。解决问题时还需考虑：

- 技术债务

- 解决方案的长期可维护性

- 方案运行的时间与计算成本

- 模型机理的可解释性

- 对营业利润的影响（商业项目中，增加利润和/或降低成本始终是主旋律）

- 不同复杂度和抽象层级的结果传达

通常这些因素都比单纯的评估指标表现更重要。

技术债务虽在软件开发中更常见，但与数据科学密切相关。它指那些为加速项目交付而采取、但后期需以更高成本返工的临时方案。David Sculley等谷歌研究者的经典论文《机器学习系统中的隐藏技术债务》深刻阐述了该问题对数据科学的意义：https://proceedings.neurips.cc/paper/2015/file/86df7dcfd896fcaf2674f757a2463eba-Paper.pdf 这类专业知识难以通过Kaggle竞赛获取，主要需在企业环境中实践积累。但Kaggle竞赛培养的技能与我们讨论的诸多考量并非割裂，它们能有效补充企业级数据科学流程。通过参赛，你能接触多元数据和问题，进行深入特征工程与快速假设迭代，并学习用开源工具构建前沿方案——这些都是值得在个人履历中突出的宝贵技能。最佳展现方式是建立作品集，收录基于Kaggle竞赛及其他平台资源的解决方案。

构建Kaggle竞赛作品集有多种方式，最简单的是利用平台提供的功能，特别是数据集、Notebook和讨论区。

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_473.jpg?x=242&y=944&w=356&h=362&r=0"/>

<!-- Media -->

## 吉尔伯托·蒂特里茨

https://www.kaggle.com/titericz

在继续之前，我们通过专访吉尔伯托·蒂特里茨探讨Kaggle带来的职业机遇。这位竞赛与讨论双料大师曾位居Kaggle排名榜首，现保持金牌总数第一纪录，现任英伟达高级数据科学家，近期还登上《连线》专题报道：https://www.wired.com/story/solve-these-tough-data-problems-and-watch-job-offers-roll-in/

你最喜欢的竞赛类型及原因？在Kaggle上最擅长的技术方法是什么？

自2011年参赛以来，我最偏爱结构化表格数据竞赛。最常用的技术是分类特征的目标编码（错误方式层出不穷）和堆叠集成。

## 你如何着手参加Kaggle竞赛？这种方式与你日常工作有何不同？

Kaggle是机器学习的绝佳实践平台。与现实项目的主要区别在于，Kaggle竞赛的问题定义、数据格式、目标变量和评估指标都已预先设定完善。因此我总会从探索性数据分析（EDA）开始，理解赛题和熟悉数据集是获得竞争优势的关键。随后我会花时间制定恰当的验证策略——这对模型验证至关重要，需确保验证方式与Kaggle私有测试集的评分逻辑一致。虽然分层K折验证适用于大多数二分类问题，但必须评估是否需要采用分组\( K \)折或时间序列分割，以准确验证模型、防止过拟合，并最大程度模拟私有测试集环境。之后我会专注于特征工程和超参数优化的实验。最后必定会提交至少一个梯度提升树模型和一个深度学习方案，这种多样性融合能有效提升预测差异度，从而优化竞赛指标。

## Kaggle对你的职业发展有帮助吗？具体体现在哪些方面？

是的，Kaggle直接改变了我的职业轨迹。2016年之前我是一名电子工程师，而通过2011年起在竞赛中积累的经验，我成功转型进入数据科学领域。Kaggle帮助我理解机器学习概念，并将理论知识转化为实践。这个平台堪称绝佳的实验场，你可以下载数据集进行深度挖掘，这种竞争机制既能提升编程与机器学习技能，又令人欲罢不能地持续精进。在排行榜上名列前茅能为职业生涯带来无可估量的价值，全球猎头都会通过Kaggle物色合适人选，竞赛中获得的知识经验更是职业发展的强力助推器。

## 你如何通过Kaggle构建个人技术履历？

加入Kaggle后，我花费数年掌握了从数据中提取信息、优化指标的各种技术算法与技巧。虽然高准确率是多数竞赛的核心目标，但仅靠运气几乎不可能实现——要赢得比赛或进入金牌区，知识储备与实战经验至关重要。我的Kaggle奖牌数量就是最好的履历证明：截至2021年11月共获得58枚金牌和47枚银牌，这浓缩了我在平台积累的机器学习经验。按每个竞赛至少持续1个月计算，这相当于连续105个月以上的竞技机器学习实践。

## 根据你的经验，新手Kaggle选手常会忽视哪些要点？有哪些现在掌握但希望初学时就知道的知识？

新手往往忽视验证策略的重要性。这种现象不仅存在于Kaggle，全球数据科学家都常会在模型构建中忽略这个实验理论的核心要素。制定验证策略虽无通用准则，但必须考虑模型的实际应用场景，使验证过程尽可能贴近真实使用环境。

## 你在过往竞赛中犯过哪些错误？

错误不胜枚举，几乎试遍了所有可能的错误组合。但错误的价值在于从中学习——只要发现并修正，通常就不会重蹈覆辙。Kaggle选手最常见的错误是过度依赖排行榜分数而忽视本地验证结果。这种对排行榜的过拟合现象与真实项目形成鲜明对比：实际工作中必须建立可靠的验证策略，因为模型将在真实数据上一锤定音，不像竞赛可以每日多次提交。

## 对于数据分析和机器学习，有哪些特别推荐的工具或库？

几年前我可能会推荐\( R \)，但考虑到Python在机器学习领域的迅猛发展及其在生产环境中的通用性和易用性，我现在建议所有机器学习初学者都掌握它。针对表格数据处理，我推荐使用pandas进行数据操作，若追求速度则可选用cuDF（RAPIDS.ai基于GPU加速的pandas版本）。探索性数据分析建议结合Seaborn或Matplotlib库使用DataFrame，机器学习方面推荐Scikit-learn、SciPy、cuML（GPU版）、XGBoost、LightGBM、CatBoost和PyTorch。值得注意的是，使用原始特征构建简单XGBoost模型既快速又能为后续模型比较提供良好基准。

## 参加竞赛时最需要牢记或做到的关键事项是什么？

参加Kaggle竞赛并提交公开Notebook很简单，但进入金牌区却极具挑战性。因此最关键的是要明白——无论最终排名如何，我们都应通过Kaggle享受乐趣，从讨论论坛、公开Notebook乃至赛后优胜者分享的解决方案中汲取知识。更要明白制胜关键不在于复制他人做法，而在于跳出框架提出新颖的思路、策略、架构和方法。

## 您是否使用其他竞赛平台？与Kaggle相比如何？

我在其他平台赢得过几次比赛，但与Kaggle的最大差异在于用户规模。截至2021年11月，Kaggle拥有17.1万活跃用户，这使得论坛互动、Notebook内容和数据集交流都更为丰富。此外Kaggle提供独家优势：可免费使用Google服务器编写运行代码的Notebook，这对缺乏高性能硬件的用户来说价值连城。

## 善用Notebook与讨论区

除竞赛排名外，Notebook是Kaggle上展示能力的重要途径——它同步体现你解决问题的方式、思路呈现能力和编码水平。作为参与者间开放共享解决方案的载体，Notebook是继排名之后最能向雇主证明实力的工具。

近年来数据科学领域最重大的转变，就是从独角兽型天才的 solo 模式转向需要跨部门协作的团队模式。因此企业在招聘时更看重你清晰传达想法的能力、成果展示水平以及编写高效整洁代码的实力。

前文提到实际项目需要更全面的技能，从处理技术债务到设计高性价比方案。即便这些技能不能助你赢得比赛，仍可通过Kaggle展示——Notebook正是最佳载体。

关于Kaggle Notebook的入门指南请参阅第3章《使用Kaggle Notebook工作与学习》。平台上的Notebook大致可分为四类：

- 竞赛排名解决方案与思路

- 数据探索性分析（EDA）

- 机器学习模型或数据科学原理教程

- 论文模型或原创解决方案的新实现

这些都能助你建立独特优势：竞赛方案展示解决复杂数据科学问题的能力，而其他三类则能证明你具备：

- 从数据中提取可视化/非可视化洞见的能力（EDA），这是从科研到商业场景都至关重要的核心技能

- 传授数据科学知识，为从事教育、导师和开发者倡导工作开启大门

- 将研究转化为实践，这项关键技能在数据科学创新（尤其是深度学习领域）日新月异、亟需快速落地为解决方案的时代尤为重要

即便你在Kaggle竞赛中排名不高或没有惊艳的解决方案，只要善于推广，这三类笔记本（探索性数据分析、教程和论文复现）仍能为你创造现实机遇。为此，你需要掌握编写可读性强且引人入胜的笔记本技巧——这需要通过实践积累经验。由于这是门艺术，我们建议向他人学习，特别是用户排名靠前的笔记本大师（https://www.kaggle.com/rankings?group=notebooks&page=1&pageSize=20）。

建议你研究这些大师的笔记本架构：观察他们如何用图表组织内容、构建代码逻辑，然后结合自身专长尝试模仿。请注意，成功不仅依赖代码和图表，叙事能力同样关键。无论是展示解决方案、教学还是用TensorFlow实现神经网络架构，用文字阐释单元格内容对留下深刻印象至关重要。除浏览高分笔记本外，还可关注Kaggle上新出现的非主流精品笔记本。天体物理学家兼Kaggle活跃用户Martin Henze（https://www.kaggle.com/headsortails）每周会在论坛发布"本周隐藏瑰宝"合集，目前已累计100多期。若想获取最新优质笔记本，不妨关注他的Kaggle个人主页。

在借鉴笔记本灵感时，请务必避免无脑抄袭。Kaggle上常见有人稍作修改便将他人的笔记本伪造成原创作品，或选择性移植代码片段却不注明出处。无论哪种情况，都请始终标注原作者及来源——若无法追溯原创者，至少应注明你参考的最后一个笔记本版本。展示自身能力固然重要，但坦然承认借鉴内容更能体现你的专业素养：这既是对同行的尊重，也证明你具备识别优秀成果并加以运用的能力。

Kaggle论坛讨论也能助你在数据科学和软件开发领域获得关注。早期讨论仅用于联系主办方或解决竞赛紧急问题，赛后鲜有人分享解决方案。但随着讨论区引入用户排名和等级体系，论坛已成为重要信息源。

关于Kaggle论坛的详细指南，请参阅第4章《善用讨论论坛》。

根据经验，Kaggle讨论可分为四类：

- 详细解说竞赛解决方案（有时附配套笔记本），阐述团队如何取得特定排名

- 竞赛期间的求助与规则解读

- 致谢、赞美及闲聊

- 指导其他参赛者的教学类帖子

我们发现，精通最后一类讨论并因此获得广泛关注，有助于成为开发者倡导者——尤其当你还拥有与其他数据科学家互动的活跃渠道（如Twitch/YouTube频道、Twitter账号或Medium博客）。

随着大小企业对开发者倡导岗位需求的增长，擅长协助同行完成项目的专家炙手可热。若想深入了解该职位，draft.dev上的这篇文章提供了全面解析：https://draft.dev/learn/what-is-a-developer-advocate。

## 数据集的有效利用

Kaggle竞赛常因提供过于清洁、规整且与现实数据差异较大的数据集而受到批评。但我们持略有不同的观点：发现Kaggle竞赛数据同样可能存在杂乱或噪声较多的情况。有时所提供数据在质量和数量上并不足以支撑获得顶尖成绩，此时需要自行在互联网上寻找补充数据。

Kaggle在数据科学项目中的缺失环节，是数据收集与归档至规范化存储库的过程——这一过程在现实场景中因企业和问题差异而无法标准化。真实世界的数据处理能力主要需通过实践积累。

Kaggle引入数据集功能，正是为了扭转其仅专注建模问题的印象。Kaggle数据集在此方面极具价值：既允许用户创建上传自有数据并记录特征及其取值，又要求用户制定更新频率计划来持续管理数据。

关于Kaggle数据集的入门指南请参阅第2章《用数据集组织数据》。更有趣的是，该平台还支持关联不同分析模型——这些通过Kaggle Notebooks构建的模型，既可源自竞赛成果，也可基于上传数据的深度研究后开发的问题解决方案。

此外，Kaggle数据集提供元信息完整性检查模板。描述、标签、许可协议、数据来源及更新频率等必填信息（用于计算可用性评分）能帮助使用者理解数据用途。用户甚至可在描述或讨论区注明计划利用该数据集开展的待办任务，这能充分展现你对所上传数据潜在价值的理解。

虽然"任务"功能曾属于Kaggle数据集模块（近期已移除：https://www.kaggle.com/product-feedback/292674），但仍可通过数据描述和讨论区说明数据的预期用途。

所有这些特性使得Kaggle数据集成为展示你在Kaggle平台上问题解决经验的绝佳方式，同时也能全面体现你在数据与机器学习算法方面的能力，因为它能让你：

- 发布并维护数据集

- 通过任务路线图证明你已理解数据的价值

- 展示从数据预处理到探索性分析再到预测建模的完整编码解决方案（由于Kaggle Notebooks可直接操作同一数据源，无需额外准备）

我们强烈推荐使用Kaggle数据集来展示你在竞赛或其他项目中的成果，它能将你的工作与他人区分，并实现数据与Notebooks的整合。简言之，Kaggle数据集能向任何人证明你已实现的可运行解决方案。但存在一个局限：你基本被限制在Notebook环境中（即使使用脚本），这对他人了解代码在其他环境运行所需的软件包及版本要求不够透明。实际上，Kaggle Notebooks依赖于由Dockerfile配置文件设定的Docker环境(https://www.docker.com/)，该文件决定了已安装的版本。浏览Notebook时，除非查看这个配置文件，否则无法直观获知所用软件包版本。为此，你可以在GitHub的Kaggle代码库(https://github.com/Kaggle/docker-python/blob/main/Dockerfile.tmpl)找到该Dockerfile以便复现环境设置，但请注意该文件会随时间更新，需追踪与你工作对应的版本。

最后需注意，查看任何数据集及其关联Notebooks都需要具备Kaggle社区访问权限。

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_481.jpg?x=242&y=788&w=361&h=360&r=0"/>

<!-- Media -->

## 加布里埃尔·普雷达

https://www.kaggle.com/gpreda

我们与Endava首席数据科学家、Kaggle数据集/Notebooks/讨论版块三料大师加布里埃尔·普雷达进行了职业发展访谈。这位计算电磁学博士在投身数据科学前深耕软件开发多年，发现Kaggle后如鱼得水，大量投入最终获得丰厚职业回报。

## Kaggle如何助力你的职业发展？

Kaggle极大加速了我的数据科学学习曲线。此前我零散寻找学习资料，效率低下。在Kaggle我找到了志同道合的社区，能观摩顶尖专家的分析模型Notebooks，向他们请教甚至同台竞技。加入初期我主要做数据分析，但很快开始参赛——这意味着学习构建、验证和迭代优化模型。约两年后我成功转行，从软件项目管理转为全职数据科学家。Kaggle还提升了我的行业能见度，现公司面试时就有候选人直言因看到我的履历而应聘。

## 是否将Kaggle作品纳入求职作品集？

我的Kaggle作品集是求职的主要资历证明，LinkedIn资料都直接链接Kaggle主页。近年来雇主对Kaggle认知度提升，有些会专门询问Kaggle档案。当然也有雇主明确不认可Kaggle价值，对此我持反对意见——面试前我必查候选人的GitHub和Kaggle资料，这些能立体展现技术实力（特定语言/工具/技巧的应用）、问题解决能力，更重要的是通过讨论和Notebooks体现的沟通表达能力，这对数据科学家至关重要。

## 你依次获得Notebooks（内核）、讨论和数据集大师称号，能分享这段历程吗？

我成为了第七位Kaggle Kernels大师，并攀升至第三名的位置。约两年时间里，我始终保持在Kernels排行榜前十名。最初编写Kernels主要是为了提升R语言技能，同时分析那些更吸引我的数据集。我尝试了各种技术手段，包括多边形裁剪、构建Voronoi图的对偶网格、二维Delaunay三角剖分等。逐渐地，我开始专注于探索性数据分析，随后转向为数据集和竞赛构建模型。随着参赛频率增加，我也开始用Python编写竞赛专用Kernels。同期，我注意到部分Kernels引起了Kaggle用户的关注——不仅是点赞和分叉，还有积极评论。某些为热门竞赛数据探索编写的Kernels获得了广泛传播，为我赢得大量金牌，最终助我晋升大师及至宗师段位。现阶段我较少发布竞赛相关Kernels，主要专注于为发布的数据集创建入门级Kernels。

随后，我又斩获了Discussions宗师称号。这个成就完全出乎我的预料。最初我只是评论他人的Kernels，随着深入参与竞赛，我的讨论逐渐集中在赛事专区——或是提出竞赛相关议题，或是发起新话题，例如针对某个赛题提出解决方案，或整理应对开放性问题的资源合集。有类特殊评论值得专门提及：作为首批Kaggle Kernels宗师之一，每当发现优质新人作品，我总会点赞并抽空撰写鼓励性评语。特别是对初学者而言，这种正向反馈能极大增强他们的信心，激励他们持续投入Kaggle社区。我曾整理过《Kaggle评论指南》，核心要点包括：言简意赅但不敷衍；内容具体；提供信息而非主观臆断；适时赞美他人作品；保持友善助人态度；避免无意义@他人（仅在定向回复讨论时使用）。

最后达成的是Datasets宗师段位，这也是我排名最高的领域（全球第二）。这个进阶过程相当缓慢，必须基于真正的热爱——构建优质数据集需要持续投入数据整理、清洗和文档编写工作。我选择的主题既关乎个人兴趣，也具备广泛社会价值：从本国选举数据到欧洲社会经济议题，再到全球疫情动态（如COVID-19病例、疫苗接种、病毒变种等）。除常规数值数据外，我还收录Reddit讨论、推特推文等文本数据，其中关于疫苗谣言、板球运动、政治人物等主题的合集最受欢迎。通过自动化脚本实现数据采集、清洗和处理的流程化，不仅节省了时间（对需每小时更新的数据集尤为重要），更提升了数据质量管控。每个新数据集发布时，我都会配套编写入门Kernels——这些并非追求流量，而是作为工具帮助用户理解数据处理技术，通常包含原始数据与经清洗转换后的版本。

## 经营Kaggle之外的线上影响力

由于Kaggle数据集和Notebook需要Kaggle账户，您需考虑到并非所有人都已拥有或愿意专门为此注册账号。还需提供更易访问的替代方案。常见做法包括：在GitHub(https://github.com/)创建项目、在Medium(https://medium.com/)等平台发表文章，或更新个人博客。此外还有以下推广途径：

- 发布与Kaggle竞赛相关的可浏览器执行的代码（使用https://deepnote.com/）

- 创建聚集Kaggle爱好者的Discord社区（如Abhishek Thakur的MLSpace：https://discord.com/invite/4RMwz64gdH），或运营YouTube频道（同作者：https://www.youtube.com/channel/UCBPRJjIWfyNG4X-CRbnv78A）

- 开设Twitch频道（如Rob Mulla的直播频道：https://www.twitch.tv/medallionstallion），演示Kaggle竞赛编程（GitHub项目：https://github.com/RobMulla/twitch-stream-projects）

- 发布Kaggle资讯周报（如Shotaro Ishihara的案例：https://www.getrevue.co/profile/upura）

- 像Sanyam Bhutani那样采访Kaggle选手与数据科学专家，通过视频/播客/博客发布（平台：https://chaitimedatascience.com/；历史采访数据集由Rohan Rao整理：https://www.kaggle.com/rohanrao/chai-time-data-science）

可见推广渠道极为丰富，取决于您的目标。本章重点介绍博客与GitHub（最常见且高效），但您可自由选择适合的方式。

## 博客与出版物

写作既能深化知识（需研读主题才能撰写），又能展示个人能力。通过写作成名可带来多重收益：吸引招聘方关注、拓展Kaggle竞赛及职业人脉。建议善用社交媒体（LinkedIn/Twitter/Facebook）发布观点与短文。鉴于数据科学与Kaggle竞赛需深度讨论，最佳方式仍是撰写长文并通过博客或文章平台发布。建议协调社交媒体与长文推广，用专题帖预告或讨论文章要点。下面介绍发布渠道选择。

在Medium（特别是Towards Data Science等专栏：https://towardsdatascience.com/）发文能获得广泛关注。Medium专栏是围绕特定主题的共享写作空间，通常由多位作者供稿。该平台读者群体庞大，部分专栏在数据科学界以高质量著称。专栏设编辑负责内容筛选，确保符合政策与质量要求。适合投稿的Medium专栏包括：

- 前述的Towards Data Science（https://towardsdatascience.com/questions-96667b06af5）

- Better Programming（https://betterprogramming.pub/write-for-us-5c4bcba59397）

- Mlearning.ai（https://medium.com/mlearning-ai/mlearning-ai-submission-suggestions-b51e2b130bfb）

- Becoming Human（https://becominghuman.ai/write-for-us-48270209de63）

- Towards AI（https://pub.towardsai.net/submit-your-medium-story-to-towards-ai-a4fa7e8b141d）

这些专栏的显著优势是拥有庞大读者群，规模可能远超您的社交媒体粉丝。您将接触到企业人士与潜在合作者，获得超预期的阅读量。

除Medium外，这些网站也可能接收您的投稿：

- Hacker Noon (https://www.publish.hackernoon.com/)：在技术博主中颇受欢迎，涵盖所有科技相关内容（内容非常泛化）。月访问量达四百万人次，是向科技爱好者传播技术类内容的理想平台。但登上首页推荐位难度极大且利弊参半：既会获得大量关注，也会招致诸多批评。

- Dev.to (https://dev.to/)：主要面向开发者受众（近80万用户），主打编程教程与文章。投稿应更注重代码质量与实效性（建模相关内容需弱化处理）。

- FreeCodeCamp (https://www.freecodecamp.org/news/developer-news-style-guide/)：更侧重教程类内容，用户主要来此学习编程。适合推广机器学习课程或新开发的功能包。

- Analytics Vidhya (https://www.analyticsvidhya.com/about/write/)：在印度颇具影响力，专注于机器学习与深度学习基础概念的解析文章。

- KDnuggets (https://www.kdnuggets.com/news/submissions.html)：数据挖掘领域最老牌的出版物之一，在资深数据科学家和学术界仍拥有大量读者（2021年3月独立访客达百万）。

各平台优劣各异且受众不同，需根据内容特性选择最适合的渠道。建议先浏览其刊载内容，了解行文风格适配度。

当然您也可以选择自建博客。自主博客的优势在于不受广告干扰和编辑审查，但需自行通过社交媒体推广来积累读者。既可在自选域名从头搭建网站，也能直接使用GitHub创建技术博客。

若选择GitHub（免费且可能已用作代码仓库），这里有个快速创建博客的指南：http:// jmcglone.com/guides/github-pages/

如需更高自动化方案，Jeremy Howard的fastpages平台(https://github.com/fastai/fastpages)能自动将Notebook和Word文档转化为博客页面并发布，简化代码示例与内容的协同创作。

完全自主建站则需更多精力与资金投入（域名和服务器需付费）。此时内容自推广至关重要。自主写作的优势在于叙事性——需用比Notebook更详实的文字解释代码片段。某种程度上，工作描述与代码本身同等重要。通过调整文风可触及不同受众：通俗化表述能扩大读者群，技术化写作则可能吸引潜在雇主，但会缩小受众面。

写作是高度个性化的行为，我们的建议无法覆盖所有场景。总体原则是预先明确写作目的与目标读者群体。

## GitHub

除了作为文章引用的代码仓库，GitHub还能避免您在每场比赛中重复造轮子。可将复用代码存储在项目或Gists中(https://docs.github.com/en/ github/writing-on-github/editing-and-sharing-content-with-gists)——这是可单独访问的代码片段集。

尽管将代码全留在Kaggle可能很诱人，但长期会导致查找困难。因为Kaggle Notebooks无法按项目分类，仅能通过投票数或最后运行时间等属性排序。GitHub则更便于检索复用，例如创建包含全部代码的脚本后，直接下载导入Kaggle Notebook而无需复制。

以下示例演示了如何下载并复用表格神经网络的辅助函数：

---

!wget https://raw.githubusercontent.com/Imassaron/deep_learning_for_

tabular_data/master/tabular.py

#从Tabular模块导入

from tabular import gelu, Mish, mish

from tabular import TabularTransformer, DataGenerator

---

wget命令可直接访问GitHub上的代码并下载到Notebook磁盘中，随后您只需从中导入所需函数和类。获取代码直链时，只需在GitHub仓库中找到对应文件，点击页面顶部的Raw按钮：

<!-- Media -->

<!-- figureText: Raw Blame -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_488.jpg?x=336&y=441&w=1213&h=187&r=0"/>

图13.1：GitHub文件查看页面的顶部栏。注意右上角的Raw按钮。

<!-- Media -->

点击Raw按钮后，将跳转至GitHub存储该文件的网页地址。此地址可用于在GitHub外部引用该文件。

GitHub还可用于存储Kaggle讨论中需引用的图片（因Kaggle论坛已不支持图片上传）。对于图片，虽无Raw按钮可点击，但可通过右键图片在新标签页打开，效果等同。

GitHub是展示作品的绝佳平台，但鉴于其开发者导向的定位及代码文件为主的内容特性，受众多为技术人士。企业HR通常仅浏览README.md文件，故应确保其内容精炼、版式美观；而招聘经理更关注项目代码质量。建议精心组织文件中的代码结构、流程与类设计，并包含环境安装及结果复现指南。

需使用conda(https://docs.conda.io/en/latest/)或poetry(https://python-poetry.org/)等工具确保依赖包正确安装。推荐采用CookieCutter(https://drivendata.github.io/cookiecutter-data-science/)规范项目结构，其模板能自动生成标准目录架构和说明文档，提升代码可读性与可维护性。此外还需数据版本控制系统（如DVC:https://dvc.org/）管理实验数据。这些工具操作技能更接近软件工程范畴，虽在Kaggle中可简化处理，但掌握后将显著提升GitHub项目质量，增加面试竞争力。

若需模型实时演示，最简单的方式是直接运行原始Notebook（在GitHub项目README.md中添加Kaggle Notebook链接）或使用Google Colab。要将GitHub存储的Notebook自动载入Colab，只需将链接域名从github.com替换为githubtocolab.com。

最震撼的展示方式当属通过HuggingFace Spaces(https://huggingface.co/spaces)部署在线应用。如官方文档(https://huggingface.co/docs/hub/spaces)所述，该平台可免费托管机器学习演示项目（限制16GB内存/8核CPU），支持依赖安装、GitHub代码同步，并能基于Streamlit(https://streamlit.io/)或Gradio(https://gradio.app/)构建应用界面。

例如，Kaggle专家兼哈佛大学教学研究员Rashmi Banthia（https://www.kaggle.com/rashmibanthia）发布了她在Sartorious细胞实例分割竞赛中的模型演示：https://huggingface.co/spaces/rashmi/Cell-Instance-Segmentation-MMDetection。通过实时演示展示模型及示例，即使对非机器学习受众也能直观传达其有效性。

## 关注竞赛更新与新闻简报

由此可见，在Kaggle上展示作品至关重要，这能向世界传达你对特定模型与数据问题的兴趣。因此，及时了解竞赛动态十分关键。主要方式是频繁访问Kaggle官网并订阅邮件通知。你可以在个人资料的"通知与邮件设置"页面开启站内和邮件提醒，还能选择接收包含新功能提示、平台动态以及最新竞赛资讯的邮件：

<!-- Media -->

<!-- figureText: kaggle Hi lucamassaron! Calculating word frequency just scratches the surface of natural language processing In this Snapshots video, Product Manager Meg Risdal walks us through her analysis of Animal Crossing reviews while exploring the Shifterator package's word shift graphs, an alternative to word clouds. She also provides an overview of the Quick Save and Version Naming features in Notebooks! -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_490.jpg?x=392&y=500&w=1104&h=598&r=0"/>

<!-- Media -->

图13.2：Kaggle团队发布的系列视频通知邮件

Twitter用户可通过关注特定账号获取Kaggle动态。Kagoole（https://twitter.com/kagoole）不仅能推送新竞赛信息，其Heroku应用（https://kagoole.herokuapp.com/）还提供往届竞赛解决方案，由Doarakko（https://github.com/Doarakko/）开发。另一个推荐关注的是"Is he Kerneler?"（https://twitter.com/HKerneler），由Regonn（https://github.com/regonn/）创建，实时显示各Kaggle竞赛的剩余时间。

如第一章所述，Kaggle并非唯一举办数据科学竞赛的机构。要全面掌握Kaggle及其他平台（如AICrowd、DrivenData）的竞赛动态，建议使用mlcontests.com或ods.ai/competitions等聚合网站。例如mlcontests.com不仅提供奖金、截止日期等竞赛信息，还包含云GPU性能与价格的横向对比。注册邮箱即可直接接收这些资讯。

## 本章小结

本章探讨了作品展示对职业发展的价值。虽然这些展示无法涵盖你全部的数据科学知识与经验，但仍是彰显能力的重要途径。

作品展示可选择Kaggle内置资源或外部平台。Kaggle提供一体化环境，操作便捷高效；而外部资源（如Medium专栏、GitHub、HuggingFace Spaces等）因被招聘方日常使用，具有更广泛的认知度。

下一章我们将通过探讨人脉构建与面试技巧，完整呈现Kaggle竞赛如何为职业发展赋能。

## 加入本书Discord空间

加入本书Discord工作区，每月参与作者问答会：

https://packt.link/KaggleDiscord

## 第十四章 探索职业新机遇

前章介绍了如何突出竞赛成果，本章将总结Kaggle对职业发展的积极影响。我们将探讨如何将Kaggle经历转化为求职优势——假设你已具备前文所述的所有素材（Kaggle讨论区、笔记本、数据集及衍生GitHub项目），本章将聚焦软性技巧：人脉搭建与经验呈现。

众所周知，人脉网络能带来诸多可能：从获取未公开的职位信息，到获得专业领域的技术支持。在Kaggle上建立人脉主要依靠竞赛期间的团队协作，以及Kaggle用户组织的线下活动。

关于工作机会，正如我们之前多次强调的，Kaggle并非人力资源和招聘经理筛选候选人时广泛认可的参考依据。虽然部分公司会充分考虑你在Kaggle的排名和成就，但这属于特例而非普遍情况。通常你的Kaggle经历可能被忽视甚至遭到质疑。但根据我们的经验，你在Kaggle学到的技能和实践经验极具价值——你可以通过展示编程建模成果，以及阐述个人或团队参赛经历来凸显这些优势。本文将重点介绍：

- 与其他竞赛数据科学家建立联系

- 参与Kaggle Days等线下聚会

- 获得关注与其他职业机遇

## 与其他竞赛数据科学家建立联系

人脉对求职至关重要，它能让你在职位公开前就接触潜在机会。近年来Kaggle已逐渐成为数据科学家交流合作的重要平台。过去竞赛论坛互动稀少，且团队排名因积分均分机制处于劣势。排名计算方式的改进（参见https://www.kaggle.com/general/14196）使组队参赛更受青睐。

若已熟悉队友并建立远程协作机制，Kaggle组队参赛效果显著。这种情况下，每位成员都清楚如何通过以下方式协作：

- 承担团队分配的实验任务

- 与队友协同构建解决方案

- 基于自身专长探索新方案

- 优化模型与提交文件便于集成

但组队新手往往会面临两大难题：加入现有团队或自行组建团队。若无熟人引荐，很难联系排行榜上的选手——有人倾向单打独斗，有人虽有意向却顾虑重重。与陌生Kaggle用户组队时需注意：

- 队员可能无法提供实质性贡献

- 队员可能消极协作坐享其成

- 队员存在违反竞赛规则风险导致团队 disqualification

- 队员可能窃取情报泄露给其他队伍

这些情形在竞赛中大多属于病态现象，你需要意识到，许多人在初次评估是否要与另一名Kaggle选手组队时，都会产生这些常见顾虑。唯有通过展现你作为Kaggle资深玩家的背景——即曾独立参与过若干竞赛、特别是发布过Notebook并参与过讨论——才能消除这些潜在问题的疑虑。这将极大提升你组队提议的可信度，更可能获得团队接纳。

当你成功加入团队后，建立高效且专注的成员沟通机制至关重要（例如通过创建Slack或Discord频道）。同时必须就以下日常协作流程达成共识：

- 确定如何分配实验任务

- 决定如何利用每日有限的提交次数（常引发团队内争议）。最终虽仅由队长选定两份最终提交方案，但达成共识的过程必然伴随讨论与分歧。需准备好向队友展示你采用的本地交叉验证策略及结果，以此说明特定提交方案被选定的依据。

当你们以积极方式完成团队协作后，自然会赢得其他成员的尊重与信任。在未来的竞赛中，你会发现自己更容易与相同伙伴重组战队，或在他们引荐下加入其他团队。

在Kaggle平台上，你将结识并合作的对象包括数据科学家、数据爱好者、学生、领域专家等多元群体。下文我们采访了多位具有代表性的Kaggle用户，听他们讲述日常工作与Kaggle如何融入生活。

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_495.jpg?x=240&y=1667&w=365&h=364&r=0"/>

<!-- Media -->

## 张逸润

https://www.kaggle.com/gogo827jz

张逸润是伦敦国王学院的博士候选人，同时保持着Kaggle Notebooks和Discussion双料大师头衔。他曾作为冠军队成员参与Jane Street市场预测竞赛(https://www.kaggle.com/c/jane-street-market-prediction)。

## 请做个自我介绍

我的研究方向聚焦于运用机器学习算法解决现代无线通信网络中的时序预测、资源分配及优化等难题。同时参与涉及AI隐私、联邦学习、数据压缩与传输的研究项目。

除日常博士研究外，我从博二开始活跃于Kaggle近两年。参赛首秀是Instant Gratification竞赛，期间综合运用了sklearn库中多种机器学习与统计方法。这场竞赛让我建立起对Kaggle建模流程的系统认知。

我持续通过Notebooks和论坛帖与社区分享知识，现已成为Kaggle双料大师。在交流中获得宝贵反馈与新知，这些积累助力我最终在近期竞赛中斩获冠军。

## 谈谈你们的夺冠经历

Jane Street市场预测是场硬仗。难点在于构建稳健的交叉验证(CV)策略——许多人直接使用公开排行榜作验证集，训练神经网络数百个epoch却未采取防过拟合措施。我们团队坚持自主CV策略，最终在排名震荡中胜出。

## Kaggle竞赛与日常工作有何差异？

Kaggle竞赛与博士研究截然不同：前者节奏紧张且反馈即时，后者则是长期工程。但我在竞赛中习得的新知与方法论对研究工作大有裨益。

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_496.jpg?x=245&y=1756&w=354&h=359&r=0"/>

<!-- Media -->

## 秋山修

https://www.kaggle.com/osciiart

秋山修（网名OsciiArt）是大阪大学医院的医师，本职不涉及数据科学，但保持着Kaggle竞赛大师称号。

## 请做个自我介绍

我是大阪大学医院的二年级住院医师，毕业于京都大学生命科学硕士专业。曾在制药企业从事研发工作，后转入大阪大学医学部并取得日本医师执照。

因AlphaGo的震撼开始自学数据科学与人工智能，为检验学习成果开始参与Kaggle竞赛。2017年首次参加NOAA渔业斯特勒海狮种群统计大赛，持续活跃至今已获得三枚金牌。

## Kaggle对您的职业发展有何帮助？

由于缺乏信息科学专业背景，我在申请AI公司实习和AI实验室短期研修时，都用Kaggle成绩证明自身能力。虽然本职是医生，但得益于Kaggle战绩，我偶尔能参与医疗数据研究项目。

## 您最青睐哪种竞赛类型？原因是什么？

最钟爱医疗数据类竞赛，享受运用医学知识从数据中挖掘洞见的过程。

## 您如何开展Kaggle竞赛？

热衷于发掘其他选手未察觉的数据特性，或针对竞赛数据特点尝试独特解法。虽然这类尝试大多失败，但探索过程充满乐趣。

## 请分享一次特别具有挑战性的参赛经历及解题思路

2019年Freesound音频标注大赛令我印象深刻，这是个声音数据多标签分类任务。训练集由少量精准标注数据（干净数据）和大量不可靠标注数据（噪声数据）组成，且两类数据分布存在差异。我们采用双重策略：其一是将噪声数据训练视为独立于干净数据的多任务学习；其二是通过伪标签技术（半监督学习的一种），用干净数据训练的模型预测结果重新标注噪声数据。

## 您是否使用其他竞赛平台？与Kaggle相比如何？

还使用日本的数据科学竞赛平台Signate(https://signate.jp/)和guruguru(https://www.guruguru.science/)。这些平台规模较小，数据集通常比Kaggle更精简，参赛门槛较低。有时还会举办Kaggle上没有的特色赛事。

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_498.jpg?x=247&y=680&w=351&h=353&r=0"/>

<!-- Media -->

## Mikel Bober-Irizar

https://www.kaggle.com/anokas

Mikel Bober-Irizar（昵称Anokas）是竞赛领域双料大师（竞赛大师/笔记本讨论大师），ForecomAI机器学习科学家，剑桥大学计算机科学专业学生，也是Kaggle史上最年轻的总冠军。

## 能否介绍一下自己？

2016年14岁时初涉Kaggle，当时刚接触机器学习觉得酷炫就懵懂参赛。最初几场比赛全靠复制论坛公开代码并微调，通过不断冲击排行榜逐渐掌握要领，同年即在Avito重复广告检测竞赛中获得亚军。

自那时起，我已参与75场竞赛，并于2018年成为最年轻的竞赛特级大师（Grandmaster）及首位三冠大师（Triple Master）。此后我担任萨里大学客座研究员，目前正在剑桥大学攻读计算机科学，同时从事机器学习与安全领域的研究。

## 你最喜欢哪类竞赛？为什么？在技术方法和解题思路上，你在Kaggle的专长是什么？

我特别热衷需要大量特征工程的竞赛，以及包含多元数据类型的赛题——这类竞赛能让你充分发挥解题创意，比那些要求所有人采用相同方法、只为小数点后几位拼杀的比赛有趣得多。

我不认为自己有特定的方法论专长，但乐于尝试不同方案。

## 请分享你参加过最具挑战性的竞赛，以及你用来攻克任务的关键洞察。

几年前谷歌举办过图像内物体及其关系检测竞赛（如"椅子在桌边"）。其他团队花费大量时间采用传统方法训练大型神经网络，而我当时既缺乏相关知识也没有足够算力竞争。我另辟蹊径，运用精妙的启发式方法和树模型，仅用几小时工作就获得第七名。

## Kaggle对你的职业发展有帮助吗？

Kaggle为我带来无数机遇，也是一个极佳的交流社区。通过参赛我结识了许多人并学到大量知识。更重要的是，Kaggle正是我进入机器学习领域的起点——若非如此我可能不会涉足这个领域。所以是的，它对我的帮助难以估量。

## 你在过往竞赛中犯过哪些错误？

很容易陷入无法复现复杂解决方案的困境，因为最终方案往往混合了多个代码版本和中间数据集。若幸运获奖，向主办方交付可运行代码时会压力巨大！当进展顺利时，最好及时确定解决方案并整理代码。

另一个常见错误是为不同模型使用不同验证集，或未保留验证预测结果，这会阻碍模型比较或在竞赛后期进行元学习。

## 有哪些特别推荐的数据分析或机器学习工具/库？

我特别推荐XGBoost——它在表格数据上仍常胜于神经网络（其新近分支LightGBM也是）。SHAP非常适合解释模型（包括复杂模型），能为你提供后续尝试方向的洞见。

## 参加竞赛时最重要的注意事项是什么？

我认为关键是要避免陷入超复杂方案的泥潭，而应尝试渐进式改进。现在的竞赛比我初入时困难许多，参考他人公开的竞赛代码并从中学习是明智之举。不妨考虑与其他Kaggle用户组队：团队竞赛始终是我最享受的参赛形式，总能带来绝佳的学习体验。

最后提醒：多数创意终将失败——若想赢得竞赛，必须坚持不懈持续实验！

Kaggle无疑深刻影响了前三位受访者丰富多彩的人生与职业轨迹，而他们的征程才刚刚开始。下面我们将对话两位已在各自公司担任高管的Kaggle用户，他们同样因Kaggle经历了漫长而硕果累累的成长之旅。

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_500.jpg?x=244&y=898&w=354&h=355&r=0"/>

<!-- Media -->

## 3.

https://www.kaggle.com/dansbecker

首先是DataRobot决策智能产品副总裁、Notebooks特级大师Dan Becker。Kaggle在他职业生涯中扮演了重要角色。

## 能否介绍一下您的经历？

2000年在一家三人初创公司，我首次尝试用机器学习帮助零售商优化eBay商品保留价，当时我们试图运用神经网络却完全不得要领，最终惨败收场。

到2002年，我确信机器学习根本行不通。后来取得经济学博士学位后，我在美国政府担任经济学家。当我想搬去科罗拉多州时，发现当地鲜有需要经济学博士的岗位，于是开始寻求非学术领域的资质证明。

2010年，我看到报纸报道Heritage Health Prize竞赛——这是Kaggle早期举办的奖金\( \$ 3 \)百万美元赛事。当时我仍相信经济学家使用的简单模型会比花哨的机器学习预测更准。抱着"好成绩能助我在科罗拉多找到理想工作"的念头，我开始了比赛。首轮提交虽非垫底，却也相去不远。目睹自己的模型评分被众人远远甩开时，我心都凉了。虽短暂放弃过获胜希望，但不甘平庸的我开始夜以继日地钻研。重新学习这十年间突飞猛进的机器学习技术后，我每天更新模型，虽耗时却欣喜地看着排名节节攀升。当跻身中游时，我意识到继续努力或能冲进前十名。

当我进入前十时，一家分析咨询公司联系我，邀请以他们名义参赛用于营销，条件是允许我在科罗拉多工作。就这样，Kaggle竞赛帮我实现了最初目标。

我们最终获得亚军。虽无奖金，但这次竞赛成就了我之后的所有职业发展，其成功远超我的想象。

## Kaggle还如何影响了您的职业？

Kaggle几乎塑造了我的整个职业生涯：首份数据科学家工作来自排行榜上的猎头邀约；后来先后任职Kaggle公司和以招募Kaggle优胜者为策略的DataRobot；再回到Kaggle创建数据科学教育平台Kaggle Learn。可以说过去十年每份工作都源于当初在Kaggle的成功。

从经济学转行数据科学时，Kaggle战绩是我被录用的关键。如今资深如我虽不再需要作品集，但很庆幸总是工作找上门来。

## 您最青睐哪类竞赛？在技术方法上有何专长？

作为社区老人，我已有七八年未全力投入比赛，但始终钟情新颖赛制。比如2013年通过Kaggle首届深度学习竞赛首次接触该领域——那是在Keras、TensorFlow等框架出现之前，整个社区都在论坛里共同探索这项全新技术。

Kaggle还举办过对抗建模赛，选手需构建能通过微调图像欺骗其他模型的系统。这种实验性赛事独具魅力，虽然未必会再举办，但我特别享受这种整个社区在论坛集体攻关的体验。

## 您如何制定Kaggle竞赛策略？与日常工作有何不同？

最近几次参加比赛时，我专注于"能为这个比赛开发什么工具来实现跨项目工作自动化"。虽然成效不彰，但这个挑战很有趣，与我处理其他专业事务的方式截然不同。

在比赛之外，我痴迷于分析学，热衷于研究各类有趣主题的数据。我常说作为数据科学家的优势就是能直接观察数据（不经过ML模型过滤的方式）。

我也经常思考如何从ML模型的预测推导出决策。例如当模型预测杂货店在下批进货前能卖出1000个芒果时，实际应该囤多少货？有人想当然认为是1000个...正好等于预测销量。这是错误的。

必须权衡囤货过多导致腐烂的成本与缺货损失的成本，还要考虑芒果保质期。能否将超额库存维持到下次进货？这类优化问题是我日常工作的重要部分，但在Kaggle比赛中不会出现。

请分享你参加过最具挑战性的比赛，以及你用来解决问题的洞见。

在Practice Fusion糖尿病分类挑战赛中，我尝试构建自动化系统来处理数据连接和特征工程。最大的教训是：当文件数量较多时，仍需人工检查数据以确定合理的特征工程方案。

## 根据你的经验，新手Kaggle选手常忽视哪些要点？你现在掌握了哪些希望初学时就知道的知识？

新人往往低估了在Kaggle比赛中取得好成绩的门槛。他们以为用通用方法就能轻松进入前50%...这通常不现实。最让我惊讶的是在集成模型时，利用排行榜分数为不同模型分配权重的价值。

## 你在过往比赛中犯过哪些错误？

我多次在多阶段比赛的最终提交环节搞砸细节（结果排名垫底或接近末尾）。

# 有哪些特别推荐的数据分析或机器学习工具/库？

主要还是标准工具链。

在Kaggle之外，我个人偏爱用Altair做可视化...同时大量编写SQL。SQL虽不适合构建复杂模型，但擅长简单聚合和趋势分析，我认为这恰恰是其优势而非缺陷。

<!-- Media -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_503.jpg?x=249&y=713&w=343&h=350&r=0"/>

<!-- Media -->

## 李正允

https://www.kaggle.com/jeongyoonlee

最后是李正允，这位多次获奖的竞赛大师现任Netflix研究院排名与搜索算法工程团队高级研究科学家。

## 能介绍一下你自己吗？

我是Jeong，现任Netflix高级研究科学家。2011年完成博士学位后，我加入分析咨询初创公司Opera Solutions时创建了Kaggle账号。在那里我结识了包括Michael Jahrer在内的Kaggle狂热爱好者，我们共同参与了KDD杯和Kaggle竞赛。此后即便离开公司，我仍以参赛者和组织者身份持续参与竞赛。如今虽不像从前那样投入大量时间，但仍会定期关注以学习机器学习领域的最新工具与方法。

## Kaggle对您的职业发展有帮助吗？

帮助巨大。首先它提供了机器学习领域的资质证明——无论是当我作为应聘者时遇到的招聘经理，还是作为面试官时接触的候选人，都提到过被我的Kaggle竞赛记录所吸引。其次，它能学习最前沿的机器学习方法。通过参与跨领域百余场竞赛，我掌握的解决方案比同行更丰富。第三，这里汇聚了全球顶尖数据科学家网络——我在Kaggle结识众多杰出同行并享受协作：翻译过Abhishek Thakur的著作，与Mario/Giba/Abhishek在KDD组织专题讨论，目前正为Luca的书籍进行访谈。2012年加入新公司后，我运用Steffen Rendle在KDD杯提出的因子分解机，一个月内将预测性能较原有SVM模型提升\( {30}\% \)。在联合创立的初创公司，我们的核心卖点是超越市场标准线性回归的集成算法。在Uber任职期间，我引入对抗验证来解决机器学习流程中的特征协变量偏移问题。

## 您最青睐哪类竞赛？在技术方法层面，您在Kaggle的专长是什么？

偏好中小型数据集竞赛（多为表格数据），这样即便用笔记本也能随时随地进行快速迭代。2015年参赛高峰期，我常在飞机上或照顾三胞胎的间隙构建解决方案——孩子们2014年底出生时，我正任职于联合创办的初创公司。

我认为自己并无特殊建模技术，专长在于竞赛管理：包括招募队员、搭建协作框架（如Git/S3/Messenger/Wiki/内部排行榜/交叉验证分割）、协助团队高效运作等。因此虽非个人竞赛大师，但因其他大师愿与我合作，仍能跻身前十。

## 您如何规划Kaggle竞赛？与日常工作有何不同？

致力于构建支持快速迭代和渐进改进的流程。尝试越多创意，竞赛表现越佳——这一原则同样适用于日常工作。区别在于范畴：工作中需从定义问题和确认数据开始，而Kaggle竞赛这两者已给定，我们从探索性分析起步。

## 据您观察，新手常忽视什么？现在掌握哪些希望初学时就知道的经验？

近来发现许多用户直接复刻他人分享的Notebook并微调得分。但真正重要的是学习过程而非排名积分。建议新手多花时间构建原创方案。

参与竞赛时最应牢记什么？

重在求知，非为胜负。

# 您使用其他竞赛平台吗？与Kaggle相比如何？

现任韩国机器学习竞赛平台Dacon AI顾问。该平台2018年创立至今已举办96场竞赛，虽处发展初期，但为韩国用户提供了类似Kaggle的体验。

## 关于参与Kaggle Days及其他线下活动

结识其他Kaggle用户（及更容易加入团队）的有效方式就是线下见面。即便非Kaggle主题聚会，演讲者常会分享参赛经验或涉及竞赛相关主题——例如许多研究类竞赛要求优胜者撰写论文，这些成果可能在会议演讲中被引用展示。

直到2018年，由Maria Parysz和Pawel Jankiewicz创立的LogicAI公司与Kaggle合作，在波兰华沙举办了首届Kaggle Days活动，才出现了与Kaggle直接相关的特殊事件。他们聚集了100多名参与者和8位Kaggle大师级人物作为演讲嘉宾。

随后举办了更多Kaggle Days活动。以下是已安排的各项活动，附有相关资料和演讲的链接：

- 2018年5月，华沙 (https://kaggledays.com/events/warsaw2018)

- 2019年1月，巴黎 (https://kaggledays.com/events/paris2019)

- 2019年4月，旧金山 (https://kaggledays.com/event/sanfrancisco2019)

- 2019年4月，迪拜 (https://kaggledays.com/events/dubai2019)

- 2019年10月，北京 (https://kaggledays.com/events/beijing2019)

- 2019年12月，东京 (https://kaggledays.com/events/tokyo2019)

从巴黎的第二场活动开始，还在多个城市举办了小型见面会（30个不同地点超过50场）。无论是参加大型活动还是见面会，都是结识其他Kaggle用户并建立友谊的绝佳机会，对职业发展或组队参加未来Kaggle竞赛都大有裨益。事实上，本文作者之一正是通过这种方式找到了下一份工作。

## 获得关注与其他工作机会

曾几何时，Kaggle是雇主寻找数据分析和机器学习建模稀缺人才的热门平台。Kaggle在讨论区设有招聘版块，众多招聘方会浏览排行榜物色人选。企业或通过举办竞赛直接招募人才（Facebook、英特尔和Yelp都为此举办过招聘竞赛），或在看到选手在特定类型问题上的出色表现后招揽优秀参赛者（如保险公司AXA在其远程信息处理竞赛后所做的那样）。《连线》杂志对Gilberto Titericz的采访标志着这一现象的巅峰，报道称"排名靠前的解题者会收到大量工作邀约"(https://www.wired.com/story/solve-these-tough-data-problems-and-watch-job-offers-roll-in/)。

近来情况有所变化，许多Kaggle用户反映，在比赛中获胜或取得好成绩后，最多只能期待招聘方几个月的联系。让我们看看变化的原因与现状。

如今，要求Kaggle经验的工作机会已不多见，因为企业通常更看重相关领域工作经验（最好是同行业或同知识领域）、数学密集型学科的学术背景，或谷歌/亚马逊/微软的认证。Kaggle经历仍会带来以下优势：

- 被关注Kaggle排名和竞赛的招聘人员发现

- 获得企业青睐，因为许多管理者和人力资源部门会留意Kaggle个人资料

- 提供编程和机器学习能力的证明，可能免去额外测试环节

- 获得特定公司高度相关问题的实战经验（如远程信息处理、欺诈检测或深度伪造等Kaggle竞赛主题），这些经验因数据非公开而难以通过其他途径获取

然而，企业很少会直接采信你的比赛成绩和排名，因为很难区分哪些成果真正体现了你的技能，哪些是招聘方不太关注的其他因素所致（例如你能投入竞赛的时间、硬件条件或运气成分）。

在以下情况下，你的Kaggle排名和成绩更容易受到关注：

- 你在某场竞赛中表现出色，而该竞赛的问题对企业特别重要。

- 你围绕企业关注的主题在多项竞赛中持续取得好成绩，这证明你具备真实能力，而非仅是无实质基础地自诩为"数据科学家"或"机器学习工程师"。

- 通过参与Kaggle，你展现出对数据分析的真正热情，甚至愿意无偿投入业余时间。这虽是加分项，但也可能成为双刃剑——若未能展现对自身价值的认知，可能导致薪资报价偏低。

虽然Kaggle排名和成绩本身未必是决定性因素，但能成为差异化优势。招聘方可能据此筛选潜在候选人。最受关注的是竞赛和Notebook板块排名（因此这两个领域竞争最激烈，顶级大师数量也最多），但特定竞赛的排名有时也会被留意。当企业寻求某些稀缺能力（如NLP或计算机视觉）时，在需要娴熟运用这些技能才能获胜的竞赛中更容易发现人才。

另一个重要差异点出现在面试环节。你可以引用参赛经历来展示问题解决思路、代码实现方式以及与队友的协作过程。此时比起Kaggle排名或奖牌，更重要的是讨论具体细节：竞赛涉及的行业领域、处理的数据类型及其吸引力，并运用STAR法则（职场面试常用方法）阐述你在竞赛中的行动。

## STAR法则

运用STAR法则时，你应按照情境(Situation)、任务(Task)、行动(Action)、结果(Result)的框架组织参赛经历。该方法侧重行为描述而非技术细节，强调个人能力而非算法性能——他人或许采用相同算法，但成功实施的关键在于你。

该方法主要适用于成功案例，但也可用于失败经历，尤其是那些让你获得重要洞见、避免重蹈覆辙的情况。

## 应用该方法需将经历分解为四个要素：

- 情境：描述背景和细节，让面试官快速理解问题与机遇

- 任务：说明你在该情境中的具体职责，突显个人技能与行为层面的贡献

- 行动：阐述你为完成任务采取的具体措施

- 结果：说明行动带来的具体成效及整体成果

部分公司会明确要求使用STAR法则（或其衍生方法GICF，即目标-影响-挑战-发现法则，更强调结果）；其他公司虽不明确要求，但期待类似的表述逻辑。

最佳答案应契合你所面试公司的价值观与目标。

仅汇报比赛中的排名和奖牌可能不足以打动面试官，因此重构你在Kaggle竞赛中的成功经验至关重要。无论你是个人参赛还是团队协作，这种方法都适用；若是后者，需重点描述你如何与队友互动并产生积极影响。下面我们探讨具体实施方式。

首先，阐述竞赛中出现的情境——可能是初期阶段、实验阶段或最终收尾阶段。提供清晰背景至关重要，这能让听者判断你的应对是否得当。需详尽描述该情境及其需要你关注和行动的原因。

接着说明你承担的具体任务，例如数据清洗、探索性分析、建立基准模型或持续优化解决方案。

然后描述任务执行过程。若能配合Medium技术文章或GitHub项目（如前一章所述）将极具说服力。通过规范的文档和优质代码系统化展示你的经验与能力，能强化面试官对你价值的认可。

最后阐明取得的成果，可以是定性描述（如协调Kaggle团队协作）或定量数据（如你的贡献对最终结果的影响程度）。

## 总结（与临别赠言）

本章探讨了Kaggle竞赛如何助力职业发展，涉及通过组队参赛和往届赛事活动建立人脉，以及将Kaggle经验转化为求职优势。根据我们及其他Kaggle用户的经验，仅凭竞赛成绩无法确保获得职位，但能吸引招聘方关注，并佐证你在数据科学领域的能力（需配合前一章所述的精心构建的作品集）。

本章也是全书的终章。通过14个章节，我们系统讲解了Kaggle竞赛、数据集、Notebook和技术讨论，涵盖从评估指标到模拟竞赛等机器学习与深度学习技术主题，旨在帮助你在Kaggle平台内外获得更大成就。

作为十年Kaggle参赛者，我们深知平台虽包罗万象，但知识分散于数百场竞赛、数千份Notebook和讨论中。对新手而言，及时获取所需信息颇具挑战。本书萃取了参与各类竞赛必备的核心知识，因此这并非传统意义上的数据科学著作，而是专精于Kaggle平台的数据科学实战指南。

除技术实践建议外，我们更想传递：十余年来，我们始终能将Kaggle经历转化为宝贵财富。你可将本书视为我们在数据科学竞赛领域的探索实录。Kaggle之旅不会因获得宗师头衔或全球第一而终结——它永无止境，因为参赛方式和经验应用存在无限可能。本书的终结正是你Kaggle征程的开始，愿你如我们一般，收获漫长而丰硕的旅程。祝君前行无疆！

## 加入本书Discord空间

加入本书Discord工作区，每月参与作者问答专场：

https://packt.link/KaggleDiscord

##

<!-- Media -->

<!-- figureText: Packt> -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_511.jpg?x=241&y=208&w=741&h=243&r=0"/>

<!-- Media -->

packt.com

订阅我们的在线数字图书馆，畅享7,000余本图书和视频，以及行业领先的个人发展规划与职业进阶工具。详情请访问官网。

## 订阅优势

- 向4000多位行业专家学习实用电子书和视频教程，减少学习时间，增加编码实践

- 使用专为您定制的技能计划提升学习效率

- 每月免费获取一本电子书或视频

- 全站搜索功能助您快速获取关键信息

- 支持内容复制粘贴、打印及添加书签

访问www.packt.com，您可阅读免费技术文章合集，订阅各类免费通讯，并获取Packt书籍和电子书的独家折扣与优惠。

## 您可能感兴趣的其他书籍

若喜欢本书，您可能对Packt以下书籍也感兴趣：

<!-- Media -->

<!-- figureText: EXPERT INSIGHT Python Packty Machine Learning with PyTorch and Scikit-Learn Develop machine learning and deep learning models with Python PyTorch book of the bestselling and widely acclaimed Python Machine Learning series PyTop Source 2000 Source Yuxi (Hayden) Liu Vahid Mirjalili -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_513.jpg?x=247&y=879&w=438&h=534&r=0"/>

<!-- Media -->

PyTorch与Scikit-Learn机器学习实战

塞巴斯蒂安·拉什卡

刘玉溪（海登）

瓦希德·米尔贾利利

## ISBN: 9781801819312

- 探索机器从数据中"学习"的框架、模型与技术

- 使用scikit-learn进行机器学习，PyTorch进行深度学习

- 训练针对图像、文本等数据的机器学习分类器

- 构建并训练神经网络、Transformer模型和提升算法

- 探索模型评估与调优的最佳实践

- 使用回归分析预测连续目标结果

- 通过情感分析深入挖掘文本与社交媒体数据

<!-- Media -->

<!-- figureText: DOPERTINSIGHT Packty Transformers for Natural Language Processing for NLP with Python, PyTorch, TensorFlow, BERT, and CPT-3 Foreword by: Office of the CTO, Good Second Edition Denis Rothman -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_515.jpg?x=247&y=212&w=421&h=519&r=0"/>

<!-- Media -->

自然语言处理中的Transformer模型 - 第二版

丹尼斯·罗斯曼

## ISBN: 9781803247335

- 探索使用最新预训练Transformer模型执行NLP技术的新方法

- 掌握原始Transformer、GPT-3、BERT、T5、DeBERTa和Reformer的工作原理

- 了解ViT和CLIP如何标注图像（包括模糊图像！）以及使用DALL-E重建图像

- 使用TensorFlow、PyTorch和GPT-3执行情感分析、文本摘要、非正式语言分析、机器翻译等任务

- 评估关键Transformer模型的生产力，界定其在生产环境中的适用范围、潜力与局限

<!-- Media -->

<!-- figureText: for Time-Series Python Machine Learning Packty with Python Ben Auffarth -->

<img src="https://cdn.noedgeai.com/01970ccf-8d28-7636-9a5e-35a0547e8bf1_516.jpg?x=247&y=212&w=429&h=529&r=0"/>

<!-- Media -->

## Python时间序列机器学习

本·奥法特

## ISBN: 9781801819626

- 理解时间序列的主要类别，学习检测异常值与模式

- 选择正确方法解决时间序列问题

- 通过自相关和统计技术分析季节性与相关性模式

- 掌握时间序列数据可视化

- 理解经典时间序列模型如ARMA和ARIMA

- 实现深度学习模型，包括高斯过程、Transformer及前沿机器学习模型

- 熟悉Prophet、XGBoost和TensorFlow等众多库

## Packt正在寻找像您这样的作者

若您有兴趣成为Packt作者，请访问authors.packtpub.com立即申请。我们已与数千名开发者和技术专业人士合作，帮助他们与全球技术社区分享见解。您可以提交通用申请，应征我们正在招募的热门专题作者，或提交自己的创意。

## 分享您的想法

现在您已完成《Kaggle竞赛宝典》阅读，我们期待聆听您的见解！若从亚马逊购买本书，请点击此处直达本书亚马逊评价页面分享反馈，或在原购买站点留下评论。

您的评价对我们和技术社区至关重要，将帮助我们确保持续提供优质内容。

## 符号表

632自助法 172

A

准确率 114

采集函数 261, 295

自适应过拟合 150

对抗性测试 25

对抗性验证160,180

示例 181, 182

使用 179-181

人工智能伦理

参考链接 74

秋山修 472, 473

albumentations（图像增强库）346, 347

特性 346

阿里云 11

参考链接 11

AlphaZero（阿尔法零）

参考链接 431

分析竞赛 19

Analytics Vidhya（分析维迪亚）11, 462

参考链接 11

年度竞赛 18

## 索引

注意力机制 288

AUC评估指标 105

数据增强技术

图像增强 335

文本增强 414

自相关 166

自编码器

去噪自编码器 226-230

AutoGluon框架 330

AutoViz工具

参考链接 204

平均精确率 118

前\( k \)项平均精确率(AP@K) 134

平均集成技术 307-309

B

装袋技术 305

基础优化技术 242

网格搜索 243-245

折半搜索 246, 247

随机搜索 245, 246

基础技术：文本增强

策略

置换法 417-420

同义词替换 415, 416

贝叶斯优化 261

自定义 268-276

扩展至神经架构搜索 276-285 BayesSearchCV函数 268 贝克尔·丹 476 巴蒂亚·鲁奇 299-301 偏差与方差 157, 158 双变量分析 204 混合法 276, 317 优势 317 最佳实践 318-323 劣势 318 博伯-伊里扎尔·米克尔 474 自助法 171-173 博鲁塔 222 BorutaShap 222 瓶颈去噪自编码器 227 边界框 130, 357 校准函数 143 CatBoost 257 参数 257, 258 参考链接 213 网址 257 切斯勒·瑞安 174 分类任务 二分类 100 评估指标 114 多分类问题 101 多标签问题 101 任务类型 100 CodaLab平台 11 参考链接 11

代码竞赛 22

决定系数 110

科恩卡帕系数 124

列块 256

常见物体上下文数据集(COCO) 372

通用任务框架(CTF)

范式 23

社区竞赛 19

竞赛类型 17

分析竞赛 19

年度赛 18

挑战解决方案 24-26

代码竞赛 22

社区竞赛 19

精选赛 17

新手入门赛 18

大师赛 18

练习赛 19

招聘竞赛 18

研究赛 18

竞赛页面，Kaggle 12

代码菜单 14

数据菜单 14

概览菜单 14

规则菜单 14

复杂堆叠与混合解决方案

创建 329, 330

计算资源 26

概念漂移 184

conda

参考链接 464

混淆矩阵 115

连接

建立，与竞赛数据科学家

470,471

Connect X 426

智能体 427

展板427

参考链接426

提交材料，建筑427-430

科昂，泽维尔 331

CookieCutter（模板工具）

参考链接464

相关矩阵314

成本函数99

批评意见，Kaggle竞赛33,34

交叉熵119

交叉验证策略

平均法315,316

交叉验证预测函数

参考链接171

CrowdANALYTIX（众包分析平台）10

参考链接10

CTGAN 196

D

达内塞，阿尔贝托 259-261

数据

收集 42

规模，缩减 208, 209

数据增强 335

数据泄露 187

数据科学竞赛平台 4-6

阿里云 11

分析维迪亚 11

CodaLab 11

CrowdANALYTIX 10

DrivenData 10

Kaggle竞赛平台 7

次要平台 11

Numerai 10

Signate 10

Zindi 10

数据集

利用 455, 456

设置 37-41

操作指南 48, 49

数据版本控制系统(DVC) 465

URL 201

深度神经网络(DNNs) 276

深度堆栈去噪自编码器 228

去噪自编码器(DAEs) 227, 229

瓶颈式去噪自编码器 227

深度堆栈去噪自编码器 228

克里斯·迪奥特 338, 347

Detectron2目标检测平台 371

开发者社区(Dev.to) 462

戴斯系数 132

Kaggle讨论论坛

书签功能 85

讨论方法示例 86-89

过滤 83

竞赛页面 84

网络礼仪 92

工作流程 79-81

DistilBERT模型 393

测试数据分布

处理 183, 184

训练数据分布

处理 183, 184

道arakko

URL 466

Dockerfile文件 457

DrivenData平台 10

参考链接 10

E

早停法 354

高效网络B0架构(EfficientNet B0) 350

嵌入向量(embeddings) 404

经验贝叶斯方法(empirical Bayesian approach) 218

集成算法(ensemble algorithms) 304, 305

集成选择技术(ensemble selection technique) 320

集成学习(ensembling) 303, 304

平均化技术(averaging techniques) 305

模型平均化(models, averaging) 308, 309

策略(strategies) 305

训练案例采样(training cases, sampling) 308

误差函数(error function) 100

评估指标(evaluation metric) 98

自定义指标(custom metrics) 136-139

自定义目标函数(custom objective functions) 136-139

优化(optimizing) 135

探索性数据分析(exploratory data analysis, EDA) 20, 453

降维

使用t-SNE算法 205-207

降维

使用UMAP算法 205-207

显著性检验 203-205

极端随机树 252

F

F1分数 119

fast.ai框架

参考链接 8

fastpages工具 462

F-beta分数 119

精选竞赛 17

特征工程技巧

特征重要性评估

实际应用 220-222

特征衍生 211-213 基于列的元特征 213, 214 基于行的元特征 213, 214 目标编码 215-220

特征泄漏 188

芬克，劳拉 384

分支 57

自由代码营 462

## G

## 游戏人工智能

参考链接 73

几何平均数 312

入门竞赛 18

示例 18

代码片段 463

GitHub

笔记本，保存至 60-62

全球小麦检测竞赛

参考链接 357

目标-影响-挑战-发现方法 484

谷歌云平台 (GCP)

升级至64-66

Google Colab 465

Kaggle数据集，使用49-51

参考链接49

Google地标识别2020

参考链接18

Gonen，首次442

梯度提升305

梯度树提升253

Gradio

网址465 网格搜索242-245

GroupKFold

参考链接166

H

黑客午报461

Halite游戏439, 440

棋盘440

参考链接439

二分搜索246, 247

调和平均数312

Martin Henze 70-72

Heroku应用

URL 466

HistGradientBoosting算法258, 259

超参数258

HuggingFace Spaces平台

URL 465

超带优化285

Hyperopt优化库296

图像分类

问题处理349-356

ImageDataGenerator方法341-344

模仿学习441

独立同分布152

实例分割130

标注间一致性(inter-annotation agreement) 124

中级机器学习(Intermediate ML)

参考链接(reference link) 73

四分位距(interquartile range, IQR) 213

交并比(intersection over union, IoU) 131, 377

石原正太郎(Ishihara, Shotaro) 412

保序回归(isotonic regression) 143

迭代分层(IterativeStratification)

参考链接(reference link) 165

J

杰卡德指数(Jaccard index) 131

詹森·朱利亚诺(Janson, Giuliano) 184

K

Kaggle应用程序接口(API) 14

竞赛类型(competitions types) 17

参考链接(reference link) 14

Kaggle数据集

法律免责条款(legal caveats) 51, 52

参考链接37

在Google Colab中的使用49-51

Kaggle Days活动30, 481

Kaggle学习平台

课程73-76

参考链接73

Kaggle线下聚会

参与方式481

Kaggle新手社区

参考链接29

Kaggle笔记本14, 27, 53, 66

Kaggle线上存在感

博客460-463

GitHub平台463-465

出版物460-463

日语Kaggle社区

参考文献链接29

Kaggle推特主页

参考文献链接12

Kagoole

URL 466

KBins离散化器

参考文献链接164

KDD杯第5届

KDnuggets第462期

Keras内置数据增强341

ImageDataGenerator方法341-344

预处理层345

Keras调参器285

模型创建285-294

URL 285

内核53

k折交叉验证161-163

k折变体164-168

知识发现与数据挖掘

参考链接5

L

L1范数113

L2范数113

拉尔科·德米特里155

排行榜

窥探150-152

叶片分类

参考链接101

泄漏

处理187-190

留一法(LOO)159

李正润479

词汇多样性402

LightGBM253

超参数254,255

参考链接 212

参考文献 253

线性模型 250

对数平均值 312

对数损失 105, 119

损失函数 99

安德烈·卢基扬年科 125

Lux AI游戏

参考链接 441

## M

机器学习可解释性参考链接 74 多数表决 309, 310

安德鲁·马拉尼昂 43-47

大师赛 18

马修斯相关系数(MCC) 121,

122

平均绝对误差(MAE) 109, 113

平均精度均值

前K项(MAP@\{K\}) 133-135

幂次均值 312

均方误差（MSE）109

中等

URL 460

Medium平台出版物

参考文献 461

元特征 213

Meta Kaggle数据集 102-105

参考链接 102

元模型 317

分类评估指标

准确率 114-116

F1分数 119

对数损失 119

马修斯相关系数（MCC）121

122

精确率指标 116-118

召回率指标 116-118

ROC曲线下面积(ROC-AUC) 120, 121

多分类评估指标

宏平均 123

宏F1值 123

平均F1值 124

微平均 123

微F1值 123

多类别对数损失

(列平均对数损失) 123

加权法 123

回归评估指标 109

平均绝对误差(MAE) 113

均方误差(MSE) 109-111

均方根误差(RMSE) 111

均方根对数误差(RMSLE) 112

R平方值 110, 111

指标，多标签分类与

推荐问题 133

平均准确率@\{K\} 134

指标，目标检测问题 129-131

戴斯系数 132, 133

交并比(IoU) 131

读心术错觉 92

混合增强技术 229

MLFlow

URL 201

模型

混合，使用的元模型 317

堆叠 323-327

模型验证系统

调优 176-178

罗布·穆拉 306

多臂老虎机(MAB) 435

多类别分类

指标122

多头注意力机制288

多标签分类与

推荐问题

指标133

多重机器学习模型

平均法

交叉验证策略，315页平均法

316

多数投票309-312

预测结果平均312-314

ROC-AUC评估均值

校正316

加权平均314,315

N

纳什均衡432,433

自然语言处理(NLP)389

海王星人工智能平台(neptune.ai)

参考链接201

嵌套交叉验证168-170

网络礼仪规范92

神经网络

表格类竞赛应用231-235

神经遗忘决策

集成算法(NODE)234

未见指标

处理方法105-107

自然语言处理增强库(nlpaug)420-423

没有免费午餐定理5

非线性变换110

笔记本

加速器56

环境配置56

互联网 57

语言 56

职业发展助力 452

进阶要求67,68

运行 58-60

保存至GitHub 60-62

设置 54-56

使用 63, 64

Numerai（Numerai） 10

参考链接 10

## 0

## 目标检测

处理 357-370

指标 129

目标函数 99

OCR错误 421

安德拉达·奥尔泰亚努 74-76

独热编码(one-hot encoding) 211

小野寺和树(Onodera, Kazuki) 247-249

开放数据科学网络参考链接 29 开放域问答(open domain Q&A) 398-411 机遇 35 Optuna TPE方法 295-299 序数任务(ordinal task) 100, 101 作为多分类问题处理 101 作为回归问题处理 102 折外预测(out-of-fold predictions)143,170,323, 410

生成 170, 171

过拟合(overfitting) 157

P

pandas库，Kaggle Learn课程 73

帕鲁尔·潘迪(Pandey, Parul) 19-21

Kaggle性能等级 32

管道(Pipelines)

特征 409

像素精度(pixel accuracy) 130

普拉特缩放(Plat's scaling) 143

Playground竞赛 19

示例 19

诗歌

参考链接 464

作品集

构建，与Kaggle 447-449

数据集，利用455, 456

讨论区，利用452-454

笔记本，利用452-454

正类100

精确率指标117

精确率/召回率权衡117

参考链接118

普雷达，加布里埃尔457-459

预测概率141, 142

调整142-144

预测结果

后处理139-141

预处理层345

私有测试集16

概率评估方法 161

k折交叉验证 161-163

k折变体 164-168

折外预测(OOF)

生成 170, 171

概率校准

参考链接 316

代理函数 261

伪标签 224-226

公开测试集 15

让-弗朗索瓦·普杰 235

Q

二次加权卡帕系数 105

R

苏达莱·拉杰库马尔 144

随机森林 251, 305

随机搜索 242, 245, 246

随机状态

设置（用于可复现性）202, 203

排名 32, 33

贡献者 33

专家 33

宗师 33

大师 33

新手 33

拉奥·罗汉 108, 109

RAPIDS

参考链接 206

召回率指标 117

受试者工作特征曲线（ROC

曲线）120, 121

招聘竞赛 18

示例 18

修正版Adam优化器 289

循环神经网络（RNNs）287

回归任务 100

评估指标 109

正则化 417 强化学习(RL) 100, 425, 426 可复现性 随机状态设置 202, 203 研究竞赛 18 ROC-AUC评估指标 313 均值修正 316 石头剪刀布 431 收益矩阵 432 参考链接 431 使用方法 432-434 均方根误差(RMSE) 109-111 均方根对数误差(RMSLE) 112-114

游程编码(RLE) 371

转换为COCO格式 372, 373

## S

## 采样方法与集成

袋装法 308

粘贴法 308

随机补丁 308

随机子空间 308

采样策略 159

2020年圣诞竞赛 435-439

参考链接 435

奖励衰减 435

Scikit-multilearn库

参考链接 164

Scikit-optimize（Scikit优化库）

使用262-267

评分函数 99

语义分割 130, 371-384

情感分析 389-396

重大变革 151

共享词 403

ShuffleSplit（随机拆分）

参考链接 171

Sigmoid方法 143

Signate（数据科学平台）

参考链接 10

简单算术平均 312

简单格式 21

模拟拼写错误 421

尺寸

数据缩减 208, 209

斯皮尔曼相关系数(Spearman correlation) 399

分割策略

使用 159

稳定性选择(stability selection) 221

堆叠法(stacking) 305, 323-327

变体 327-329

STAR方法 483, 484

随机加权平均(Stochastic Weighted Averaging, SWA) 289

分层\( k \)折

参考链接 164

Streamlit框架

URL 465

子采样(sub-sampling) 171

误差平方和(sum of squared errors, SSE) 109

总平方和(sum of squares total, SST) 110

支持向量机

分类支持向量机(SVC) 243

支持向量机

支持向量机(SVMs) 243, 250, 251

替代函数 261, 295

交换噪声 228

交换 417

对称平均绝对百分比误差

(sMAPE)

参考链接 114

同义词替换 415

合成数据仓库(Synthetic Data Vault)

参考链接 197

系统化实验 153

T

表格网络(Tabnet) 234

表格数据竞赛

神经网络 231-235

表格游乐场系列 196-201

目标编码(target encoding) 216

任务类型

分类(classification) 100

序数(ordinal) 101

回归(regression) 100

团队协作(teaming) 28, 29

Telstra网络中断事件

参考链接(reference link) 189

张量处理单元(tensor processing units/TPU) 338

测试集(test set) 168

预测(predicting) 170

文本增强策略(text augmentation strategies) 414

基础技术(basic techniques) 415-420

nlpaug工具 420-423

TF-IDF表示法 406

塔库尔，阿布舍克 397

蒂特里茨，吉尔伯托 449-452

分词处理 392

TPE方法

在Optuna中 295-299

训练-测试集划分 160

图像变换 336

演示 336-341

TransformedTargetRegressor函数

参考链接 111

树状结构帕森

估计器(TPEs) 261, 262

t-SNE降维 205-207

通古兹，博扬 223

两阶段竞赛 21

U

UMAP降维 205-207

单变量分析 204

通用句子编码器（Universal Sentence Encoder）

参考链接 404

可用性指数 41

V

验证 153, 154

验证损失 157

验证集 168

预测 170

版本控制系统 465

## W

加权平均值 312-314

加权均方根比例误差（Weighted Root Mean Squared Scaled Error）

参考链接 114

权重与偏置（Weights and Biases）

参考链接 201 X

XGBoost算法 255, 256

参数 256, 257

参考文献链接 212, 255

谢逸凡 90, 91

Y

Yolov5算法 357

Z

张一润 471

Zindi平台 10

参考文献链接 10