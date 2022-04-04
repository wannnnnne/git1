# day09

## String

1.  字符串不变：字符串的值在创建后不能被更改。（下图直接创建了新的字符串）

![image-20211108154600217](C:\Users\灯下黑\AppData\Roaming\Typora\typora-user-images\image-20211108154600217.png)

2. 因为String对象是不可变的，所以它们可以被共享。  

3. 字符串效果相当于是char[]字符数组，但是底层原理是byte[]字符数组。

4. **字符串常量池：程序当中直接写上的双引号字符串，就在字符串常量池中，new出来的不在池中。**

   对于基本类型，==是对于数值的比较。

   对于引用类型，==是对于地址的比较。

5. ![image-20211108160844829](C:\Users\灯下黑\AppData\Roaming\Typora\typora-user-images\image-20211108160844829.png)

6. ![image-20211108165631120](C:\Users\灯下黑\AppData\Roaming\Typora\typora-user-images\image-20211108165631120.png)

7. ```
   String six = nine.replace("shi", "ri");
   String[] FenGe = nine.split("i");
   System.out.println(FenGe);//输出的是地址，字符串常量池地址
   ```

## static

1. 只在类中保存唯一一份，所有本类对象共享同一份。

2. 静态方法不属于对象，而是属于类的。

   如果没有static关键字，那么必须首先创建对象，然后通过对象才能使用它。

   如果有了static关键字，那么不需要创建对象，直接就能通过类名称使用它。

   对于本类中的静态方法，可以省略类名称。

3. 注意事项：

   ①静态方法**不能直接访问**普通成员变量或成员方法。（原因：因为在内存中先有的静态内容，后有的非静态内容）。

   ②静态方法中不能用this关键字。（**静态方法不用对象，而用类**）

4. ![image-20211108200004934](C:\Users\灯下黑\AppData\Roaming\Typora\typora-user-images\image-20211108200004934.png)

5. 静态代码块：随着类的加载而**执行且执行一次**，**优先于main方法和构造方法的执行**。  

   **静态内容总是优先于非静态，所以静态代码块比构造方法先执行。**

   public class ClassName{
   static {
   // 静态代码块的内容
   			}
   }  

6. 静态代码块典型用途：用来一次性地对静态成员变量进行赋值。



