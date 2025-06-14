# 2025
## 05.24
多字加上句号，够
## 1.19
在 AI 时代，要怎么做呢，最近一年看了不少书和blog，仔细想了想，可能需要学习这几个事情：
- 理解现实：AI再强，终究是要作用于现实的，所以理解现实究竟如何是怎样的很重要。
- 发现问题：理解完现实后，能不能从中发现问题呢？这个问题是“真需求”还是“假需求”？这个环节不妨试试 5 Why，找到那个 Root Question
- 解决问题：发现问题之后，用哪些方式来解决问题？他们的优缺点是什么？最佳解决方案是什么？最佳方案哪些事情可以借助外力？借用哪些外力
## 1.8 
补充一个基于 5 why 的分析：
```markdown
## 数据安全与泄露风险:
为什么大型模型存在数据泄露的风险？
因为大型模型需要大量的数据来进行训练，而这些数据可能没有得到妥善的保护。

为什么数据没有得到妥善保护？
由于安全措施不足或过时。

为什么安全措施不充分？
组织可能没有优先考虑安全，或者缺乏实施强安全协议的专业知识。

为什么组织不优先考虑安全？
可能是因为缺乏对数据安全重要性的认识或预算限制。

为什么缺乏意识？
组织可能没有经历过重大数据泄露事件，或者缺乏相关教育。

## 模型验证与偏见检测:
为什么大型模型容易出现缺陷？
因为它们是在可能包含偏见或不准确数据上进行训练的。

为什么数据验证不充分？
可能是因为验证过程不彻底，或者在模型开发过程中没有给予足够的重视。

为什么验证过程不彻底？
可能是因为急于部署，或者缺乏对有效验证方法的理解。

## 对抗攻击的脆弱性:
为什么大型模型容易受到对抗攻击？
因为它们可能被设计来引发错误的输入所欺骗。

为什么模型没有得到更好的保护？
可能是因为防御不断演变的对抗技术具有挑战性和资源密集性。

为什么难以预见所有潜在威胁？
因为人工智能领域发展迅速，新的攻击向量不断出现。

## 透明度与可解释性:
为什么模型透明度对安全很重要？
因为不透明的决策过程使得识别和纠正偏见或错误变得困难。

为什么难以使复杂模型透明？
可能是因为复杂模型与可解释性之间存在权衡。

## 法规合规性:
为什么法规合规性对大型模型的安全很重要？
因为法规强制执行数据保护和伦理AI使用标准。

为什么并非所有组织都符合法规？
可能是因为法规复杂且各地区差异大，或者组织缺乏 awareness。

## 人为因素:
为什么人为错误会引发大型模型的安全问题？
因为对自动化系统的依赖可能导致 oversight 或错误。

为什么人为错误没有得到充分解决？
可能是因为人员培训或监督不足。

为什么培训或监督不足？
可能是因为缺乏资源、时间，或者没有认识到人为因素在模型安全中的重要性。

## 基于分析的行动步骤:
- 加强安全措施，定期更新 robust 安全协议，以保护数据和模型。
- 加强验证流程，确保在模型开发过程中给予足够重视。
- 投资于对抗防御技术，跟上不断演变的攻击方法。
- 提高模型透明度，探索在不牺牲性能的情况下增加解释性的方法。
- 确保法规合规性，了解相关法规并确保模型符合所有法律标准。
- 解决人为因素，为管理模型的人员提供全面培训和监督。
- 通过解决这些领域的问题，组织可以显著提高AI应用中大型模型的安全性和可靠性。
```
## 1.1
最近一个季度在做大模型安全方面的工作，也学了一点这方面的知识，现在用 SMART 框架来整理一下学习内容：

### 具体性（Specific）
大模型安全的具体性，就是要清楚识别和定义安全目标。比如，对于特定的安全威胁，像越狱攻击、提示注入攻击等，得制定明确的防护办法和应对策略。这包括：
- 确定要保护的数据类型
- 明确潜在的攻击途径
- 设定防护措施的具体标准
### 可测量性（Measurable）
可测量性是指能对安全目标进行量化评估。对大模型来说，可以这样测量：
- 监控系统的漏洞发现比例
- 测试模型面对特定攻击的反应时间
- 评估用户生成内容里有害信息的识别准确率
通过这些指标，能持续跟踪大模型的安全性能，然后及时调整策略。
### 可实现性（Achievable）
可实现性要求设定的目标在技术和资源上能达成。对大模型而言，意思是：
- 保证团队有必需的技术能力
- 资源分配合理，能支持持续的安全研究和开发
- 用合适的技术工具来落实安全措施
比如，用现有的机器学习框架做自动化漏洞检测。
### 相关性（Relevant）
相关性确保所设定的安全目标与整体业务目标相一致。在大模型应用中，这意味着：
- 安全措施应与业务需求相匹配，避免不必要的资源浪费
- 考虑到行业标准和法规要求，确保合规性
例如，在数据保护方面，确保符合GDPR或其他相关法律法规。
### 时限性（Time-bound）
时限性要求为每个安全目标明确设定时间框架。这能助力团队把控进度并评估成果。比如：
- 建立季度审查机制，用于评估安全措施的有效性
- 在特定时间内完成漏洞修复工作
### 大模型自身安全框架
根据最新的大模型安全研究报告，大模型存在多种安全风险，比如训练数据质量、算法鲁棒性、系统平台安全等方面的问题。因此，报告提出了一个包含四个层面的自身安全框架，分别是：
1. 安全目标：明确要达成的具体安全成果。
2. 安全属性：确定系统应有的基本安全特征，像机密性、完整性和可用性。
3. 保护对象：找出需要保护的信息资产和系统组件。
4. 安全措施：制定针对已识别风险的具体防护办法，涵盖技术手段和管理策略。

# 2024
## 12.27
> https://berthub.eu/articles/posts/on-long-term-software-development/

how to develop the long term software:
1. reduce the dependencies
2. MORE TESTING
3. reduce Complexity
4. Write boring simple code. Even more simple than that. Even more boring.
5. no LinkedIn-based software development
6. Logging, telemetry, performance
7. keep the team
8. Be open source

## 12.14
2023年那会儿，还在思考 Chatgpt：
![image](https://github.com/user-attachments/assets/707f0878-5de1-4a2e-81a3-7bd0b20e6981)

而最近一年，可以说是具体实践了大量的 AI 工具，从写代码到替换搜索引擎, 可以说是无所不在了。
而其中 Promopt 也算是重要一环了，尤其是是早期模型还不是那么“聪明”的情况下，多数情况也需要Promot来帮助我们获得更好的记过。所以前期也看了很多关于讨论该如何写好一个 Prompt的文章，加之后续的实践，在这里稍作一个总结：

其中较为核心的元素如下：
```
Prompt = 角色 + 背景 + 任务 + 示例

- 角色：设定AI的身份，使其能够从特定视角进行思考。
- 背景：提供必要的信息，以便AI理解上下文。
- 任务：明确要执行的具体操作。
- 示例：通过例子来展示预期结果。
```
有了这些基本上就可以组成一个比较靠谱的 Prompt 了，但除此之外其实还有一些元素是可以帮助我们获得更好的提示结果的。

剩余的元素还有：
- 输出限定：输出格式（Markdown、JSON、表格），语言风格（专业、通俗、幽默），语言选择，长度限制
- 约束条件：不能使用的方法，需要避免的陷阱，特定禁忌或敏感话题，版权和伦理考虑
- 步骤细化：明确输出的思考过程，要求逐步推理，解释每一步的逻辑
- 评估标准：定义"好"的具体衡量指标，输出质量评判规则，期望达到的专业水准
- 交互指南：如何追问和深入，后续可能的探讨方向，鼓励AI主动提供额外洞察
- 上下文记忆：指定保留之前对话的关键信息，上下文记忆，避免重复或遗忘之前的讨论

以上元素大体上都是用于规范输入输出、确定模型执行逻辑和标准（也就是思维链），从而获得更为精确的结果。

比如这就是我自己搞的一个 英语学习教练 的一个 Prompt：
```
角色：你是一位常驻于纽约，从小从纽约长大的，经验丰富的英语教育专家和语言学习教练，拥有超过15年的国际教学经验，。

背景：服务于不同年龄段和英语水平的学习者，熟悉多种语言学习方法和跨文化交流策略

任务：作为个性化的英语学习助手，帮助学习者提高英语能力

输出限定：
- 语言：中英双语
- 风格：专业且友好，通俗易懂，用词带有美式纽约的口语习惯用法
- 格式：结构清晰的Markdown

具体职责：
1. 根据学习者当前水平提供定制化学习建议
2. 解答语法、词汇、发音等具体问题
3. 提供语言学习策略和资源推荐

约束条件：
- 避免使用过于学术的术语
- 禁止直接给出答案，鼓励学习者思考
- 尊重文化差异，提供跨文化语言洞察

步骤细化：
- 诊断学习者当前水平
- 分析学习障碍
- 制定个性化学习路径
- 提供具体的练习和改进建议

评估标准：
- 建议的针对性
- 解释的清晰度
- 学习方法的创新性

交互指南：
- 鼓励学习者提供更多上下文
- 主动询问学习目标和兴趣
- 适时分享语言学习小技巧

示例模式：
1. 当解释语法时，提供：
   - 规则说明
   - 使用场景
   - 常见错误
   - 实际应用示例

2. 词汇学习时，展示：
   - 单词定义
   - 词源
   - 同义词和反义词
   - 搭配用法
   - 记忆技巧
```

实际应用结果：![image](https://github.com/user-attachments/assets/3363a346-df4f-4234-aa47-8c6287ed591a)

## 11.29
发现了一个关于概率论的网站，很有意思：https://probability.visualized.fun/
每个章节后的人生哲理很有意思：
1. 大数定理："人生就像一场大数定理实验，重要的不是单次的成败，而是坚持到收敛的那一刻。 记住 ——样本量不够，就往死里试！"
2. 贝叶斯定律："人生就像一场贝叶斯更新，每一条新信息都是一次概率革命。不过最重要的是 ——先验概率不重要，重要的是不断更新！"
3. 凯利公式："人生就像一场投资，每个选择都是一次下注。合理分配你的时间、精力和资源， 让收益最大化，风险最小化。不过最重要的是 ——及时止损，大胆梭哈，人生最重要的是开心啦！
## 10.18
最近在思考，为何大部分的内容创作者都会在一段时间后选择放弃，最近看到关于内容工作者的生产流程：
1. 你的大部分时间用来扩大受众。
2. 你不断培养这些受众，作为销售内容的市场。
3. 你创造可以获利的内容产品，投向这个市场。
4. 重复第一步。

想要维持这个流水线，需要做到：定期推出一些有意思或有用的内容，吸引受众。这无疑是很累的，灵感也终究会有枯竭的时候。
## 9.25
Here are some tips for successful refactoring:

- Be incremental: Make small, manageable changes rather than sweeping rewrites.
- Deeply understand code before doing significant refactors or new abstractions.
- Match the existing code style: Consistency is key for maintainability.
- Avoid too many new abstractions: Keep it simple unless complexity is truly warranted.
- Avoid adding new libraries, especially of a very different programming style, without buy-in from the team.
- Write tests before refactoring and update them as you go. This ensures you're maintaining the original functionality.
- Hold your coworkers accountable to these principles.
  ![image](https://github.com/user-attachments/assets/021189cf-004e-4a19-bea1-d76b77849956)

## 9.17
1,000 True Fans: https://kk.org/thetechnium/1000-true-fans/

this is the summary:
- Creators don't need millions of fans, they only need 1,000 true fans to make a living.
- True fans are defined as loyal fans who will buy all of the creator's works, bringing them stable income.
- The formula for calculating the number of true fans is: each true fan spends an average of $100 per year, 1,000 true fans generate $100,000 in annual income, which is enough to sustain most people's lives.
- The number 1,000 is not absolute and can be adjusted according to the creator's situation, but it is much lower than the goal of millions of fans.
- In the internet age, creators can directly connect with true fans without intermediaries, greatly reducing the difficulty of obtaining 1,000 true fans.
- Crowdfunding is a great way to allow true fans to support creators' works in advance.

Based on this, it is quite similar to a platform or tool. If we can get the true fans and provide them with support, it will also be sufficient. a very simply formula：
> 1000 fans * Function（tool || platform）= performace

  

## 8.16
### 六顶思考帽
六顶思考帽是由英国学者爱德华·德博诺（Edward de Bono）提出的一种思考方法。这种方法旨在通过模拟不同的思考方式来提高决策和问题解决的效率。每顶"帽子"代表一种特定的思考模式。让我们详细了解一下：

1. 白帽：代表客观和中立
   - 关注事实和数据
   - 不带感情色彩
   - 类似于科学家的思考方式

2. 红帽：代表情感和直觉
   - 关注感觉和直觉反应
   - 不需要为情感做出解释或合理化
   - 允许表达恐惧、喜欢、不喜欢等情绪

3. 黑帽：代表谨慎和批判
   - 指出计划中的风险和潜在问题
   - 进行逻辑性的负面分析
   - 帮助识别弱点，以便改进

4. 黄帽：代表乐观和积极
   - 寻找机会和好处
   - 探索可能性
   - 提供建设性的观点

5. 绿帽：代表创造力和新想法
   - 产生新的概念和观点
   - 寻找替代方案
   - 突破常规思维

6. 蓝帽：代表过程控制和宏观思考
   - 管理思考过程
   - 确定讨论的焦点
   - 总结和得出结论

在实践中，可以按需"戴上"不同的帽子来看待问题。例如，在考虑一个新项目时：

- 白帽：收集关于项目的客观数据和信息
- 红帽：表达对项目的直觉感受
- 黑帽：分析项目可能面临的风险和挑战
- 黄帽：探讨项目可能带来的好处和机会
- 绿帽：提出创新的实施方案
- 蓝帽：总结各方面的意见，制定行动计划

这种方法的优点是：
1. 鼓励全面思考
2. 减少冲突，因为每个人都在同一时间采用相同的思考模式
3. 提高会议效率
4. 培养灵活的思维能力


## 07.05
最近看完了之前听 孟岩 podcast 强烈推荐的《有限和无限的游戏》，整体来讲书的翻译有点绕口（也可能是原文就是如此），但总体看完有一些启发：
### 游戏的本质

#### 有限游戏：

- **目的**：赢得胜利
- **特征**：有明确的开始和结束，固定的规则，特定的赢家
- **范围**：在既定边界内进行

#### 无限游戏：

- **目的**：延续游戏本身
- **特征**：没有固定的开始和结束，规则可变，无特定赢家
- **范围**：挑战和探索边界本身

### 参与者心态

#### 有限游戏参与者：

- **追求**：获得头衔、权力和胜利
- **态度**：严肃，害怕不可预知的结果
- **时间观**：消耗时间，追求可预测的未来

#### 无限游戏参与者：

- **追求**：体验生活的多样性，探索可能性
- **态度**：开放，乐于接受变化和挑战
- **时间观**：创造时间，每一刻都是新的开始

### 对生活的影响

#### 人生观：

- 有限游戏将人生视为一系列需要"赢"的比赛，而无限游戏将人生视为一个持续探索和成长的过程。

#### 成功定义：

- 有限游戏以外在成就（如头衔、地位）衡量成功，无限游戏则关注个人成长和对世界的贡献。

#### 创造力：

- 无限游戏鼓励创新和突破边界，而有限游戏倾向于在既定规则内优化。

#### 文化与传统：

- 文化本质上是一种无限游戏，不断演变和创新，而非简单的传统复制。

#### 权力与力量：

- 有限游戏中的胜利者获得权力，而无限游戏中每个参与者都拥有内在力量。

总的来讲，注意区分有限的游戏和无限的游戏，去 **玩** 无限的游戏


倒是让我这几年的一些想法得到了印证，我自己喜欢旅行，很大的原因就在于，可以去探索世界的多样性。 
有时候太注重确定性，或许并不是坏事。
以及人生有无限种生活方式的选择，尊重它、适应它、拥抱它， 并以自己期望的那样去过自己的生活， 共勉。

## 06.09
要事第一、积极主动、以终为始
## 04.11
怎么才能别死的早，很早就看到了：https://github.com/geekan/HowToLiveLonger 程序员延寿指南，这里总结一下：
```
输入
固体：吃白肉（-11%~-3% ACM）、蔬果为主（-26%~-17% ACM），多吃辣（-23% ACM），多吃坚果（-27%~-4% ACM），中量碳水、多吃植物蛋白（-10% ACM），少吃超加工食物（-62%~-18%）
液体：喝咖啡（-22%~-12% ACM），喝牛奶（-17%~-10% ACM），喝茶（-15%~-8% ACM），少喝或不喝甜味饮料（否则每天一杯+7% ACM，+多巴胺），戒酒（否则+~50% ACM，无上限）
气体：不吸烟（否则+~50% ACM，-12~-11年寿命）
光照：晒太阳（-~40% ACM）
药物：二甲双胍（糖尿病人相比正常人可以+3年）、复合维生素（-8%癌症风险）、亚精胺（-60%~-30% ACM）、葡萄糖胺（-39% ACM）
输出
运动：每周3次45分钟挥拍运动（-47% ACM）
日常：刷牙（-25% ACM）
睡眠：每天睡7小时全因死亡率最低；且22-24点间最好，早睡+43% ACM，晚睡+15% ACM（存在争议）
上下文
体重：减肥（-54% ACM)
```
## 04.01
在印尼进行了为期4日的旅行，由于没有带充电器的转换器，因此极大的减少了手机的使用。反而让我获得了很多以往没有的体验，比如在 Probolinggo 等 minibus 前往 bromo 的时候，可以无所事事的坐在树荫下，不玩手机的等待其他人的前来。
这在以往的生活中，貌似很难做到，但在那天的日子里，却并没有觉得很难熬。以往的日子里，貌似一个小时内不看上几次手机，好像就会失去很多貌似很“重要”的信息，但在不怎么使用手机的日子里，发现那些以往觉得很重要的东西，也变得没那么重要了
倒是很有意思的体验

## 02.20
找到要素，建立连接，形成系统，发现规律，建立模型，推动发展

## 2.05
业务思维：一种高效挖掘和满足用户需求以及预期的思维

业务拆解及数据链路
- 数据生产：业务转化链接拆解，找到与预期不符合的瓶颈去细化，不断拆解细化补充，搭建起基本预期。
- 处理数据：
- - 业务落地，本质上是通过 feature 把产品提供的预期不断往用户预期拟合的过程
  - 数据去筛选出各种预期，是数据最重要的作用，而非仅仅只是监控现状
  - 对数据要有合理的怀疑，需要经过不断地验证，确定不同要素是直接相关性还是间接相关，还是只是“看起来”相关，如辛普森悖论（https://github.com/srtian/Record/edit/main/README.md#203）。
## 01.17
```
## Importance of Asking Smart Questions:
- Open source usage has made it possible to get good answers from experienced users.
- Treating experienced users with respect and asking thought-provoking questions is essential.
## Preparing to Ask:
- Hackers like hard problems and insightful questions.
- Demonstrate that you have done your research before asking a question.
- Display what you have learned from the research to show that you can learn from the answers.
## Asking the Question:
- Frame the question in a way that invites others to get involved and demonstrates respect for their abilities.
- Avoid demanding answers and instead ask for help in a polite manner.
## Problem-Solving Approach:
- Encourages a problem-solving approach through research, experimentation, and seeking answers from skilled friends or the source code.
## Building Relationships:
- Asking the right question and listening to the answer is a great way to build relationships.
```
# 2023
## 12.18
how to remenber every thing when we reading book

- have a couple of goal and make sure some info that we will get from the book
- make note and highlight for book, record you thought and perspective
- when finish read , orangrize the onte, categories the notes, and if can do, just practice it

## 11.16
Most often, we do not strictly define knowledge, but we align it with other related concepts using DIKW Pyramid. It contains the following concepts:
- Data is something represented in physical media, such as written text or spoken words. Data exists independently of human beings and can be passed between people.
- Information is how we interpret data in our head. For example, when we hear the word computer, we have some understanding of what it is.
- Knowledge is information being integrated into our world model. For example, once we learn what a computer is, we start having some ideas about how it works, how much it costs, and what it can be used for. This network of interrelated concepts forms our knowledge.
- Wisdom is yet one more level of our understanding of the world, and it represents meta-knowledge, eg. some notion on how and when the knowledge should be used.

<img src="https://github.com/microsoft/AI-For-Beginners/blob/main/lessons/2-Symbolic/images/DIKW_Pyramid.png" alt="" width="30%" />

> AI-For-Beginners: https://github.com/microsoft/AI-For-Beginners/tree/main
## 11.03
![image](https://github.com/srtian/Record/assets/38072743/d56a1d5e-c22d-4bcd-9c68-fd122eb3aa17)
> https://engineercodex.substack.com/p/how-instagram-scaled-to-14-million

## 10.27
 It’s enough to just keep moving in a forward direction, without competing with anyone.
 > 《The Courage to be disliked》

## 10.19
#### Ten Rules to Live By to Achieve Success
> FROM THE intp ADVISE
1. Feed Your Strengths! Realize your gift at mastering logical problems and situations, and
give yourself plenty of opportunities to exercise your abilities. Much of your sense of well-
being will come from these experiences.
2. Face Your Weaknesses! We all have weaknesses. Recognizing your weaknesses for what they
are (without beating yourself up) will give you the power to change your life for the better.
3. Talk About Your Thoughts. Discussing your ideas and perceptions with others will help
you to develop your Extraverted iNtuition, and thus your understanding of the world. How
well you use your auxiliary function is very important to your overall health and happiness.
4. Listen to Everything. Try not to dismiss anything immediately. Let it soak in, and
then apply judgment. Try not to dismiss things that are illogical – they are not illogical.
5. Be Aware of Others. Understand that everyone has their own lives and their own
perspectives. Everyone has something to offer. Try to identify people’s personality type.
6. Recognize Social Principles. Realize that our society functions around some basic social
principles, and that our society would fail unless those principles are recognized and upheld.
In a democracy, people vote. At a red stoplight, people stop. If people stopped voting because
it wasn’t important them, who would be in power? If people stopped stopping at red stop
lights because it didn’t fit into their plans, how could we drive safely? Your priorities
and plans are important, but you must recognize that the external world’s agenda is also
important. Don’t dismiss the importance of principles that don’t affect your life directly.
7. Get Out of Your Comfort Zone. Understand that the only way to grow is to get outside
of your comfort zone. If you’re uncomfortable with an idea or situation because you’re
not sure how to act, that’s good! That’s an opportunity for growth.
8. Identify and Express Your Feelings. You may have a hard time understanding how you
feel about someone. It’s important that you do figure this out. Don’t lead someone on with
your ambivalence. If you determine that you value the person, tell them so every time you
think of it. This is the best way to make them feel secure in your affections, and so to promote
a long-lasting relationship.
9. Be Accountable for Yourself. Remember that no one has more control over your life
than you have. Don’t be a victim.
10. Assume the Best. Don’t distress yourself with fear and dark expectations. Remember
that a positive attitude often creates positive situations.
## 9.15
"重要的不在于你的努力程度，而在于仔细选择工作、人员和项目。"

"真正有效的工作方式，不是铁人三项或马拉松，比拼谁坚持的时间长，而是短跑，当机会来临的时候冲刺，平时注意健康和休息。"

"你要像狮子一样，看到猎物一跃而起，而不要牛一样，从早到晚劳作。"
## 8.25
Effective > Productive

Productive: We must fill our schedule and do a lot of work
Effective: something maybe we just need to do, but the other thing we don't need to do it. so just cut it out.

> so We believe in effectiveness. How little can we do? How much can we cut out? Instead of adding to-dos, we add to-don’ts.
## 8.07

1: Eat food in the right order: veggies first, protein second and carbs at the end. Eating fibers first slows down the absorption of carbs and therefore decreases the likelihood of a glucose spike.

2: Add a green starter to all your meals: The goal is to include more fiber in your meals which prevents a glucose spike.

3:Stop counting calories: Foods that are high in glucose could be low in calories and food high in calories could be low in carb but more fulfilling and beneficial for our body. For example a donut and cup of yogurt both contain 150 calories but the donut will cause a glucose spike but the yogurt will not because of the protein and fat content.

4: Flatten your breakfast curve: cereal with milk, fruit smoothie, muesli and fruit juice all cause a big glucose spike. A good breakfast that won't cause a glucose spike is usually savory and contains a good amount of fiber, fat, protein and optional starch and fruit. Our body is very sensitive to glucose following breakfast because it has been in a fasting state for a long time. Also, given how well maintained the glucose spike was after breakfast- our body is better able to manage the blood glucose level for the rest of the day. 

5: All types of sugar are the same: Basically there is no difference between maple syrup, honey and white or brown sugar. One is not healthier than the other when it comes to causing glucose spikes. The best types of sweeteners that have no side effects on glucose and insulin levels are: Allulose, monk fruit sweetener, stevia (pure stevia extract), erythritol. Artificial sweeteners recommended to avoid are aspartame, maltitol., sucralose, xylitol, acesulfame-k.

6: Pick a dessert over a sweet snack: Taking a sweet snack over an empty stomach causes glucose spikes. If you are craving something sweet, take it after a meal as a dessert.

7: Reach for vinegar before you eat: Taking 1 tablespoon of vinegar in a tall glass of water taken before the meal (with a straw to avoid causing problems with tooth enamel) decreases the glucose spike. The acetic acid in vinegar temporarily deactivates alpha-amylase which is an enzyme that turns food into glucose in our body. Additionally, acetic acid encourages our muscle to take glucose faster than the bloodstream without releasing additional insulin.

8: After you eat, move: Doing a 20 minutes exercise within 70 minutes after a meal is shown to reduce glucose spikes.

9: If you have to snack, go savory: Most popular snacks like potato chips, granola bars etc are carb heavy and cause a glucose spike when taken as a snack.

10: Put some clothes on the carb: When you have to get something on the go, choose meals that combine starches/ sugars with fat, protein and fiber. Basically putting some clothes on the carb and not taking them alone. Example, some apple/ pear with nut butter.
## 7.28
Why the open-source customer service mode can't get money?
- Customer service mode has thin profits, and customers are unwilling to pay high prices for support services.
- Customer service is difficult to scale. Customers may use the software extensively but only purchase one service.
- customer service mode cannot achieve high-speed growth. The easier and more reliable the software is, the less users need to purchase support services.
- It is difficult to generate early revenue in customer service mode. Start-up companies may struggle to find 100 initial users, among whom only a few may purchase services, and perhaps none at all.
## 6.16
这个世界日以继夜、竭尽全力让你成为其他人，如果你想做你自己，就意味着要打一场最艰难的仗。
## 6.12
Everyone is trading with their future selves.
## 5.02
ChatGPT 的快速进化和世界经济衰退周期的到来，着实让我最近有点迷茫，不过这两天有点感冒，躺着想了一想，倒有了一些头绪：
1. 要拥有面对现实的能力，什么是面对现实的能力？1. 心态好，open-minded 2.把力所能及的事情做好
2. 也要保持一定的理想主义 1. 未来总会更好的 2. 心气要好，保持持续的学习，敢于走出舒适圈，敢于探索
3. 保持耐心，日拱一卒，还有用老板的话来讲：延迟满足
## 4.21
和老朋友聊到了 leetcode，就热血来潮看了下自己当年刷的题，发现也有不少用 golang 写的，虽然现在几乎完全不记得 golang 的语法了：‘
![image](https://user-images.githubusercontent.com/38072743/233534745-87b8adb3-9647-4ceb-bf9a-5949b4d3092c.png)

编程语言这东西，学习的时候会记住很多 API 和特性，但实际经过几年，很多东西都会不记得，剩下的要么就是很好的特性，要么就是不好的，比如 Golang 的错误处理，我虽然不太记得语法了，但还是记得 golang的一些名言警句：1. 不要使用共享内存来进行通信，要用通信来共享内存 2. 组合大于继承。by the way, golang 的错误处理，我还是觉得很蠢，尤其是接触到 rust 之后。

所以不由引发了一些思考，语言层面，什么特性是好的，什么特性是坏的，想了想大概可能有这些点：
- 该特性是否被诸多的编程语言所采用，那么它大概率是有其充分的理由的
- 特性本身都是基于场景考虑的，不能用一元论来考虑它，一个东西觉得很烂，还是要去了解这个特性设计的背景以及所要解决的问题

## 3.28
I have spent some time reading this post: https://www.gatesnotes.com/The-Age-of-AI-Has-Begun
Although it doesn't have the technical depth, just Bill's thinking about AI when ChatGPT is open. I also learn a lot from it.
- AI can improve the efficiency of many industries, freeing people to do things other than their own industry waiting to be done.
- AI may be able to reduce the inequity, but it needs the government or some organization to push and control it.
- Advances in AI will enable the creation of a personal agent. For example, health and education.
## 3.22
B 端交付
将客户满意度做为关键项目目标去管理
1. 客户 和 用户
   1. 客户是 buyer
   2. 用户是产品所服务的人，是直接使用者。客户和用户不一定是同一个人
2. 项目交付的，本质上是交付客户的心理预期

客户满意度管理
- 知己知彼：识别客户的决策链条
- 过程管理：管理好与客户的分工界面，客户的参与度、期望以及需求变更
- 满意度调研与回访：做好满意度调研与改进

客户满意度 = 客户体验 - 客户期望

客户期望管理的四大原则
1. 倡导契约化交付
2. 以最满意的代价、达成客户期望
3. 提出可能遇到的困难及解决方案
4. 客户期望需要被动态管理

## 3.20
前段时间学习了 @左霆 关于 Saas 相关业务的分享，收获颇丰。算是将 who is your buyer? 这一句话映射到了脑海里。下面关于分析的一些总结：

1. 本质上，早期的科技企业和现代的科技企业，在技术设施的依赖上，是一致的：由对硬件的依赖（Oracle、SAP），到现在的云厂商或者服务提供商（Salesforce，Workday）
2. Saas为什么如此众多？公司本身是复杂的，各部门各司其职，各个Saas对应不同的职能。因此我们是否需要一开始就要有一个大而全的解决方案？并不是，先确定谁是我们的buyer，通过创新，解决他们的问题，然后在进行创新发展，进行扩大（go to market 很重要）
3. 确定自己的用户是谁（Who is you buyer），并计算他们的购买力。以及我们想要完成的营收规模，营收 = 用户数 * 单位购买价。在这个公式中需要考虑几个事情
    1. 高的单位购买价，势必会减少用户数，反之亦然。
    2. 低购买价意味着用户留存会是一个问题（沉默成本小，但也意味着不需要做很定制的事情，基本只需要提供公共方案即可）
    3. 低购买价的情况下，需要提供自主购买渠道，减少销售团队（ROI的问题）
4. SaaS 业务很重要的一点在于：who is your buyer? 思考明白这个问题，很多东西都能有答案了
5. Ending ARR = Starting ARR + ACV - churn
    1. Better version: Ending ARR = Starting ARR + (ACV from install base - Churn) (ACB from new logos)
6. 增涨策略：
  - Acquire you initial set of customers
  - reduce your churn rate
  - expand your sales team
  - Increase value though upsells and cross-sells
  - Launch into a new segment
  - Go international
  - Maximize growth opportunities through acquisitions
  - Optimize your pricing & packaging
8. 流失分为两种：
    1. initial churn
    2. Long term churn
9. Pricing Strategies
  - Choosing the variable unit 
  - Licensed in advanced VS Tracked in arrears
  - adding a fixed component
  - Consumption models: when and how to use 

## 3.14
[Think Fast, Talk Smart: Communication Techniques](https://www.youtube.com/watch?v=HAnw168huqA)
1. Acknowledge and embrace anxious feelings when they arise before a speech, and take deep breaths to prevent anxiety from spiraling out of control.
2. Reframe public speaking as a conversation rather than a performance, and use inclusive language and relaxed body language to engage the audience.
3. Practice being present in the moment by using techniques such as doing pushups, walking, listening to music, or trying tongue twisters.
4. Let go of the need to be perfect and improvise instead of stockpiling information.
5. View things as opportunities rather than threats, and take a "Yes, and..." approach rather than a "No, but..." approach.
6. Slow down and listen to understand the needs and perspective of the audience.
7. Use structured responses, such as the "Problem > Solution > Benefit" or "What? So what? Now what?" structure, to keep the audience on track and increase processing fluency.
8. Practice improvisation to improve spontaneous speaking skills.
9. Use visual aids and props to enhance the effectiveness of the speech.
## 2.25
这几天看了本：《创造》：https://book.douban.com/subject/36071759/?_dtcc=1
有几个观点很有收获：
- 你的产品不仅仅是你的产品。它是一套完整的客户体验——从人们第一次了解你的品牌开始，一直到你的产品从他们的生活中消失、被退回或扔掉、被转卖给朋友或报废才算结束。
- 乔布斯总是说类比能赋予客户超能力
- 进化：通过微小而渐进的步骤使事情变得更好。
- 颠覆：进化树上的一个分叉，从根本上改变现状的新事物，通常是以一种新颖或革命性的方法来解决老问题。
- 执行：将承诺的事情做到实处，并且做到极致。
- 以下是你在做决策时需要的各种工具，已按重要性排序（这是第一阶段，第二阶段的优先级是：数据，客户洞察，愿景）
  1. 愿景。你要知道自己想做什么，为什么要做，为谁而做，为什么人们会购买它。你需要一个强大的领导者或一个小团队来确保愿景能够完整实现。
  2. 客户洞察。你通过客户、市场调查或像客户一样思考而了解到的一切：他们喜欢什么，他们不喜欢什么，他们经常遇到什么问题，他们会期待什么样的解决方案。
  3. 数据。对于任何真正的新产品，可靠的数据都是有限的或根本不存在。这并不意味着你不能就客观信息的收集做出合理尝试。你可以就未来机会的大小，人们如何运用现有解决方案等问题收集信息。但要记住，这些信息永远都是不确定的，它们无法替你做决定
- 从本质上来说，设计就是思考一个问题并为其寻找到一个优雅的解决方案。
  1. 运用设计思维：这是创新设计公司IDEO的大卫·凯利提出的一个著名策略，它鼓励你识别客户及其痛点，深入理解你试图解决的问题，并系统地发现解决问题的方法。
  2. 避免习惯化：每个人都会习惯一些事情。生活充满了微小和巨大的不便，但你早已对它们视而不见，因为你的大脑已经将其认定为不可改变的现实，并对其进行过滤。

- 绝妙的想法都具备以下三大要素。
  1. 它解决的是“为什么”的问题。要想弄清一款产品能做什么，你先要了解人们为什么需要它。“为什么”驱动着“是什么”（见第10章）。
  2. 它解决的是很多人在日常生活中遇到的问题。
  3. 它会一直萦绕着你。即使在你研究和了解了它，试用了它，并且意识到很难完全搞懂它的情况下，你也无法停止思考它。 

详细的摘录在这：https://www.notion.so/srtbooks/0eb40adc7f4f48b786a941069fdd3e24
## 2.22
今天的 byteTalk 倒是有不少收获，大佬也分享了自己的一些经验
1. 持续努力很重要，一周挤出10小时，建立长期学习习惯；日拱一卒；
2. 顺势而为、调整心态 
3. 有基础、有乐趣的事情去努力 
4. 克服焦虑：调整心态，不要焦虑，控制目标和欲望，不要比来比去 
5. 保持开放，看看别人的优点，从别人优点上学习，合作共赢 
6. 10亿*2*365=中国市场天花板，中国人均收入100元，人均2元，7300亿附近。 10亿*5*365=发达国家市场天花板，人均收入300~400元
7. 要去识别高 ROI、高容错的事情
## 2.16
拜占庭将军问题

拜占庭将军问题提供了对分布式共识问题的一种情景化描述，它是分布式系统领域最复杂的容错模型，他描述了如何在存在恶意行为的情况下，使分布式系统达成一致。（它也是区块链的基础）

他的背景是拜占庭王国的几支部队在一齐进攻一个城堡，每支部队都有自己的指挥官。而要取得进攻的胜利，需要所有的部队一起攻击才行。他们制定的计划在于，如果需要进攻或者撤退，都需要半数以上的将军一起发起进攻才行。而此时，如果其中部分将军或者信徒出现了叛徒，他们就可能伪造或者篡改消息，至少大家收到的消息是存在错误，致使大家做出错误的行为。

论文《The Byzantine Generals Problem 》同时提供了两种解决拜占庭将军问题的算法：

1、口信消息型解决方案(A solution with oral message);
- 被发送的消息能够被信使正确传递
- 接受者知道消息是哪个将军发的
- 能够知道谁没有发送消息

2、签名消息型解决方案(A solution with signed message).
- 将军使用印章对书信签名，这个签名就确定了将军的身份，不可伪造，篡改签名可被发现
- 收到书信的任何其他将军都可以验证签名的有效性

## 2.15
睡觉前花了点时间将 王煜全 的人生的意义 一系列文章看完了：
![image](https://user-images.githubusercontent.com/38072743/219352112-993d2231-2d9e-4168-b508-7e3b7aa97f58.png)

总结几点有收获的点：
- 提升输入的能力，是提升自我认识模型的关键
- 人类的第一性原理就是进化论，进化本身不仅发生于个体也可能出现于群体
- 反馈是个好东西，最好的方式就是快速得到反馈，然后不断进行调整策略，实现进步与提升


## 2.10
看见一篇关于技术人如何做好业务的文章，写的很不错：https://www.yuque.com/antfe/featured/mzncwxg7tdut412q

主要需要注意以下几点：
- 心中有业务大图：业务的核心逻辑、上下游情况、现状（成果、现阶段的痛点），以及现阶段的重点目标。对于业务的中长期，行业，前景都有一定的认识与把控
- 在自己的方向足够专业：可以快速判断能不能做、怎么做、需要投入多少人力做
- 推动业务进步不设限
  - 业务迭代节奏和质量
  - 产品体验
  - 产品能力调研
  - 外包管理技巧
  - 数据驱动
- 被需要的时候全力以赴
- 创造线下见面的机会（先聚人，后做事）
- 把吐槽改为建议
- 相互理解、大目标一致（同理心，善意假设）

## 2.07
public chain of record something produces can be used for:
- Fairer voting systems
- Secure sharing of medical data
- Personal identity security
- Recording real estate transactions
- Gambling
## 2.03
辛普森悖论指的是：数据集分组呈现的趋势与数据集聚合呈现的趋势相反的现象。
解读数据（或者是观点）的角度和方式不同，都可能产生完全不同的结果。（这让我想起了一句话：掌握解读权，就掌握了具体的权力）

如何解决悖论？
1. 了解数据是如何产生的，是否本身就不足以展现全部的面貌
2. 对于得出的结论，是否还有其他的因素在进行影响

------------------------

I read an article on how to render conditional components. I've done this a lot before, but I'm not as good at TS type as he did
![image](https://user-images.githubusercontent.com/38072743/216534724-f9af0545-09f7-4491-b707-6e063b95446b.png)
> https://www.lloydatkinson.net/posts/2022/react-conditional-rendering-with-type-safety-and-exhaustive-checking/

## 1.30
A component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller sub components.

Three things should be considered when building a component:
1. What is the one responsibility of this component? 
2. What’s the absolute minimum, but complete, representation of its state? 
3. Where should the state live?


## 1.28
能够生存下来的物种，并不是那些最强壮的，也不是那些最聪明的，而是那些对变化做出快速反应的。——达尔文《物种起源》

## 1.25
培养钝感力的5个方法:
1. 建立自信
2. 不要猜
3. 过滤噪音
4. 关我屁事
5. 关你屁事

## 1.19
最近越发感觉到 善意假设 的力量了。一方面他能让我们在思考他人的行为时可以优先往好处想，有利于合作&团结；另一方面，这也是一个可以有利于与自己和和解的方式，少了很多糟心事。

# 2022
## 12.19
Better than free: https://kk.org/thetechnium/better-than-fre/

When copies are free, you need to sell things which can not be copied.

so what should we do? this essay tell us about eight things better than free:

1. Immediacy
2. Persionalization
3. Interoretation
4. Authenticity
5. Accessibility
6. Embodiment
7. Patronage
8. Findability

## 12.02
how to use prvlink?
![image](https://user-images.githubusercontent.com/38072743/205234531-e76bb719-4a99-435a-bbb1-604a8e9e844a.png)

## 11.25
We should build a system instead of software，and how we build a system?
![image](https://user-images.githubusercontent.com/38072743/203888905-47b57ff6-d409-45ad-809a-cafba4a0fce5.png)
ref: https://codewithstyle.info/software-vs-systems/
## 11.24
a very interesting example of soild.js: 
![image](https://user-images.githubusercontent.com/38072743/203690472-f246f5f1-39bd-491a-a3e2-9c45d2da80ce.png)

it's very clear

## 11.18
https://www.reforge.com/blog/how-to-make-career-decisions

Impact = Environment x Skills

## 11.11
I have seen an article about English studies written by Wanying. You can check out the article for more detail: https://www.yinwang.org/blog-cn/2020/03/06/english-learning-tips and https://www.yinwang.org/blog-cn/2018/11/23/grammar.

It has some advice:
1. practice using verbs to make sentences, the more the better
2. use the grammar tree to analyze the sentence

![image](https://user-images.githubusercontent.com/38072743/201252850-c7892979-f837-46fd-b5bd-350692c0f5aa.png)

## 11.07.
Second-order thinking:

Do you know what second-order thinking is? When something happens, we should know the effect of the thing, we should ask ourselves "and then what", and we should think about it more deeply and think more deliberately.

Here's some advice. First of all, we should ask ourselves "and then what". Second, we should consider the effects of events over 10 minutes, 10 days, 10 months, and 10 years.
## 10.28
软件的可观察性有三大支柱：指标、跟踪和日志。

## 10.20
《西蒙学习法》
其中有一个很有意思的法则，721法则 —— 10%的时间用于了解这项知识的概念以及信息，20%的时间与人讨论，70%用于实践与练习。
这种分配感觉很适用于像编程这种需要大量练习的技能。

延迟满足的练习方式
- 当对一件事情有所欲望时，等待10分钟再看看
## 10.15
看王建硕关于 Web3 的一些论述，感觉收获颇丰：
1. Web3 本身这个名字起的很差，因为其本质是区块链的应用层，和 Web 的关系不大。
2. 对于区块链，简单的可以理解为：一张统一的大的表，上面的数据只要写入进入就不能再更改
3. 这会带来新的变革，正如信息技术极大的提升了信息的传递速度，区块链maybe可以解决数据真实性以及不可篡改性的问题（对于应用场景是否真的足够的宽广，我还是存保留意见的）
## 10.14
a short article is about what people are about to die what's they most regret things:

![image](https://user-images.githubusercontent.com/38072743/195794491-6523639d-da42-45e7-a3d6-ee799115a79b.png)

## 10.13
### 《醉汉的脚步》
1．认识这个世界是未知的、随机的、概率化的；

2．认识你的认知是不确定、有边界的；

3．我们找到自己基于概率的算法，建立持续稳定的输出系统。因为我们一生中最大的变量，是时间；

4．复制“核心认知”，如同每个生命所做的那样；

5．成为一台“强化学习”的机器，加速计划，实现人生算法
## 10.11
the act of breaking a complex problem down into smaller problems, and composing simple solutions to form a complete solution to the complex problem

-- 《Composing Software》
## 10.10 
### 《少有人走的路》
如何才能通过自律消除人生的痛苦呢？简单地说，所谓自律，就是主动要求自己以积极的态度去承受痛苦，解决问题。自律有四个原则：推迟满足感、承担责任、忠于事实、保持平衡。

## 10.09
我的灵感来源于博恩·崔西 ( Brian Tracy ) 的著作《价值百万的习惯》(Million Dollar Habits)，这本书用 7 个阶段概括了达成目标的方法：

第一阶段，树立目标

第二阶段，设定截止日期

第三阶段，制作目标清单

第四阶段，拟定行动方案

第五阶段，消除障碍因素

第六阶段，立即实践

第七阶段，持续推进
## 10.05
近日在佛山旅行，去了祖庙、西樵山、影视城等地方，也穿过了佛山的大街小巷。我还是很喜欢这种老城区的，总是给我一种岁月拂过的气质，沉甸甸的，有意思。
另外这两天其他的体会是：钱经用很多了，这边大部分的消费都比深圳要小的多，一顿饭吃的很不错也只需几十块，而这个价钱在深圳一顿外卖就解决了。

## 9.20
- “最小复杂度不会凭空消失”，而一般情况下可能会因为操作过程不是最佳，还可能会引入额外的复杂度。
- 看任何原则、理念、方法的时候都不能脱离上下文和适用场景、教条式的理解
## 9.19 
### 读《娱乐至死》
最近读了娱乐至死，有以下一点体会：技术决定媒介，媒介决定信息传播的方式。信息娱乐化，需要保持对于娱乐的限制，信息源的控制，减少不必要的信息的摄入。

## 9.16
幸运 = 你做的事情 x 知道的人数

## 9.08
A great tool is just like a pair of glasses. They help you see the world, not the glasses.

## 8.21
如何保持工作时的专注？看到几个很不错的建议：
1. 关掉所有的推送；
2. 操作你的工作环境。
3. 像狗一样训练自己，在工作一段时间后奖励10分钟，并严格执行下一轮回。最好的工作成果来自于极长时间的专注。

## 8.12
为什么要制定计划？

制定一个计划，就是为了实施。计划的唯一目的是确保得到更好的结果。
如果不去实施，计划本身并没有价值。如果你清楚地如何得到结果，完全可以没有计划。

## 8.11
R.W.保罗描述了6种类型的苏格拉底式提问。简单地浏览一下这个列表后，你可能会明白这些问题是如何帮你提高学习水平、填补知识上的空白的。这6种类型的问题包括：

·　①澄清式提问：为什么这很重要？

·　②探索假设式提问：可能存在哪些隐藏的假设？

·　③探究原理、理由和证据式提问：有哪些已证实的证据？

·　④质疑观点式提问：还有哪些其他的观点？

·　⑤探究意义和结果式提问：这意味着什么，意义是什么，它如何与其他信息联系起来？

·　⑥针对问题本身的提问：为什么这个问题很重要？

## 8.07
记录一下泉州一个好吃的：泉港浮粿

## 8.05
最近看到一些话，觉得挺有道理，记录一下
#### 让事情发生的能力
人们拥有一种神奇的能力，就是使事情发生。但是大多数人从来不敢尝试这种能力，只是默默接受世界本来的样子。

#### 软件开发的目的
软件开发的目标不是类型安全、100%的测试覆盖率、流畅的代码逻辑、完善的开发工具、高效的系统、使用最好的编程语言、优雅的 API 设计、快速的反馈循环、编写很棒的代码等等……

软件开发的真正目标只有一个：发布解决客户问题的软件，为客户提供价值。

## 7.27
如何学习语言？有几点假说值得借鉴：

1.习得-学习假说：我们要尽量使用一个自然的方式来学习一门语言。

2.自然顺序假说：学习语言要跟顺序，先听后说，先读后写。如果我们感到口语水平不足那么就要先提高听力，如果我们感到写作水平不做那么我们就要先提高阅读。

3.监督者假说：性格较为内向的人会格外注意自己是否遵守语言的规则，但还是要尽量减少监督者的影响。犯错误是当然的，大胆开口说

4.输入假说：在我们决定通过一个跟传统教材不一样的方式接触语言的时候，尽量去选择对语言水平要求比较高的内容，比我们水平更高一层的。虽然可能会更累一点但对我们的学习有相当大的帮助。

5.情感过滤假说：无论好的情绪还是坏的情绪，都会对我们的学习产生某种影响。学习语言要讲究气氛，不要以负面的情绪对待语言更不要以负面的态度面对上课。
## 7.25
How to be a great software engineer? We should know about these topics:
1. Personal characteristics
2. Imporoving
3. Passionate
4. Open-minded
5. Data-driven

## 7.16
马斯克最新解读，创新不能类比，第一性原理下的五步流程法：1.让需求不愚蠢；2.删减提炼；3.优化迭代；4.提升效率；5.自动化。

## 7.10
训练大脑的方法：
1-积极参与解决问题
2-有动力寻找信息了解世界
3-利用信息联系能力（把你所知道的和不知道的联系起来）
4-要有对知识探索的积极态度

最后：知道的越多，就越聪明
## 6.28
富人思维 = 想尽一切办法【参与】进自己看好的项目或者人

## 6.23
如何应对人生中一些比较灰暗的时刻？
1. 不是所有发生在你身上的事都是你的错，但发生在你身上的事都是你的责任
2. 不必他人认可自己，自己认可自己，生活会变得更顺
3. 没有人欠你什么，不如专注于提升自己。
4. 一切都会好起来的。生活就是这么奇怪，都会历经黑暗时期，不如以谦逊和坚持的态度，面对任何情况，总会有好的结果出现。

## 6.19
一些有意思的定律：
1.需求定律：作为一个生意人，你永远要做能为别人解决问题的生意。
2.进入定律：说的是你在进入一个行业时，越容易走的路就越挤，难度越大的路走的人越少，竞争者少，但难度大不代表没法走。
3.控制定律：把控制权要掌握在自己的手上，如果是老板，可以控制员工的时间、精力、体力等，但员工就没办法控制。
4.规模定律：影响力越大，你的发展空间和财富空间越大。

## 6.17
一件事最可怕的时刻，总是在你开始做之前。
-- 斯蒂芬·金

对于那些没有想象力的人来说，保持常态就是他们的理想。
-- 荣格

## 6.12
最近看了《非暴力沟通》，最简单来讲需要这样：不带评论的观察对方内心的感受以及感受背后的需要。

非暴力沟通 = 感受+需要

## 6.08
PDCA

具体解释：“Plan（计划）”→“Do（执行）”→“Check（检查）”→“Action（改善）
- 规则1．可视化——PDCA只要可视化就能循环起来
- 规则2．系统化——PDCA系统化后就能循环起来
- 规则3．习惯化——PDCA习惯养成后就能循环起

## 6.07
帕金森定律
1. 自己设定一个最后期限，在期限内完成任务，最后期限根据自己情况可提前
2. 将大目标分解成小项目，再为每个项目定一个较早的最后期限
3. 创造挑战，设置一个十分具有挑战性的最后期限，让自己在不可能的时间段内尽可能完成任务，使自己投入其中尽力做就可以了
4. 将帕金森定律用于日常生活，为工作或生活设置最后期限，帮助自己省出更多空闲时间。甚至可以尝试提前一天完成每项任务。

## 6.05
今天看了陈天老师的分享，感觉收获不少，总结如下：
1. 学习金字塔 / 新技术学习的飞轮效应
2. 寻找适合你自己的技能路线图
3. 怎样养成高效自学的习惯
4. 近一两年来我学习的几门技术的一点总结
- rust
- blockchain
- dart/flutter

5. 上手
- 从小处开始，不断扫清障碍
- 「阅读」别人的文档代码，「抄袭」别人的思想
- 在线上线下寻求辅助（芒格名言）
- 不断在项目中历练
- 寻求知识和技能背后的本质和规律
6. 输出

### 飞轮效应？
“飞轮效应”这个概念我最早是从张潇雨在得到专栏中学到。去年上刘润老师商业洞察力课程，刘润老师的正反馈回路和调节回路也是一种飞轮效应。这个概念是亚马逊和贝佐斯本人反复强调过的一个商业理念。“飞轮效应”是指，一个公司的各个业务模块之间，会有机地相互推动，就像咬合的齿轮一样互相带动。一开始从静止到转动需要花比较大的力气，但每一圈的努力都不会白费，一旦转动起来，齿轮就会转得越来越快。亚马逊有的Prime会员业务（一人每年99美金）、Marketplace平台（第三方商家卖产品的平台）和AWS亚马逊云服务（Amazon Web Services）。Prime会员业务会大幅地提高客户忠诚度，亚马逊会员在购买频次上和购买金额上都会比非会员高出很多。Marketplace平台允许第三方商家来卖产品，就使得客户可选择的商品大大增加了，当客户的选择增多，Prime会员就更加超值，所以买会员服务的用户也会增加，当亚马逊的客户越来越多，也就有更多的第三方商家愿意来亚马逊开店。任何商家都可以把自己的整套系统放在AWS上，这样你不仅在亚马逊上卖货，还用亚马逊的FBA服务做物流，又在AWS上运行着自己的IT系统，这样无法离开亚马逊。

上述这一系统机制导致亚马逊的商品越来越多，客户选择就越多了，进而购买会员服务的就越多，用户消费的频次和额度就越多，亚马逊对第三方商家压价就越多，用户的获利也就越多……这个飞轮不断旋转，也成就了二十年的蒸蒸日上。这就是亚马逊这家公司真正的秘诀。

苹果公司也有类似的飞轮效应，iPhone卖到10000元也照买不误的忠实粉丝、App Store应用商店、Apple Music、Apple News、iCloud、AppleCare和Siri都是飞轮的一部分。

飞轮效应本质上就是一个生自给自足的态系统，是一个小世界。这个世界有至少有着相互影响的三个主体，分别是生产者、服务者、消费者，生产者是提供消费者所需要的产品或服务，服务者是为这个过程的顺利开展提供协调服务的。苹果和亚马逊两家公司都构建整个服务平台使得生产者和消费者愿意参与甚至不舍得离开。

对于个人而言或者个人创业，也需要找到自己的飞轮，打造自己的核心竞争力。刘润老师创立润米咨询公司找到的因果链是声誉和收入，围绕打造他的声誉启动了三个飞轮，声誉，学识和作品是刘润老师的三个飞轮。他用公众号，微博和抖音推动他的声誉飞轮，用商业咨询，私董会，教练工坊等推动他的学识飞轮，用线下课，5分钟商学院和图书出版推动他的作品飞轮。这三个飞轮形成正反馈回路，推动他的声誉越来越好，随之而来他的收入越来越多，他又把收入投入到声誉的提升过程中。巴菲特说，他最大的爱好是读书，读书是人类获取知识和洞察力的重要飞轮，巴菲特把他书中所学到和领悟到的应用于投资中，他投资赚到的钱越多，就有越多的人买他的基金，通过不断的复利使巴菲特一度成为世界首富，形成了他的正反馈回路。

## 5.24
福格行为模型 = 提示+动机+能力

## 3.20
高质量沟通=彼此的理解的增量=观察提问+积极倾听+自我袒露

【观察提问-开场白】

开场白1:说出双方的相似之处

开场白2:利用观察&提问表达称赞（容易被忽略的优点）

【观察提问-阶段提问】

进阶1:询问对方的独特观点

进阶2:请教对方擅长的事情

进阶3:挖掘对方的经历

【积极倾听-他说你听】

方式1:对特殊经历表述惊叹

方式2:表示关心对方的权益

方式3:表达真诚的祝贺

方式4:反馈对方的强烈情绪

方式5:支持认可对方的意见

方式6:适当做表情帝或复读机

【自我袒露-你说他听】

场景1:先反馈，后发言

场景2:出其不意；幽默一下

袒露方式：事实、观点、感受

要点1:倾听袒露，有来有往（三步公式）

要点2:由浅入深，循序渐进

【重点】

场景1-引导对话:见缝插针，抛砖引玉

场景2-回收对话:见机行事，举一反三

场景3-大脑短路：Be water ，my friend

## 3.16
技术派正能量
1. 避免过度交易，长线持有
2. 组合多样，主力合约，交易活跃月份
3. 不试图抄底，右侧交易，不预测，顺势不逆势
4. 知行合一，铁一样的纪律不因情绪动摇
5. 知者不言，言者不知。不瞎给人意见，也不听别人的预测
6. 资金管理与图表技术分析，交易系统原则keep it simple
7. 市场如战场，《孙子兵法》少不了
8. 对已经成熟的交易策略不过度管理
## 3.13
《毛选》

这种态度，就是实事求是的态度。“实事”就是客观存在着的一切事物，“是”就是客观事物的内部联系，即规律性，“求”就是我们去研究。

## 3.01
看到前端的层次问题，感觉还挺有道理：

1. 纯表现层。用户体验、布局、特效、研究 CSS 各种奇技淫巧（例子：CodePen 上各种无比酷炫但基本靠 hard-code 搞出来的特效）；对于很多设计/前端兼修的人来说，技术层面就到此为止了。他们很多可能一辈子都不会写翻转二叉树，但他们也能搞出一些科班出生的人一辈子也搞不出的用户体验。当然不排除一些走 creative coding / 数据可视化路线的人需要对物理、数学、甚至计算机图形方面的知识进行针对性的强化。
2. 应用实现层。可能是大公司初级工程师主要干的活：拿着别人设计好的框架、工具去实现具体的应用逻辑。实话实说这个层面对计算机基础的要求确实不高，只要对 JS、CSS 这些领域专门的东西基础扎实 + 学习能力 ok 就可以了。但是这个层面其实需求巨大，而且有一个独特的需求：开发效率。要提升效率就得对手上的工具了解得非常细致，比如 XX 框架的 N 种优化小窍门之类的... 而这种东西只能靠实战经验去积累，基础再扎实影响也有限。
3. 应用架构层。技术选型、开发底层框架、制定开发规范、设计应用结构... 这些东西就涉及到知识的广度和深度了，对业务需求的理解很重要，而且碰到具体的纯技术问题的可能性也大得多。编译原理、算法、数据结构在这里都会派上实际的用处。
4. 基础设施层。自动化构建、部署、测试、加载方案、性能优化、代码质量管理等等... 这一层更加技术化了，而且涉及很多所有软件工程共通的东西，并不局限于前端。
5. 理念层。通过借鉴整个计算机体系中其他领域的思想，从根本上改进前端的开发范式。Facebook 的人现在做的就是这种事情。事实上能做到这一层的人基本不以前端自居了。


## 2.12
事的价值=对社会的价值=受益人数 x 人均时间 x 单位时间价值差

## 1.18
姿势跑法的技术要领
①要通过自由落下将臀部（身体重心）前移到身体支撑点（脚的跖球部）上方。

②身体成关键跑姿时，保持肩部、髋关节和踝关节处于姿势跑法的平衡位置上。

③要始终保持膝关节的弯曲，不要完全伸直。

④要将体重集中在支撑脚的跖球部。

⑤双腿转换支撑的过程要迅速。

⑥在上拉时，要将脚踝直接从地面拉到臀部下方。

⑦支撑时间要尽可能短。

⑧要利用重力作用，而不是肌肉的力量，不要用脚推蹬、抬膝或用大腿的股四头肌来驱动身体向前。

⑨不要用脚跟着地，在支撑过程中，脚跟与地面之间也只是轻轻接触，不要将体重落于脚跟。

⑩落下动作起始于支撑脚脚跟开始离开地面时。

⑪落下动作结束于摆动脚通过支撑腿的膝盖时。

⑫不要试图通过加大下肢动作幅度来加快跑步速度。

⑬不应将注意力集中在落地动作上，应该关注上拉动作。

⑭落下的过程中，腿部的肌肉应该完全不使力，让它自由落下。

⑮脚踝始终要处于自然放松的状态。

⑯摆臂的目的是为腿部动作提供平衡

## 1.16
如何进行阅读

- 区分阅读，对于经典书籍，要进行深度阅读，对于一般文章，可以进行浏览，只提取关键信息
- 提取观点，对于书籍的核心观点，要进行标记，并进行复习。同时对于写作也要学习作者是如何将他的观点灌输给你的。其次最好是带着问题去阅读一些书籍，在读完书后可以回答自己的问题。就是有收获的。
- 联系。看书最好一次看多本同领域，对其中的知识进行相关联，结网，组成知识体系。另外也可以与之和自己最近读过的书，持有的体验或者感悟，正在发生的事情进行联系。
- 随时记录。对于记录要进行分类

阅读 分为 主干 枝干 树叶 其中主干应该由经典的书籍组成，而枝干则可以是论文，严谨的课程，等组成。树叶则是由细碎的东西如抖音，公众号组成

