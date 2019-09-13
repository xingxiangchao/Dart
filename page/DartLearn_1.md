1. Dart中的数据类型
    1. 变量与常量
        1. **变量**
            1. 使用var 声明变量，可赋予不同类型的值
            2. 未初始化时，默认值为null
            3. 使用关键字final声明一个只能赋值一次的变量
        2. **常量**
            1. 使用const 声明常量
            2. 使用const 声明的必须是编译期常量
        3. final 和 const 的区别
            1. const 是编译时常量，在编译的时候就初始化了，但是 final 变量是当类创建的时候才初始化。


    2. 内置类型
        1. 数值型 Number
            1. 整型 Int
            2. 浮点型 double
            3. 数值型操作
                1. 预算符 +、 -、 *、 / 、～/(取整)、 %;
                2. 常见属性 isNaN、isEven、isOdd
                3. 常用方法 abs()、round()、floor()、ceil()、toInt()、toDouble()
        2. 字符串 String
            1. 使用引号，双引号创建字符串
            2. 使用三个引号或者双引号创建多行字符串
            3. 使用r创建原始raw 字符串
            4. 字符串操作
                1. 运算符： +、*、==、[]
                2. 插值表达式：${expression}
                3. 常用属性：length、isEmpty、isNotEmpty
            5. 常用方法
                1. contains()、subString()
                2. startsWith()、endsWith()
                3. indexOf()、lastIndexOf()
                4. toLowerCase()、toUpperCase()
                5. trim()、trimLeft()、trimRight()
                6. split()、replaceXXX()
        3. 布尔型 Boolean
            1. 使用bool 来表示
            2. 值只有 true、 false
        4. 列表 List(数组)
            1. 创建List: var list = [1,2,3];
            2. 创建不可改变的List: var list = const[1,2,3];
            3. 构造创建：var List = new List();
            4. 常用操作
                1. [],length
                2. add(), insert()
                3. remove(),clear()
                4. indexof(),lastIndexOf()
                5. sort(),sublist()
                6. shuffle(),asMap(),forEach() 
        5. 键值对 Map
            1. 创建Map: var language = {'first': 'Dart', 'second': 'Java'};
            2. 创建不可改变Map: var language = const {'first': 'Dart', 'second': 'Java'};
            3. 构造创建：var language = new Map();
            4. 常用操作
                1. [],length
                2. isEmpty(),isNotEmpty()
                3. keys,values
                4. containsKey(),containsValue()
                5. remove()
                6. forEach()
        6. Runes,Symbols