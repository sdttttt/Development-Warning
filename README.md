<h1 align="center">
  软件开发原则
</h1>

### 开闭原则（OCP）

开闭原则（OCP）是面向对象设计中“可复用设计”的基石，是面向对象设计中最重要的原则之一，其它很多的设计原则都是实现开闭原则的一种手段。1988年，勃兰特·梅耶（Bertrand Meyer）在他的著作《面向对象软件构造（Object Oriented Software Construction）》中提出了开闭原则，它的原文是这样：“Software entities should be open for extension,but closed for modification”。翻译过来就是：“软件实体应当对扩展开放，对修改关闭”。这句话说得略微有点专业，我们把它讲得更通俗一点，也就是：软件系统中包含的各种组件，例如模块（Modules）、类（Classes）以及功能（Functions）等等，应该在不修改现有代码的基础上，引入新功能。开闭原则中“开”，是指对于组件功能的扩展是开放的，是允许对其进行功能扩展的；开闭原则中“闭”，是指对于原有代码的修改是封闭的，即不应该修改原有的代码。

### 里氏代换原则（LSP）

里氏代换原则(Liskov Substitution Principle LSP)面向对象设计的基本原则之一。 里氏代换原则中说，任何基类可以出现的地方，子类一定可以出现。 里氏代换原则是对“开-闭”原则的补充。（多态）

### 依赖倒转原则（DIP）

所谓依赖倒置原则（Dependence Inversion Principle）就是要依赖于抽象，不要依赖于具体。简单的说就是要求面向抽象进行编程，不要面向具体进行编程，这样就降低了客户与实现模块间的耦合。面向过程的开发，上层调用下层，上层依赖于下层，当下层剧烈变动时上层也要跟着变动，这就会导致模块的复用性降低而且大大提高了开发的成本。面向对象的开发很好的解决了这个问题，一般情况下抽象的变化概率很小，让用户程序依赖于抽象，实现的细节也依赖于抽象。即使实现细节不断变动，只要抽象不变，客户程序就不需要变化。这大大降低了客户程序与实现细节的耦合度。（面向抽象编程、面向接口编程），父控制子，子不要控制父。依赖倒转也可以叫做控制反转。

### 接口隔离原则（ISP）

使用多个专门的接口比使用单一的总接口要好。一个类对另外一个类的依赖性应当是建立在最小的接口上的。一个接口代表一个角色，不应当将不同的角色都交给一个接口。没有关系的接口合并在一起，形成一个臃肿的大接口，这是对角色和接口的污染。“不应该强迫客户依赖于它们不用的方法。接口属于客户，不属于它所在的类层次结构。”不要强迫客户使用它们不用的方法，如果强迫用户使用它们不使用的方法，那么这些客户就会面临由于这些不使用的方法的改变所带来的改变。

### 合成/聚合复用原则

合成/聚合复用原则(Composite/Aggregate Reuse Principle ,CARP)经常又叫做合成复用原则。合成/聚合复用原则就是在一个新的对象里面使用一些已有的对象，使之成为新对象的一部分；新的对象通过向这些对象的委派达到复用已有功能的目的。它的设计原则是；要尽量使用合成/聚合，尽量不要使用继承。

### 迪米特法则（松耦合）

迪米特法则（Law of Demeter）又叫作最少知道原则（Least Knowledge Principle 简写LKP），就是说一个对象应当对其他对象有尽可能少的了解,不和陌生人说话。英文简写为: LoD迪米特法则可以简单说成：talk only to your immediate friends。 对于OOD来说一个软件实体应当尽可能少的与其他实体发生相互作用。每一个软件单位对其他的单位都只有最少的知识，而且局限于那些与本单位密切相关的软件单位。迪米特法则的初衷在于降低类之间的耦合。由于每个类尽量减少对其他类的依赖，因此，很容易使得系统的功能模块功能独立，相互之间不存在（或很少有）依赖关系.
