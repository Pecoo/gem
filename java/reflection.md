### 获取反射的方式
1. Class.forName(path);
2. 类.class;
3. object.getClass();
4. ClassLoader.loadClass();
5. 基本数据类型 int.class double.class
6. 基本数据类型的包装类 Integer.Type

### 类加载时机：
1. 当创建对象时（new）
2. 当子类被加载时
3. 调用类中的静态成员时
4. 通过反射
### 类加载过程：
1. 加载：将.class文件加载进内存，并为之创建一个java.lang.Class对象。此过程由类加载器完成
2. 连接：Linking，将二进制数据合并到JRE中
    1. 验证
    2. 准备
    3. 解析
3. 初始化：JVM负责对类进行初始化，主要是对静态成员进行初始化