# 单一职责原则

单一职责原则（SRP：Single Responsibility Principle）：不要存在多于一个导致类变更的原因。通俗的说，即一个类只负责一项职责。

遵循单一职责原的优点：

* 可以降低类的复杂度，一个类只负责一项职责，其逻辑肯定要比负责多项职责简单的多；
* 提高类的可读性，提高系统的可维护性；
* 变更引起的风险降低，变更是必然的，如果单一职责原则遵守的好，当修改一个功能时，可以显著降低对其他功能的影响。

需要说明的一点是单一职责原则不只是面向对象编程思想所特有的，只要是模块化的程序设计，都适用单一职责原则。
