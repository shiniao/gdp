# GDP

go design pattern，学习设计模式。

## SOLID设计原则

1. [开闭原则](solid/scm.go)
2. [单一职责原则](solid/srp.go)
3. [依赖倒置原则](solid/dip.go)
4. [接口隔离原则](solid/isp.go)
5. [里氏替换原则](solid/lsp.go)
6. [迪米特原则](solid/lod.go)

## 设计模式

### 创建型模式
创建型模式的主要关注点是“怎样创建对象？”，它的主要特点是**将对象的创建与使用分离**。
这样可以降低系统的耦合度，使用者不需要关注对象的创建细节，对象的创建由相关的工厂来完成。

- [单例模式](design_pattern/singleton.go)

  单例模式说的是系统中的某个资源只能出现一个实例。
  
- [简单工厂模式](design_pattern/simple_factory.go)

  简单工厂模式说的是应该用一个专门的类或者方法来产生其他的类。
  
- [建造者模式](design_pattern/builder.go)

  建造者模式说的是将一个复杂对象的构造与它的表示分离，
  使同样的构建过程可以创建不同的表示。比如汽车厂生成车子，
  汽车的组装过程是一样的，但是零件可以不同。
  
- [原型模式](design_pattern/prototype.go)
  
  原型模式说的是对象的复用，面向接口编程时，不需要知道该对象内部，但是可以生成新的对象实例。

### 结构型模式
- [代理模式](design_pattern/proxy.go)
  
  代理模式说的是使用一个中介（代理）达到访问原对象的目的，因为原对象可能不适合直接访问。
  或者通过代理模式延迟对原对象的操作。
  
- [适配器模式](design_pattern/adapter.go)
  
  适配器模式说的是将一个类的接口转换成客户希望的另外一个接口，
  使得原本由于接口不兼容而不能一起工作的那些类能一起工作。
  
- [桥接模式](design_pattern/bridge.go)

  桥接模式说的是将抽象和实现分离，使得各个实现之间可以相互组合。
  比如图形的形状和颜色，形状有圆形和方形，颜色有红色和黑色，使用桥接模式，
  达到形状和颜色之间的任意组合。
  
- [装饰模式](design_pattern/decorator.go)

  装饰模式说的是在不改变现有对象结构的情况下，
  动态地给该对象增加一些职责（即增加其额外功能）。

- [外观模式](design_pattern/facade.go)
  
  外观模式说的是一种通过为多个复杂子系统提供一个一致的接口，
  而使这些子系统更加容易被访问的模式。
  外观模式将多个子模块组合在一起，通过统一的接口将子模块的功能提供给外界。