# 核心方法

基础方法为排除法，数学特性法和方程法；

提高方法为：赋值法和线段法

## 代入排除法

基本的解题思路是，根据题干，判断题型。根据题型选择解题方法。

### 适用范围

- 选项信息充分：
  - 题干中的变量=选项中的变量
  - 选项为一组数、可转化为一组数
  - 题目中含关键字：
    - 分别是
    - 各是
    - ...和...之比是

  - 复杂题目：人多、数少、关系乱或者方程复杂（排队题etc）

### 常用题型

年龄、不定方程和复杂方程比较常用

- **年龄问题**
  - A的年龄大B.……，求A、B年龄
- **不定方程问题**
  - 变量数量 > 方程数
- **复杂方程问题**
  - 首先列出方程，然后再依次代入验证条件
- 多位数问题
  - 题干的变量是三位数以上，且对该变量给出条件
- 和差倍比问题
  - $$\frac{x+n}{y}=\frac{a}{b}$$，求x或y

### 具体用法

使用排除法，或者代入法，或者两者结合解题

- 排除选项法，把选项和题干信息对比时，可以从以下角度考虑
  - 尾数：[容斥原理问题](section2.md#容斥原理问题)用的多
  - [奇偶](#奇偶特性)：[不定方程组](#不定方程组)
  - [倍数](#倍数特性)：用的最多
  - 大小：倍差关系，已知答案的位数，计算选项时，先判断位数；

- 代入法，把选项代入方程式时，代入顺序可以从以下角度考虑
  - 题干条件：优先选择简单的条件验证，比如和差关系比倍数关系好考虑
  - 最值问法：如果题目问最大，先从最大的选项开始
  - 代入方向：

> 【例 1】(2018 江西)一家三口，妈妈比儿子大 26 岁，爸爸比儿子大 33 岁。1995 年，一家三口的年龄之和为 62。那么，2018 年儿子、妈妈和爸爸的年龄分 别是:
>
> A.23，51，57 B.24，50，57
> C.25，51，57 D.26，52，58

解析：年龄问题，代入法或者方程法，先使用简单的题干条件，爸爸比儿子大33岁，排除掉ACD项，选B

> 【例 2】(2019 北京)某工厂有甲、乙、丙 3 条生产线，每小时均生产整数 件产品。其中甲生产线的效率是乙生产线的 3 倍，且每小时比丙生产线多生产 9件产品。已知 3 条生产线每小时生产的产品之和不到 100 件且为质数，则乙生产 线每小时最多可能生产多少件产品?
>
> A.14 B.12
> C.11 D.8

解析：工程问题，使用方程法，又是不定方程组，考虑代入法，题目是最值问法，最大从14开始，代入4得89，89不能被2整除，也不能被3，5，7，9整除，因此是质数，符合条件，选A

⚠️ 质数是只能被1和本身除的数，要想验证n是质数，查看n是否能被$$\sqrt{n}$$以内的数整除，如果能，则不是质数。

> 【例 3】 (2016 广东)大型体育竞赛开幕式需要列队，共 10 排。导演安排演 员总数的一半多一个在第一排，安排剩下演员人数的一半多一个在第 2 排......依 次类推。如果在第 10 排恰好将演员排完，那么参与排队列的演员共有多少名?
>
> A.2000 B.2008
> C.2012 D.2046

解析：可以使用方程法解决，但是方程过于复杂，使用代入法，设总共有x人则$$\frac{\frac{x}{2}-1}{2}$$	为整数，选D

## 数学特性法

主要有奇偶和倍数两个特性，当计算均为整数时，需要考虑

### 奇偶特性

- 适用范围
  - **不定方程问题**：比如3x+4y=25，则x必为奇数	；
  - 知和求差、知差求和：答案是求差或求和，找题目中是否有和\差，从而判断答案的奇偶特性
  - 2倍、平均、相等、偶数

- 具体用法
  - 和差（只适用于两位数）
    - 同奇同偶才为偶
    - 一奇一偶则为奇
  - 乘积
    - 一个为偶则为偶
    - 全部为奇才为奇

### 倍数特性

- 适用范围
  - “（百）分数”，“倍数”，“比例”，“分担”

- 具体用法
  - 整数型：$$X=a\times b$$，则X能被a或b整除
    - 若 $$a=m\times n$$，且m和n没有公约数，则X能被a整除 
    - 若X能被a和b同时除，则能被$$a\times b$$同时除
    - 用于不定式，7x+3y=60，则x一定能被3整除
  - 余数型：若$$y=ax+b$$，则$$(y-b)$$能够被$$a$$整除
- 比例型：$$\frac{a}{b}=\frac{m}{n}$$，m、n互质[^1]
    - a、b分别是m、n的背书
    - $$a\pm b$$是$$m\pm n$$的背书
    - 出现形式有$$\frac{m}{n}$$，a%，m:n，a倍

> 【例 1】 (2017 福建)如图，一个正方体的表面上分别写着连续的 6 个整数， 且每两个相对面上的两个数的和都相等，则这 6 个整数的和为:
>
> ![page7image13025488.png](assets/section1/page7image13025488.png) 
>
> A.53 B.52
> C.51 D.50

解析：未知数数量=方程数量，为常规方程组，但解起来比较麻烦，选项也无法使用代入法，发现结果和3有倍数关系，只有C可以被整除，选C

> 【例 2】(2017 江西)某公司研发出了一款新产品，当每件新产品的售价为3000 元时，恰好能售出 15 万件。若新产品的售价每增加 200 元时，就要少售出1 万件。如果该公司仅售出 12 万件新产品，那么该公司新产品的销售总额为:
>
> A.4.72 亿元 B.4.46 亿元
> C.4.64 亿元 D.4.32 亿元

解析：常规方程组，同时发现答案和12有倍数关系，12=3*4，能被3整除的只有D，选D

> 【例 1】(2016 深圳)两箱同样多的蛋黄派分别分发给两队志愿者做早餐， 分给甲队每人 6 块缺 8 块，分给乙队每人 7 块剩 6 块，已知甲队比乙队多 6 人， 则一箱蛋黄派有多少块?
>
> A.120 B.160
> C.180 D.240

解析：常规方程组，同时发现答案+8与6有倍数关系，6=3*2，+8后能被3整除的只有B。

> 【例 2】(2015 江苏 A)一群大学生进行分组活动，要求每组人数相同，若 每组 22 人，则多出一人未被分进组;若少分一组，则恰好每组人数一样多。已 知每组人数最多只能 32 人，则该群学生总人数是:
>
> A.441 C.536
>
> B.529 D.528

解析：常规方程组。同时发现答案-1与22=2*11有倍数关系，只有A和B符合选项，考虑代入法，发现441不能被19整除，因此选B

> 【例 3】(2018 陕西)苗苗有一堆草莓，乐乐也有一堆草莓。苗苗的草莓五 个五个地数，最后剩两个，七个七个地数，最后还是剩两个;乐乐的草莓五个五 个地数，最后剩四个，六个六个地数，最后剩三个。已知苗苗比乐乐多 8 个草莓， 则苗苗的草莓数为:
>
> A.37 B.62
> C.72 D.77
> E.87 F.92
> G.102 H.107

解析：方程法，应该是常规的。考虑倍数特性，被5和7除，都余下2，说明能被35除，将剩下的选项代入，选H

> 【例 1】 (2017 吉林)古希腊数学家丢番图(Diophantus)的墓志铭:过路 人，这儿埋葬着丢番图，他生命的六分之一是童年;再过了一生的十二分之一后，他开始长胡须，又过了一生的七分之一后他结了婚;婚后五年他有了儿子，但可 惜儿子的寿命只有父亲的一半，儿子死后，老人再活了四年就结束了余生。根据 这个墓志铭，丢番图的寿命为:
>
> A.60 B.84
> C.77 D.63

解析：方程法。以分数形式提到比例，考虑倍数特性，能被6、12、7整除，说明能被84整除，选B

> 【例 2】(2019 广东选调)某单位购买了 30 个文件袋，有大、中、小三个型 号。已知大号文件袋和中号文件袋数量之比为 5:6，中号文件袋和小号文件袋 数量之比为 3:2。那么，所购的小号文件袋有多少个?
>
> A.4 B.6
> C.8 D.10

解析：方程法，设份数为x，则一共有5+6+4=15份，解x=2，则小号文件有8份，选C

> 【例 3】 (2015 北京)甲、乙两个班各有 40 多名学生，男女生比例甲班为 5:6，乙班为 5:4。则这两个班的男生人数之和比女生人数之和:
>
> A.多 1 人 B.多 2 人
> C.少 1 人 D.少 2 人

解析：不定方程，赋值法，总数在[41,49]的区间范围内，甲班有44人，乙班有45人，选A

> 【例 4】(2018 山东)某企业有不到 100 名员工，本月只有 1/12 的员工未得 到每人 1000 元的全勤奖，只有 13 名员工未得到每人 1000 元的绩效奖，两个奖 都未得到的员工占员工总数的 1/14。问企业本月共发放全勤奖和绩效奖多少万 元?
>
> A.7.1 B.12.6
> C.14.8 D.16.8

解析：不定方程，赋值法。员工人数<100，且能被12和14整除，员工人数为84，$$\frac{11}{12}\times 84\times 1000+(84-13)\times 1000=148000$$

- 判定法则
  - 口诀
    - 3/9只看各位数字之和：某个数能被3/9整除，则其各位数字的和能被3/9整除
    - 2/4/8；5/25/125只看末两/三位数
  - 因式分解
    - 判断能否被$$A\times B$$整除，只需判断是否能同时被$$A$$和$$B$$整除
    - $$A$$和$$B$$必须互质

## 方程法（重要）

方程分为两类，一是常规方程组，二是不定方程组。常规方程组又分为一元和二元。根据变量是否为整数，不定方程组又分为限定的和不限定的。

### 常规方程组

- 适用范围
  - 存在明显等量关系
    - 提到”共有……“，”多/少……“等字眼
    - 经典问题中的公式，如等

- 常用题型
  - 和差倍比
  - 浓度
  - 牛吃草
  - 利润
  - 行程
  - 工程
- 具体用法
  1. 设未知数
     1. 设最小数，A是B的3倍，设B
     2. 设中间数，A在题目中出现1次，B出现3次，设B
     3. 问谁设谁
  2. 把其他未知量用未知数表示
  3. 利用等量关系，列方程（组）求解

> 【例】(2018 四川)甲和丙的年龄和是乙的 2 倍，今年甲的年龄是丙的 3 倍，9 年后甲的年龄是丙的 2.4 倍，则多少年后丙的年龄是乙的 4/7?
>
> A.7 B.9
> C.12 D.14

解析：年龄问题，考虑代入法，但本题未知量多，选择传统的方程法。由于丙的出现次数最多，设丙为x，则甲为3x，乙未2x。$$(3x+9)=2.4\times (x+9)$$，解得x=21，再根据问什么设什么，列出方程$$(21+y)=(42+x)\times \frac{4}{7}$$，使用倍数特性中的余数法，选A

### 不定方程组

*适用范围*

- 未知数个数多于方程个数

*常用题型*

- 和差倍比
- 利润

*具体用法*

- 限定性不定方程
  - [奇偶](#奇偶特性)
  - [倍数](#倍数特性)
  - 尾数
    - 5的倍数，尾数只能为0（偶数），5（偶数）
    - 比如37x+20y=271，x只能以3结尾
- 非限定性不定方程
  - 多项式的整体代换
  - 赋零法：尽量取两式都有的量为0

> 【例 1】(2015 联考)每年三月某单位都要组织员工去 A、B 两地参加植树活 动，已知去 A 地每人往返车费 20 元，人均植树 5 棵，去 B 地每人往返车费 30元，人均植树 3 棵，设到 A 地有员工 x 人，A、B 两地共植树 y 棵，y 与 x 之间满 足 y=8x-15，若往返车费总和不超过 3000 元时，那么，最多可植树多少棵?
>
> A.498 B.400
> C.489 D.500

解析：方程法，题目中已经给出答案的方程，先考虑奇偶，奇偶相加为奇，因此为C

> 【例 2】(2017 江苏)小王打靶共用了 10 发子弹，全部命中，都在 10 环、8环和 5 环上，总成绩为 75 环，则命中 10 环的子弹数是:
>
> A.1 发 B.2 发
>
> C.3 发 D.4 发

解析：不定方程，$$10x+8y+5z=75$$，首先考虑奇偶，z一定为奇数，奇数与5相乘，尾数为5，考虑尾数法，x尾数为0，则y的尾数为0，则10x + 5z = 35，x+z=5，使用代入法，x=2，y=3，选B

> 【例 3】(2018 四川)某企业采购 A 类、B 类和 C 类设备各若干台，21 台设 备共用 48 万元。已知 A、B、C 类设备的单价分别为 1.2 万元、2 万元和 2.4 万 元。问该企业最多可能采购了多少台 C 类设备?
>
> A.16 B.17
> C.18 D.19

解析：不定方程，$$x+y+z=21$$，$$3x+5y+6z=100$$，先考虑奇偶特性，排除AC，再用代入法排除D，选B

> 【例 4】(2018 上海)现有甲、乙、丙三种货物，若购买甲 1 件、乙 3 件、 丙 7 件共需 200 元;若购买甲 2 件、乙 5 件、丙 11 件共需 350 元。则购买甲、 乙、丙各 1 件共需多少元?
>
> A.50 B.100
> C.150 D.200

解析：不定方程，x+3y+7z=200，2x+5y+11z=350，x、y和z有多个解，但答案提示存在恒等关系，考虑赋值法，将最复杂的的z设为0，解得x和y都为50元，选B

> 练习三(2016 国考)20 人乘飞机从甲市前往乙市，总费用为 27000 元。每 张机票的全价票单价为 2000 元，除全价票之外，该班飞机还有九折票和五折票 两种选择。每位旅客的机票总费用除机票价格之外，还包括 170 元的税费。则购 买九折票的乘客与购买全价票的乘客人数相比为( )。
>
> A.两者一样多 B.买九折票的多 1 人
> C.买全价票的多 2 人 D.买九折票的多 4 人

解析：不定方程，$$x+y+z=20$$，$$20x+18y+10z+34=270$$，先消元，得$$10x+6y=36$$，x+y奇偶无法判断，考虑尾数法，10x尾数为0，则6y尾数为6，y=1，x=2，选A

## 赋值法

### 适用范围

- 题干中没有出现具体的值
- 在$$A=B\times C$$这样的三量关系中，至多给出其中一个量的具体值

### 常用题型

- [工程问题](section2.md)

- 行程问题

- 经济利润问题

- 浓度问题

### 具体用法

1. 对题目中的不变量赋值（即所有公式都会出现的变量）
2. 根据所给数字赋值公倍数（总量赋值一般用公倍数）
   - 比如已知$$a\times b = c$$，题目中给出了符合这个条件的两个公式，那么要根据a\b对应的两个值，取公倍数
   - 如果一个量都没给出，可以赋值两次
3. 根据所给比例关系赋值（见[常规方程组](#常规方程组)中设中间数为未知数）
4. 赋值尽量便于计算和简化

## 线段法

### 适用范围

*混合比例问题*

- 混合：两个或多个部分组成一个整体
- 比例：计算公式位两个量相除的形式

### 常用题型

- 浓度混合
- 平均数混合
- 利润率混合
- 折扣混合
- 比例混合
- 增长率混合

### 具体用法

1. 混合之前写两端，混合之后写中间
2. 距离和量成反比，份数计算不能反

### 注意事项

- 混合浓度，对应溶液量之比
- 混合平均数，对应人数之比
- 混合利润率，对应成本之比
- 混合折扣，对应定价之比
- 混合比重，对应总体之比
- 混合增长率，对应基期量之比



[^1]:互质，两个数之间没有公约数。2和3互质，2和6不互质