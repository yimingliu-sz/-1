 

#                 Stack Overflow 用户画像分析   

![1553132482697](C:\Users\ADMINI~1\AppData\Local\Temp\1553132482697.png)

## 项目介绍                                                                               

本次项目的灵感来自于互联网，Stack Overflow 每年都会对其用户进行线上调研，从2011至2018，已持续了8 年。

Stack Overflow2018年度开发者调查是针对183个国家和地区，获得了超过100,000个用户的回复，是对软件开发人员进行的最全面的调研，调研了开发人员从职业满意度、求职到教育、编码偏好各个方面的经验。

## 项目目的                                                                                 

本次项目主要利用Stack Overflow2018年近10万——98855个用户调研数据，以实现Stack Overflow的用户画像分

析。Stack Overflow（简称Stack）想利用用户画像来吸引广告商的注意，以及投放广告以获得推广效果，目前需解决以下问题：

- **什么类型的广告适合投放在Stack？**

- **Stack在什么类型的平台发布广告可以使自己的推广效果达到最大呢？**

****

## 项目分析过程                                                                           

***本项目主要用Python进行数据清洗，整合以及数据分析探索，使用Tableau进行数据可视化，使用Typora撰写Markdown数据分析报告。*

Stack此次的用户调研一共涉及128个问题，相当于128个特征，其中部分特征对项目的分析目的没有针对性，因此首先对特征进行筛选。

### 1.来自什么国家？                                                                                     

**共98443个受访者回答*

Stack的用户分布于全世界的183个国家。从世界范围来看，美国在Stack的用户数最多且占比超过20%，由于美国的计算机技术占领先地位，用户排名第一也是在合理的解释范围。其中印度的IT行业也是非常发达，其用户数在是 stcak排名第二，且是第三的德国人数的2倍。中国排名17，如果没有网络安全的限制，中国的排名应该更高。

可以看出，Stack 的用户主要分布在北美，印度，欧洲等IT技术较发达的国家。

![1553131404104](C:\Users\ADMINI~1\AppData\Local\Temp\1553131404104.png)



### 2.写代码是否是用户的兴趣？是否对开源项目做过贡献？                              

**均有98855个回答*

Stack的用户中大部分以写代码为兴趣，说明他们平时对IT领域的信息会比较关注。

Stack的用户中有43.6%的用户为代码开源做过贡献，这部分用户的技术能力相对较强，开源代码的门槛相对较高。

![1553131433734](C:\Users\ADMINI~1\AppData\Local\Temp\1553131433734.png)

​                 ![1553131442111](C:\Users\ADMINI~1\AppData\Local\Temp\1553131442111.png)



### 3.用户的性别，年龄以及编程年龄分布                                                        

**共64469个回答*

Stack的用户男性占92.2%，女性仅占6.2%，说明对代码关心的男性远多于女性。

![1553131513113](C:\Users\ADMINI~1\AppData\Local\Temp\1553131513113.png)

**共64574个回答*

用户年龄主要集中在25-30岁，以青年为主要力量。

![1553131524553](C:\Users\ADMINI~1\AppData\Local\Temp\1553131524553.png)

**共93835个回答*

用户编码年龄主要集中在3-5年，有一定的经验，仍需学习阶段。

![1553131535596](C:\Users\ADMINI~1\AppData\Local\Temp\1553131535596.png)

**共77903个回答*

用户以编码为职业的时间集中在0-2年，3-5年这两个阶段，说明上Stack的用户大多都是刚入行不久，刷Stack的目的主要是提升个人技能。

![1553131549037](C:\Users\ADMINI~1\AppData\Local\Temp\1553131549037.png)

 

### 4.用户的最高学历是怎么样的？                                                                  

**共94703个回答*

Stack用户拥有本科学历的占到46.1%，其次是硕士占到22.59%，而没有接触过正式教育的用户仅占0.74%。整体上看用户的学历普遍在本科及本科以上。

![1553131560271](C:\Users\ADMINI~1\AppData\Local\Temp\1553131560271.png)

### 5.目前的求职状态是什么？是否是学生？                                                     

**共95321个回答*

Stack活跃的用户，74%都是在职员工，其次有9.7%的用户是自由职业者，5.6%的用户是拥有一份兼职，说明有近

90%的用户都有一定经济能力。

![1553131576702](C:\Users\ADMINI~1\AppData\Local\Temp\1553131576702.png) 

**共9401个回答*

有74.2%的用户不是学生，结合求职状态数据可看出有全职工作的用户一般不是学生，但是全职学生或兼职学生的比例达到25.8%。虽然职业人士占Stack用户的大部分，但学生群体亦是一股不小的力量。

![1553131586073](C:\Users\ADMINI~1\AppData\Local\Temp\1553131586073.png)

 

### 6.用户的收入分布                                                                                     

**共46860 个完整回答*

原始的薪资数据是以美元年薪换算（假设一年有50周，12个月），将薪资和薪资类型为NaN值或0值的数据剔除。在工资处理中发现有许多年薪的数据非常大，最大大到200w，通过箱型图看数据分布，发现异常值较多，上极限值为198139.5美元年薪，因此将异常值排除出去再来进行统计，这意味着我可能排除了类似facebook创始人马克· 扎克伯格年薪这样的数据。

![1553131597592](C:\Users\ADMINI~1\AppData\Local\Temp\1553131597592.png)

通过直方图可以看出，用户工资主要集中在3-5万年薪左右，这在美国的个人收入中算中等收入，且有很多年前超过十万的高收入人群，Stack用户有很大一部分工作中会用到编码，也可以推测出他们属于IT行业，而IT行业在美国算是高薪职业。其中0-9907美元年薪收入也占比较大的一部分，这可以用前面提到学生数据解释，有25.8%的用户是学生。

![1553131608365](C:\Users\ADMINI~1\AppData\Local\Temp\1553131608365.png)

整体的平均年薪随编码年龄而增长，与编码相关的工作平均年薪在前20年的变化是比较快的，这也是职业的发展期，而超过20年后，平均年薪趋于稳定。

![1553131619518](C:\Users\ADMINI~1\AppData\Local\Temp\1553131619518.png)

### 7.用户的作息时间（WakeTime）                                                              

**共72146个回答*

用户的作息大部分正常，占比最高的是7：01-8：00 AM 这一时间段，一般公司的上班时间为9：00。

![1553131630005](C:\Users\ADMINI~1\AppData\Local\Temp\1553131630005.png)

### 8.用户一天花多少时间在电脑上                                                                  

**共72133个回答*

如果按上班8小时计，那么上班工作用到电脑的时长在5-8小时，说明不用在非工作时间使用电脑，那么数据表明：只有30.6%的用户属于这一范围。程序员加班文化结合来看，大概有65.9%的程序员需要加班。

![1553131640361](C:\Users\ADMINI~1\AppData\Local\Temp\1553131640361.png)

### 9.用户一天花多少时间在户外及锻炼的频率                                                 

**共72024个回答*

一天所花时间少于39分钟在户外的用户可以说是非常宅了，基本上没事不出门。

而有71.9%的用户在每天会在户外花30分钟-2小时，算上平时的通勤时间，在2小时内还是比较合理的。

![1553131653035](C:\Users\ADMINI~1\AppData\Local\Temp\1553131653035.png)

**共72108个回答*

几乎不运动的用户占了很大一部分，在四种分类中占比也是最高。但是基本上satck用户还是挺注意健康的，62.6% 的用户每周都至少有运动一次。

![1553131661296](C:\Users\ADMINI~1\AppData\Local\Temp\1553131661296.png)

### 10.用户是否有家庭                                                                                   

**共62596个回答*

有家庭的用户占28.9%，而未婚/无家庭的用户占到71.1%，前面也有提到，Stack用户的年龄集中在22-34这一青年阶段，所以未婚/无家庭的占比大也有合理解释。

![img](data:image/png;base64,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) 

## 项目总结                                                                                 

我们从Stack的一些个人基本信息，如：国籍，性别，年龄，学历，收入，家庭，是否职业编程，求职状态，作息时间，使用电脑的时间，在户外的时间及锻炼频率，去描写了一个大体的用户画像。

由数据可以总结出：

- **Stack的用户来自世界范围，从而可以提现出satck是一个国际化平台；**

- **Stack的用户几乎都是年轻男性，很大一部分未婚； satck的用户学历高，收入客观，有一份相关编码的工作；**

- **satck的用户工作时间长，加班普遍，但也非常自律，坚持早起和运动。**

## 项目问题解决方向                                                                     



- **什么类型的广告适合投放在 Stack?**

  从用户画像看出，针对男性的高品质，且不用花费太多时间去选择的产品，比较适合satck的用户，因为他们的收入不错，但时间主要花在工作上。例如可以投放最新的运动产品，数码产品等。

-  **Stack在什么类型的平台发布广告可以使自己的推广效果达到最大呢？**

  可以有针对性地去程序员集中的地方投放推广广告，如程序员论坛，程序员博主等；

  另一方面，大部分人把Stack当做一个提升自我技能及疑问解答的开源网站，那么可以和一些编程培训学校或网站合作，培养未来的中坚力量。

## 反思与致谢                                                                              

- 本数据集一共有128个特征，本次报告只分析了有针对性的15个特征，还有很多特征值得去深挖了解，如可以通过年龄切片成不同的数据集，去多个方面对比，以发现每个年龄层不同的特征及偏好；

- 本分析的结果都只是统计学上的相关性，并不具备因果关系，因果性有待日后更严谨的大样本随机双盲试验得出结果。