# 2024 CCL24-Eval      手语数字人翻译质量评测

## 主题 ： 小语种自然语言处理

### 评测组织者
* 姚登峰教授（tjtdengfeng@buu.edu.cn），北京联合大学/清华大学  
* 仰国维副研究员，河南财经政法大学/中国聋人协会手语研究与推广委员会  
* 金澎教授，乐山师范学院特殊教育语言智能四川省哲学社会科学重点实验室
* 陈毅东副教授，厦门大学
* 徐聪主任，中国聋人协会手语研究与推广委员会/华夏出版社国家通用手语数字推广中心
* 王海旭研究员，青海广播电视台/中国盲文手语研究应用中心
* 陈斌博士，株洲手之声信息科技有限公司
* 吴力权副秘书长，深圳市信息无障碍研究会
* 沈刚副主任，中国聋人协会手语研究与推广委员会
* 陈华铭副主任，中国聋人协会手语研究与推广委员会
* 刘春达，北京手语研究会
* 丁艳丽，北京联合大学国家语言文字推广基地
* 胡可，北京联合大学
* 陈澜，深圳市联谛信息无障碍有限责任公司
* 袁甜甜，天津理工大学

### 联系人及联系方式
* 赵源（1398396428@qq.com），北京联合大学硕士生
* 张睿诠，厦门大学硕士生
* 刘振宇，北京联合大学硕士生    

  

## 1.任务内容  
&emsp;&emsp;CCL（China National Conference on Computational Linguistics）为中国计算语言学大会，会议组织单位为中国中文信息学会。CCL是全国最权威、最具影响力、规模最大的NLP会议之一，它聚焦于中国境内各类语言的智能计算和信息处理，为研讨和传播计算语言学最新学术和技术成果提供了广泛的高层次交流平台。

&emsp;&emsp;随着科技的进步，手语数字人（Sign Language Avatars）已经成为促进聋人群体与社会沟通的重要工具。手语数字人通过模拟手语动作，为聋人提供实时的翻译服务，有助于打破语言障碍，提升聋人群体的社会参与度。为了确保手语数字人能够提供准确、自然且易于理解的手语翻译，对其翻译质量进行评测至关重要。本次评测旨在评测手语数字人将汉语翻译成中国手语方面的自然性和准确性，确保手语数字人能够符合手语语法规则，并且能够被聋人群体所理解和接受。

&emsp;&emsp;由于手语为小语种，语料库规模有限，因此本次评测将不设自动评测环节，全部采取人工评测的方式进行。由中国聋人协会手语研究与推广委员会认证的精通中国手语的聋人和专业手语翻译人员组成的评测者对手语数字人的翻译结果进行人工评测。

&emsp;&emsp;鉴于各参赛队伍均已拥有自主产权的手语语料库（欢迎各参赛队伍提供语料，本评测团队和中国聋人协会手语研究与推广委员会审核后将一起公布），此次评测提供的语料库仅作为参考，以确保评测的全面性和公正性。

&emsp;&emsp;本评测团队提供的首批语料库分为三个部分，总计包含1074个句子。

| 语料库    | 文本 | 视频 | 句子数量 | 版权所有者                 | 联系人      | 备注                                                     |
| --------- | ---- | ---- | -------- | -------------------------- | ----------- | -------------------------------------------------------- |
| XMU_CSL   | ✔️    | ✔️    | 500      | 厦门大学                   | 陈毅东 教授 | 视频：按照视频帧文件夹的形式，可以使用Python来批处理合成 |
| BUU_CSL   | ✔️    | ✔️    | 500      | 北京联合大学               | 姚登峰 教授 |                                                          |
| ZZSZY_CSL | ✔️    | ✔️    | 74       | 株洲手之声信息科技有限公司 | 陈斌 博士   |                                                          |

## 2.评测数据  
#### 数据提供：
手语语料库以及对应的真人手语演示集合：  
&emsp;&emsp;在本次评测语料库中，我们会选择特定场景的语料，并提供相应的书面语文本及其对应的手语转写文本作为参考示例。这些参考示例包括词性标注和手势级别的标注。此外，评测还将提供参考示例的手语视频演示，特别注意其中的表情变化。

&emsp;&emsp;（注：标记为❶❷的是词目相同但词义不同的常用词；标记为①②的是词目和词义相同，但手语动作有差异的常用词。其他手语内容的参考资料包括《国家通用手语常用词表》和《国家通用手语词典》APP等相关资料。）

* &emsp;例1：  
&emsp;书面语：女儿可能生病了，快带她去医院。  
&emsp;手语转写文本：  
&emsp;&emsp;词级标注：  
&emsp;&emsp;&emsp;女儿②/病/可能②，带❶/医院/速度  
&emsp;&emsp;手势级标注：  
&emsp;&emsp;&emsp;女-矮/病/可能②【疑问】，带❶/医生-家/速度

![Image text](https://github.com/ann-yuan/lzygjzs/blob/main/1.png)

&emsp;&emsp;上面图例是心理活动波长，类似于“渐变”的表情变化过程。

&emsp;&emsp;解读：y上半轴表示正面情绪作用，y下半轴表示负面情绪作用；x右半轴表示正常表情，k斜率表示手势动作快慢。


![Image text](https://github.com/ann-yuan/lzygjzs/blob/main/table1.png)

&emsp;手语演示：  
&emsp;&emsp;![image](https://github.com/ann-yuan/lzygjzs/blob/main/video1.gif)

* &emsp;例2：  
&emsp;书面语：为了赢得比赛，儿子一直在专心训练。  
&emsp;手语转写文本：  
&emsp;&emsp;词级标注：  
&emsp;&emsp;&emsp;为/比赛/赢②，儿子②/专心/训练/一直  
&emsp;&emsp;手势级标注：  
&emsp;&emsp;&emsp;为/比较/胜利②，男-矮/认真【眼睛同时向下看】-心/练习/一直

![Image text](https://github.com/ann-yuan/lzygjzs/blob/main/2.png)

&emsp;&emsp;上面图例是心理活动波长，类似于“渐变”的表情变化过程。

&emsp;&emsp;解读：y上半轴表示正面情绪作用，y下半轴表示负面情绪作用；x右半轴表示正常表情，k斜率表示手势动作快慢。


![Image text](https://github.com/ann-yuan/lzygjzs/blob/main/table2.png)

&emsp;手语演示：  
&emsp;&emsp;![image](https://github.com/ann-yuan/lzygjzs/blob/main/video2.gif)


## 3.评价标准   
&emsp;&emsp;评测将以手语语法的准确性、表达的自然性和可读性以及是否满足聋人理解为主要标准，综合考虑手势清晰度、流畅性、与汉语原文的语义一致性等。具体包括：

&emsp;&emsp; 1、手语语法准确性：

&emsp;&emsp; 词序和结构：检查翻译是否遵循中国手语的词序规则，例如，汉语的主谓宾结构在手语中可能需要调整为更符合手语习惯的顺序。

&emsp;&emsp; 手势形态：评测手势是否正确，是否使用了恰当的手指位置、手掌方向和手部运动。

&emsp;&emsp; 语法标记：手语中有许多语法标记，如时态、否定、疑问等，需要确保这些标记在翻译中得到正确表达。


&emsp;&emsp; 2、自然性：

&emsp;&emsp; 流畅性：翻译过程中的手势是否连贯，是否模仿了自然手语的流畅性，避免生硬的断续。

&emsp;&emsp; 表达习惯：评测翻译是否符合聋人群体的日常表达习惯，包括常用的手语短语和惯用表达。

&emsp;&emsp; 非言语元素：考虑面部表情、身体姿态和空间布局等非言语元素是否自然地融入翻译中。


&emsp;&emsp; 3、可读性：

&emsp;&emsp; 清晰度：手势是否清晰可见，是否容易被理解，避免模糊不清的动作。

&emsp;&emsp; 一致性：确保同一概念或词汇在不同句子中的手势表达保持一致，便于理解和记忆。

&emsp;&emsp; 适应性：评测翻译是否考虑到不同语境下可能需要的调整，以提高可读性。


&emsp;&emsp; 4、文化适应性：

&emsp;&emsp; 文化差异：翻译是否考虑到文化差异，避免直译可能带来的文化误解或不恰当的表达。

&emsp;&emsp; 社会语境：评测翻译是否考虑了社会语境，如礼貌用语、行业术语等，以确保在特定社会环境中的适宜性。

&emsp;&emsp; 情感色彩：检查翻译是否能够准确传达原文的情感色彩，如讽刺、幽默等。

&emsp;&emsp; 本次评测主要采用人工评测方式。在评估参赛团队的手语数字人时，评测人员会选择特定场景，输入一段文字，生成对应的视频，即数字人的翻译已完成。人工评测用于综合评估手语数字人在各指标方面的表现，每项指标的总得分为去掉一个最高分和一个最低分后的所有评分的算术平均值。假设有一组评分![](https://latex.codecogs.com/svg.image?&space;X=x_{1},x_{2},...,x_{n})，具体的计算公式为：
![](https://latex.codecogs.com/svg.image?&space;R=\frac{\sum_{x_{i}\subset&space;X'}x_{i}}{n-2})

&emsp;&emsp; 式中：  
&emsp;&emsp; \$n\$ ——&emsp;评价人员数量；  
&emsp;&emsp; \$X'\$ ——&emsp;移除最高分 \$max(X)\$和最低分 \$min(X)\$后的评分集合

&emsp;&emsp; 评测人员包括精通中国手语的聋人和专业的手语翻译人员，计划招募20人。这些评测人员经过专业培训后，负责进行手语评测，观看测试结果，并按照设定的得分标准进行整体评估。

&emsp;&emsp; 为了测试手语数字人，参赛队伍需提供系统接口。评测负责人将在系统接口上输入一些句子，并录制手语数字人的翻译过程，这些录制将以随机顺序发送给评测人员。评测方法如下：

&emsp;&emsp; 场景准备：本次评测将选定5个场景，并为每个场景设计3个句子，总计15句，用于全面评估参赛手语数字人的翻译与表达性能。

&emsp;&emsp; 手语生成：参赛队伍需提供的数字人接口将用于生成15句指定内容的手语视频，以便进行性能评测。

&emsp;&emsp; 性能评测：比赛评价标准包括准确性、自然性、可读性和文化适应性四个关键指标。基于这些指标，本次评测将设定12道选择题，全面覆盖所有测试句子。评测人员将根据手语视频的实际表现来选择答案，每题得分直接关联至相应的评价指标，每个指标的最高得分为5分。

&emsp;&emsp; 数据收集和分析：收集评测人员的评分和反馈，得到每个数字人各项指标的评测结果，综合得出每个参赛作品的最终得分。

&emsp;&emsp; 注：根据参赛规模和实际情况，本次评测保留调整场景句子数量、选择题数量的权利，以确保评测的适应性和公平性。


### 3.1 &emsp;手语语法准确性 
&emsp;&emsp; 本次评测指标是评估手语数字人在手语语法准确性方面的表现。评测的内容包括手语数字人是否遵循中国手语的词序规则，手势的准确性，以及语法标记在翻译中是否得到正确表达。

&emsp;&emsp;手语语法准确性得分表如下表所示：  
| 分数 | 评分标准 |
| --- | --- |
| 1 | 基本不遵循手语语序习惯，都不符合手语五要素（手的形状、手的动作、手的位置、手掌的方向和面部表情）标准，缺乏表现时态、否定、疑问等语法标记的能力。 |
| 2 | 通常不遵循手语语序习惯，很少符合手语五要素标准，几乎不表现时态、否定、疑问等语法标记。 |
| 3 | 在一定程度上遵循手语语序习惯，部分符合手语五要素标准，能够在一定程度上表现时态、否定、疑问等语法标记。 |
| 4 | 大多数情况下遵循手语语序习惯，大部分时间符合手语五要素标准，能较好地表现时态、否定、疑问等语法标记。 |  
| 5 | 完全遵循手语语序习惯，严格符合手语五要素标准，完美地表现时态、否定、疑问等语法标记。 |  

### 3.2 &emsp;自然性 
&emsp;&emsp; 本次评测指标是评估手语数字人在自然性方面的表现。这包括评估手势的连贯性、翻译是否符合聋人群体的日常表达习惯，以及面部表情、身体姿态和空间布局等非言语元素是否自然地融入翻译中。

&emsp;&emsp; 自然性得分表如下表所示：  
| 分数 | 评分标准 |
| --- | --- |
| 1 | 手势表达的时候，缺乏任何连贯性和流畅性，呈现出生硬、不协调的状态，与聋人日常表达的习惯完全不符。非言语元素如表情、体态、空间位置和运动轨迹等几乎未被考虑，导致手语交流难以达到有效沟通。 |
| 2 | 手势缺乏连贯性和流畅性，显得生硬和不自然，与聋人的日常表达习惯严重不符。表情、体态、空间位置和运动轨迹等非言语元素几乎未被考虑或表现得极不自然。 |
| 3 | 部分手势表现出一定的连贯性和流畅性，但仍有生硬之处。时而符合聋人的日常表达习惯。表情、体态、空间位置和运动轨迹等非言语元素被部分考虑，但整合度和自然性有待提升。 |
| 4 | 大部分手势连贯、流畅，不显生硬，较好地符合聋人的日常表达习惯。表情、体态、空间位置和运动轨迹等非言语元素较好地融入。 |  
| 5 | 手势完全连贯且流畅，无任何生硬之感，完全符合聋人的日常表达习惯。能够全程体现表情、体态、空间位置和运动轨迹等非言语元素。 |  

### 3.3 &emsp; 可读性 
&emsp;&emsp; 本次评测指标是评估手语数字人在清晰度、一致性和适应性方面的表现。

&emsp;&emsp; 可读性得分表如下表所示：  
| 分数 | 评分标准 |
| --- | --- |
| 1 | 手势表达极不清晰，动作混乱，几乎无法准确理解。同一概念或词汇的手势在不同句子中表达极为不一致，造成混淆和困扰。缺乏对手势的基本规范和一致性，使得整体传达的信息异常混乱，对于聋人的交流体验形成巨大障碍。 |
| 2 | 手势表达不清晰，动作模糊，难以理解。同一概念或词汇的手势在不同句子中表达不一致，导致理解和记忆困难。在不同语境下的适应性完全未被考虑，严重影响了可读性。 |
| 3 | 手势部分清晰，虽有模糊之处，但大体上可理解。对同一概念或词汇的手势在不同句子中大多数情况下保持一致，偶尔存在一致性问题。在不同语境下的适应性得到了部分考虑，但在某些情况下仍需改进。 |
| 4 | 手势大多数情况下非常清晰，易于理解，仅极少数动作略有不清晰。对同一概念或词汇的手势在不同句子中几乎始终保持一致，有助于理解和记忆。在不同语境下的适应性被较好地考虑，有效提高了可读性。 |  
| 5 | 手势完全清晰，毫无模糊之处，易于理解。对同一概念或词汇的手势在所有句子中始终保持完全一致，极大促进理解和记忆。在不同语境下的适应性被完全考虑，极大提高了可读性。 | 

### 3.4 &emsp; 文化适应性 
&emsp;&emsp; 本次评测指标是评估手语数字人在文化适应性方面的表现。评测内容包括翻译时是否考虑了文化差异、社会语境的适应性，以及是否能够准确传达原文的情感色彩。

&emsp;&emsp; 文化适应性得分表如下表所示：  
| 分数 | 评分标准 |
| --- | --- |
| 1 | 目标语言未考虑文化差异，未反映南北方及其他地区手语文化的不同，导致交流难以理解。缺失社会环境中的礼貌用语和行业术语，情感色彩传达不准确，如讽刺、幽默等未能恰当表达。 |
| 2 | 目标语言未考虑文化差异，南北方及其他地区手语文化的差异未得到适当反映。社会环境中的礼貌用语和行业术语缺失，情感色彩如讽刺、幽默等未能准确传达。 |
| 3 | 目标语言在一定程度上考虑了文化差异，南北方及其他地区的手语文化部分得到反映。在一定程度上使用了社会环境中的礼貌用语和行业术语，对情感色彩的传达如讽刺、幽默等部分准确。 |
| 4 | 目标语言在大多数情况下考虑了文化差异，南北方及其他地区的手语文化大多数情况下得到适当反映。普遍使用了社会环境中的礼貌用语和行业术语，对情感色彩的传达如讽刺、幽默等大多数情况下准确。 |  
| 5 | 目标语言完全考虑了文化差异，南北方及其他地区的手语文化差异都得到了完全的反映和尊重。充分使用了社会环境中的礼貌用语和行业术语，对所有类型情感色彩的传达，如讽刺、幽默等都极为准确。 | 

### 3.5&emsp;综合评价方法  
&emsp;&emsp;手语数字人翻译质量的人工评测包括四个主要指标：手语语法准确性、自然性、可读性以及文化适应性。综合得分是根据每个单项指标的得分与其相应的权重系数计算得出的加权和。评测重点关注手语数字人在准确表达手语的能力，强调自然性和可读性，同时兼顾对文化适应性的考量。在整体评测架构中，单项指标的权重分配如下。
| 指标类型 | 指标名称 | 权重系数 | 占比 |
| --- | --- | --- | --- |
| 人工评测翻译质量 | 手语语法准确性 | 0.30 | 30% |
| 人工评测翻译质量 | 自然性 | 0.25 | 25% |
| 人工评测翻译质量 | 可读性 | 0.25 | 25% |
| 人工评测翻译质量 | 文化适应性 | 0.20 | 20% |

&emsp;&emsp;（以上内容可能还会有调整，请关注网站最新消息）

## 4.评测赛程 
* ~开放报名：2024年1月1日~  
* ~公布手语语料库等以及评测方法：2024年3月15日~  
* ~报名截止： 2024年3月15日~
* ~参赛队提交系统接口：2024年5月6日（最终）~
* 正在进行评测ing~
* 组织者返回评测结果：2024年~5月25日~ -->  5月15日
* 参赛队提交评测任务技术报告用于审稿：2024年~5月31日~ -->  5月21日
* 参赛队提交技术报告最终版： 5月25日-6月15日
* 评测论文录用通知：2024年~6月25日~ -->  6月15日
* CCL 2024评测研讨会：2024年7月25-28日
* ***以上时间点以CCL24-Eval官方提供的时间点为主。如实际情况与以上时间点有出入，请联系本次评测任务的负责人（微信号：annwois）***

### 任务大致流程：
报名完成的参赛队伍请邮箱联系本次评测联系人（1398396428@qq.com），以获取本次评测提供的手语语料库（需提前签署语料库保密协议及版权声明书），参赛队伍可以使用自带的手语语料库，也可以使用本次评测提供的手语语料库，最终提交评测任务技术报告和系统接口及其使用说明书。本次评测将通过系统接口来测评参赛队伍的手语数字人，并录制最终生成的手语视频，评测联系人提交给评测者来完成本次评测。
(注：本次评测所提供的手语语料库只用于训练，不能同时作为测试)

## 5.奖项设置  
本届评测将设置一、二、三等奖，由中国中文信息学会为获奖队伍颁发荣誉证书。

## 6.撰写技术报告
报告可由中文或英文撰写。  
报告统一使用CCL 2024的论文模板。  
报告正文不得超过4页，参考文献页数不限。  
报告应至少包含以下四个部分：模型介绍、评测结果、结果分析与讨论和参考文献。  

## 7.报名提交方式及申请本次评测语料使用权
点击报名链接填写报名表 https://f.kdocs.cn/g/aYC93cfz/    进行报名，我们会发送邮件确认您已经参赛，如需要本次评测提供的语料库，请参赛队伍需自行向评测联系人申请本次评测语料使用权，并签署保密协议。
 1)	每支参赛队伍需指派一名联系负责人。
 2)	参赛队伍联系负责人需填写本次评测语料的使用权协议，并签署保密协议，扫描后通过E-mail发送给评测联系人（1398396428@qq.com）。
 3)	申请通过后，评测联系人将返回手语语料库给参赛队伍联系负责人，以供参赛队伍使用。该语料数据只可用于本次评测任务，不可有其他任何用途，请尊重手语标注者的成果。
 4)	本次评测语料库的知识产权按其版权分别归属北京联合大学、乐山师范学院、厦门大学、青海广播电视台、株洲手之声信息科技有限公司所有。
