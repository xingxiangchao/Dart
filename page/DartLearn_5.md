5. 面向对象
    1. 类与对象，声明、创建及基本特性
        1. 类与对象
            1. 使用关键字 class 声明一个类
            2. 使用关键字new 创建一个对象，new 可省略
            3. 所有对象都继承与Object 类
        2. 属性与方法
            1. 属性默认会生成getter 和 setter 方法
            2. 使用final 声明的属性只有getter 方法
            3. 属性和方法通过.访问
            4. 方法不能被重载
        3. 类及成员可见性
            1. Dart 中的可见性以library(库)为单位
            2. 默认情况下，每一个Dart 文件就是一个库
            3. 使用_表示库的私有性
            4. 使用import 倒入库
        4. 计算属性
            1. 计算属性的值是通过计算而来，本身不存储值
            2. 计算属性赋值，其实是通过计算转换到其他实例变量
    2. 构造方法及初始化列表
        1. 构造方法
            1. 如果没有自定义构造方法，则会有个默认构造方法
            2. 如果存在自定义构造方法，则默认构造方法无效
            3. 构造方法不能重载
            4. 命名构造方法
                1. 使用命名构造方法，可以实现多个构造方法
                2. 使用类名.方法的形式实现
            5. 常量构造方法
                1. 如果类是不可变状态，可以把对象定义为编译时常量
                2. 使用const 声明构造方法，并且所有变量都为 final
                3. 使用const 声明对象，可以省略
                4. 如对象离的属性只需要被设置一次，就可以使用 const 来声明，因为常量在运行时更快，编译期就已经确定了。
            6. 工厂构造方法
                1. 工厂构造方法类似设计模式中的工厂模式
                2. 在构造方法前添加关键字factory实现一个工厂构造方法
                3. 在工厂构造方法中可返回对象
        2. 初始化列表
            1. 初始化列表会在构造方法体执行之前执行
            2. 使用逗号分隔初始化表达式
            3. 初始化列表常用于设置final 变量的值
    3. 静态成员及对象操作符的使用
        1. 静态成员
            1. 使用 static 关键字来实现类级别的变量和函数
            2. 静态成员不能访问非静态成员，非静态成员可以访问静态成员
            3. 类中的常量需要使用 static const 声明
        2. 对象操作符
            1. 条件成员访问： ?.（可以极大情况下处理空指针的情况）
            2. 类型转换： as
            3. 是否指定类型：is, is!
            4. 级连操作：..
        3. 对象call 方法
            1. 如果类实现了call() 方法，则该类的对象可以作为方法使用