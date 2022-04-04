# day06

## boolean

三种方法：

![image-20211017162207903](C:\Users\灯下黑\AppData\Roaming\Typora\typora-user-images\image-20211017162207903.png)



## 数组

1. int[] arr = new int[3];  
2. int[] arr = new int[]{1,2,3,4,5};  
3. int[] arr = {1,2,3,4,5};  

4. **system.out.println(arr)——得到内存地址哈希值**

5. 数组一旦创建，程序运行期间，长度不可改变![image-20211017180317137](C:\Users\灯下黑\AppData\Roaming\Typora\typora-user-images\image-20211017180317137.png)

   但是这种是new了两个堆地址的

6. 数组遍历： array.fori

7. **数组可以作为方法的参数，当调用方法的时候，向方法的小括号进行传参，传递进去的其实是数组的地址值。**



## 内存

1. <font color='red'>stack：局部变量,方法的运行一定要在栈当中</font>

2. <font color='red'>heap：new出来的都在堆中，有16进制地址</font>

   字符默认为：‘\u0000’

   布尔默认为：false

   引用类型默认为：null

3. <font color='red'>方法区（method area）：储存.class相关信息，包含方法的信息。</font>

4. 本地方法栈（native method stack）：与操作系统相关

5. 寄存器（pc Register):与cpu相关

![image-20211017165517225](C:\Users\灯下黑\AppData\Roaming\Typora\typora-user-images\image-20211017165517225.png)







![image-20211017170806072](C:\Users\灯下黑\AppData\Roaming\Typora\typora-user-images\image-20211017170806072.png)

此处arrayB并没有重新new一个，直接**引用**了arrayA的内容，**地址相同，其实是同一个数组**