# 状态模式（State Pattern）

> Allow an object to alter its behavior when its internal state changes. The object will appear to change its class.

> 当一个对象内在状态改变时允许其改变行为，这个对象看起来像改变了其类。

![state-pattern](../res/images/state-pattern.svg)

* State抽象状态角色

    接口或抽象类，负责对象状态定义，并且封装环境角色以实现状态切换。

* ConcreteState具体状态角色

    每一个具体状态必须完成两个职责：本状态的行为管理以及趋向状态处理，通俗的说，就是本状态下要做的事情，以及本状态如何过渡到其他状态。

* Context环境角色

    定义客户端需要的接口，并且负责具体状态的切换。

## 状态模式的优点

* 结构清晰

    避免了过多的`switch...case`或者`if...else`语句的使用，避免了程序的复杂性，提高了系统的可维护性。

* 遵循设计原则

    很好地体现了开闭原则和单一职责原则，每个状态都是一个子类，需要添加状态时只需要增加子类，需要修改状态只需要修改子类。

* 封装性非常好

    这也是状态模式的基本要求，状态变换放置到类的内部实现，外部的调用不需要知道类内部如何实现。

## 状态模式的缺点

只有一个缺点，那就是子类太多，状态过多，容易造成类膨胀。

## 状态模式的使用场景

* 行为随状态而改变的场景

* 条件、分支判断语句的替代者