---
type: topic
concept_type: data structure
prog_language: java
field: webDev
description: '"A simple Java object. It means Plain Old Java Object."'
---

'Plain old Java object'

For an object to be a POJO, it:
- can't extend classes
- can't implement interfaces
- can't use outside annotations

This is a POJO:
```java
public class cat {
	int age;
	String name;
}
```

This is not a POJO:
```java
public class cat extends someClass {
	int age;
	String name;
}
```

```java
@Entity
public class cat {
	int age;
	String name;
}
```

**A POJO is not a [[Java Bean]]!**


