> 泛型编程是算法导向的，即以算法为起点和中心点，逐渐将其所涉及的概念内涵模糊化、外延扩大化，将其所涉及的运算抽象化、一般化，从而扩展算法的适用范围。

> 首先，基本类型如int、float等不是Object的子类，虽然Java新增了自动装拆箱（autoboxing/unboxing）的功能，但要付出性能的代价。更重要的是，这将不可避免地需要类型的显式转换（explicit conversion或cast），无法在编译期间施行严格的类型检查，由此丧失了静态类型语言的优势，为bug大开方便之门。

> 冒号讲述道，“算法串联数据，如脊贯肉；数据实化算法，如肉附脊。只有抽象出表面的数据，算法的脊梁才能显现。

> 准确地说，抽象是前提，分解是方式，模块化是结果。

> 从软件重用的角度看，可以这么理解AOP与OOP的关系：OOP只能沿着继承树的纵向方向重用，而AOP则弥补了OOP的不足，可以在横向方向重用。这算是回答了引号开始提出的问题：AOP不是OOP的分支，也不能说是超越了OOP，而是OOP的一种补充——尽管AOP并不局限于OOP语言。

> 如果一个程序是一个管道系统，AOP就是在管道上钻一些孔，在每个孔中注入新的代码流。因此AOP实现的关键是将advice的代码嵌入到主体程序之中，术语称编织（weaving）。这是很自然的——将问题分解之后再合成，问题才得以还原。

> 一些设计模式（如装饰模式、职责链模式、状态模式、访问者模式等）就是为了赋予静态语言一定的动态特征。

> 为了达到抽象的目的，实现级别的信息需要隐藏，靠的是访问控制；设计级别的信息需要过滤，靠的是抽象建模。


> 命令式编程是行动导向的，因而算法是显性而目标是隐性的；声明式编程是目标驱动的，因而目标是显性而算法是隐性的。

> 声明式编程重目标、轻过程，专注问题的分析和表达而不致陷入算法的迷宫，其代码也更加简洁清晰、易于修改和维护。


> 归根结底，编程是寻求一种机制，将制定的输入转化为指定的输出。


>  封装使得公民拥有个体身份，继承使得公民拥有家庭身份，多态使得公民拥有社会身份。

> “我猜你的意思是：在定义一个线程之前，其主函数已经模块化了，不能把功劳记在并发式编程上，对吧？”冒号笑问，“你不能孤立静止地看待每个模块，还要考虑到模块之间的相互关联和作用。相比串行式，并发式在模块之间引入了新的通信和控制方式。也就是说，原先的一些模块的定义和划分一定是建立在线程机制的基础上的。如果失去线程的支持，它们的合理性自然会打上问号，说不定整体设计都会受到牵连。这也体现了编程范式的渗透性和全局影响力。

> OOP只能沿着继承树的纵向方向重用，而AOP则弥补了OOP的不足，可以在横向方向重用。


> 举个简单的例子，计算两个函数的乘积：f（x）*g（y）。由于无副作用，f（x）和g（y）的估值过程是独立的，估值顺序也不重要，因此理论上可以对二者并行计算。另外，还可利用惰性求值（lazy evaluation）：如果算出f（x）为零，那么不用计算g（y）便可知乘积为零了。”


> “Duck类型的哲学是：**名义不重要，重要的是能力，颇有些实用主义的味道**。这种非继承性多态为软件重用开启了新的窗口，同时也埋下了一些陷阱。由于Duck类型的接口组合是隐性的，其使用者须要比普通interface更小心，以避免误用；其维护者也须要更小心，以避免破坏客户代码；另外它也可能造成滥用——将一个会叫会游的家伙放进池塘看起来不算坏主意，但如果一艘轮船趁机也轰隆隆地开了进来，事情恐怕就不那么美妙了。

 > 两种类型的体制可以用两种法律原则来类比：静态类型检查类似‘疑罪从有’的有罪推定制——在被证明合法之前是非法的，动态类型检查类似‘疑罪从无’的无罪推定制——在被证明非法之前是合法的。至于如何取舍，套用一句话：‘Static Typing Where Possible, Dynamic Typing When Needed’。不妨理解为：尽可能守规则，必要时求变通。


>  类型的动静以类型的绑定时间来划分，类型的强弱以类型的**约束强度**来划分，它们之间没有必然联系。弱类型语言允许类型的隐性转化，被认为是类型不安全的；而强类型语言则一般不允许这种转化，被认为是类型安全的。

> 在我看来，**抽象思维能力是最重要的**。当然，不独计算机领域，其他科学领域乃至艺术领域同样需要这种能力。更广泛地说，抽象是人类认识和描绘世界最首要的工具。”不知不觉冒号又走上了形而上的路线。


> 实现继承最大的硬伤是在类族之间建立了**强耦合关系**，使代码趋于僵硬、脆弱和复杂。

 > “作为一个抽象数据类型的类，其核心是抽象接口，因此首先应该设计公共接口，它们的修饰符自然都是public。如果该类是一个抽象类（abstract class），那么可能会有一些为其子类提供的服务，它们的修饰符自然该是protected。”
 
 这里吧接口问题说清楚了。为什么要成为public ，为什么一开始就要去设计接口。
  