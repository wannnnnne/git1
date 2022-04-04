# day10

## 继承

1. 格式：
   class 子类 extends 父类   

2. 重名时：super.父类成员变量名  

3. public abstract class Animal {  //抽象类

   public abstract void run()；//抽象方法
   }  

4. 注意事项：

   抽象类**不能创建对象**，如果创建，编译无法通过而报错。只能创建其非抽象子类的对象。  

   抽象类的子类，必须重写抽象父类中**所有的**抽象方法，否则，编译无法通过而报错。除非该子类也是抽象类。  

   

