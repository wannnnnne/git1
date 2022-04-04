# day07

## int num:nums

这是一个foreach循环遍历....

就是把nums这个数组进行遍历，它有多少个数，就遍历多少遍。

遍历的时候每次就把其中的一个值给num;

for(int i =0;i<nums.length;i++){

  System.out.print(nums[i]+" ");

}

给这个for循环一样....

## number&math

1. 

```
注意 == 与 equals的区别
        == 它比较的是对象的地址
        equals 比较的是对象的内容
```

2. Java 会对 **-128 ~ 127** 的整数进行缓存，所以当定义两个变量初始化值位于 **-128 ~ 127** 之间时，两个变量使用了同一地址。当两个 Integer 变量的数值超出 **-128 ~ 127** 范围时, 变量使用了不同地址。
3.  int 是基本数据类型，int 变量存储的是数值。Integer 是引用类型，实际是一个对象，Integer 存储的是引用对象的地址。

## 类和对象

类名 对象名 = new 类名();  Student s = new Student();  

## 局部变量和成员变量

![image-20211027220534633](C:\Users\灯下黑\AppData\Roaming\Typora\typora-user-images\image-20211027220534633.png)