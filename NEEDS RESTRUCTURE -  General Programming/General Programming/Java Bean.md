---
type: topic
concept_type: data structure
prog_language: java
field: webDev
description: '"A Java object that can be turned into a JSON or XML."'
---

For a class to be a Java bean:
- No-args constructor (default constructor)
- Properties must be private
- Public getters and setters
- **Must be serializable** -> Basically Java tells the program that this class can be turned into data to be written or something into a database and such. You just need to add *implements Serialiazable*

This is a Java Bean:

```java
public class cat implements Serialiazable {
	private int age;
	private String name;
	public void setAge(int age) {...}
	// setters and geters for age and name...
	public cat(){}
}
```

or, you can use *record*:
```java
public record cat(int age, String name){}
```

**Java Beans are not [[POJO]]s**

Useful in turning Java objects into JSON/XML responses to fetch requests in [[Java Spring Resources|Java Spring and other backend web development]].
