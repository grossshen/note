# SpringApplication
Class that can be used to bootstarp and launch a Spring application from a Java main method. By default class will perform the following steps to bootstrap you application:
1. create an ApplicationContext instance
2. expose command line arguments as Spring properties 
3. refresh the application context
4. loading all singleton beans
```java
public class MyApplication  {

  // ... Bean definitions

  public static void main(String[] args) throws Exception {
    SpringApplication.run(MyApplication.class, args);
  }
}
```
You can also custom the instance before `run()` method:
```java
public static void main(String[] args) throws Exception {
  SpringApplication application = new SpringApplication(MyApplication.class);
  // ... customize application settings here
  application.run(args)
}
```
