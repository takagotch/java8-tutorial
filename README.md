### java8-tutorial
---
https://github.com/winterbe/java8-tutorial

```java
interface Formula {
  double calculate(int a);
  
  default double sqrt(int a) {
    return Math.sqrt(a);
  }
}

Formula formula = new Formula() {
  @Override
  public double calculate(int a) {
    return sqrt(a * 100);
  }
};

formula.calculate(100);
formula.sqrt(16);

List<String> names = Arrays.asList("peter", "anna", "mike", "xenia");

Collections.sort(names, new Comparator<String>() {
  @Override
  public int compare(String a, String b) {
    return b.compareTo(a);
  }
});
```

```
```

```
```


