# 数据科学攻略

数据科学主要以统计学,机器学习,数据可视化以及领域知识为理论基础,其主要研究内容包括数据科学基础理论,数据预处理,数据计算和数据管理等.是一门很杂的交叉学科.需要同时具备计算机,数学,统计作为前置知识,因此还是算比较高阶的学问.

数据科学总的来说和机器学习一样,是应用统计学的一个细分学科,这两个学科要时常有交叉应用.总的来说数据科学更加偏向工程,机器学习则更加偏向研究.

## 数据科学研究的对象和要解决的问题

数据科学研究的对象是数据,数据则是人工从事物中提取出来存在[信息空间]()中的对象.万事万物只要不是静止不变的就必然会留下信息,而这个宇宙唯一不变的只有变化,因此数据科学的研究对象可以是任何事物;但这么说又不准确,更准确的说法是研究的是任何事物留下信息的数据.

那么数据科学要解决的问题就包括了:

1. 如何将事物信息提取为数据
2. 如何将数据保存在信息空间
3. 如何利用保存在信息空间的数据解决实际问题.


## 目标读者

这篇文章主要的目标读者是有一定计算机和统计基础,希望对数据科学有所了解的工程和研究人员.本文也相对更加偏向工程,理论的部分更多的是在术语表中以词条的形式做介绍.

## 非目标读者

+ 新手慎入,这个坑很大,如果纯新人建议先看我的[python攻略](http://blog.hszofficial.site/TutorialForPython/),有一定python编程基础后再入坑.
+ Java程序员慎入,本人不喜欢Java,因此相关技术栈将鲜有涉及,主要介绍的技术是围绕python展开的,因此上面才会建议新人看python攻略.希望通过本文学习`hadoop/spark`技术栈的人恐怕要失望了.


## 本教程的内容范围和组织结构

文章的目标是做成数据科学领域最佳实践的形式,由于本人不喜欢java,因此java技术栈的内容将鲜有涉及,由于数据科学是一门相当杂的学科,因此文章内容也会看起来比较杂乱.我会尽量让各个部分的内容相对独立,如果一定要有联系也会使用超链接做关联,这样以提高可读性.

文章将会划分为篇,每一篇下面的单位是章,章下面是节,篇下面可以没有章,这种情况就顺延.篇,章下面都会开头的介绍文字和结尾的结语.介绍用于总体上概括其所属的内容而结语用于介绍一些豆知识,相关的好用第三方库和个人的相关看法,希望读者喜欢.
每一节则是单独的一篇文章.我尽量让各个部分内聚避免耦合,这样可以不用按顺序,但有些确实需要有其他方面基础的那就没办法了,我会在每节开始的部分给出预备知识的超链接方便查看.

每一节中都会有1~3级标题,不会再往下分出4级标题.同时1级标题只会是一节的标题.

总结下就是如下的树状结构

```shell
篇-|
   |-章-|
        |-节-|
             |- 1级标题-|
                       |-2级标题-|
                                |-3级标题
```

或者

```shell
篇--|
    |-节-|
            |- 1级标题-|
                    |-2级标题-|
                            |-3级标题
```

在文末会有一个术语表附录,将文中出现的术语做一个总结,如果有的话也会给出wiki链接

下面是每篇的简单介绍

+ 工具链篇

    介绍数据科学领域常见的各种工具.比如python的数据科学工具箱,数据库,消息中间件,搜索引擎等.

+ 数据采集篇

    介绍从什么地方以什么形式采集数据

+ 数据清洗篇

    介绍如何过滤数据中的噪音,调整由于采集操作造成的误差,使其可以更好更准确的描绘对象的信息

+ 数据管理篇

    介绍如何将采集来,清洗好的数据保存在信息空间以便于使用和复现模拟.

+ 数据分析篇

    介绍如何分析各种数据,找到其特点用于辅助决策

+ 数据挖掘篇

    介绍如何使用探索数据以发现其更多的价值

+ 数据预测篇

    介绍如何利用机器学习等算法技术构造模型,用于预测数据的一些位置特点


## 贯穿全文的排版约定

### 难度分级

这边给出的分级方案是相对分级,具体说就是在篇/章/节/中1~3级标题中命名以`*`为开头,为标题的就是相对其他同级的来说进阶一些的内容,这些内容可以选择着看;而使用`**`开头的的则是相对最基础最重点的内容.需要加深记忆

篇/章/的标题在每个篇/章的介绍页,


### ps

一些比较关键的点会使用***加粗斜体的PS:字样***标识出来
