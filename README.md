# ClassGenerator
帮助项目开发时，自动生成类的代码。


## 例子：

当我写出如下代码
```
@SimpleGenerator
public abstract class PersonBean {

    public String name;
    public int age;
}
```
自动帮我生成一个类 
```
public class PersonBeanX extends PersonBean {
  private String name;

  private int age;

  public void setName(String name) {
    this.name = name;
  }

  public String getName(String name) {
    return this.name;
  }

  public void setAge(int age) {
    this.age = age;
  }

  public int getAge(int age) {
    return this.age;
  }

  public void PersonBean(String name, int age) {
    this.name = name;
    this.age = age;
  }
}

```

-------------------

## 鸣谢
[http://www.cjsdn.net/Doc/JDK60/](http://www.cjsdn.net/Doc/JDK60/)
[https://github.com/square/javapoet](https://github.com/square/javapoet)