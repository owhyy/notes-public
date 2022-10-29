# Annotations
#Programming #Java #OOP
> Specifying something about some code
+ `@ Override`  tells the compiler that the method defined in a child [[Paradigm#^2e4af4|class]] overrides the method for base class; this makes it so if the arguments of the method of the base class change, you will get an error when using the child class argument, instead of calling the base class one:

```java
public class BaseClass { 
	public void doSomething(Object str) { 
		System.out.println("Base class:"+str); 
		} 
}

public class ChildClass extends BaseClass { 
	public void doSomething(String str) {  // no @Override
		System.out.println("Child class:"+str); 
		} 
}

BaseClass bc = new ChildClass();
bc.doSomething("override"); // Base class:override instead of expected Child class

```

```java
public class BaseClass { 
	public void doSomething(Object str) { 
		System.out.println("Base class:"+str); 
		} 
}

public class ChildClass extends BaseClass { 
	@Override
	public void doSomething(String str) {  s
		System.out.println("Child class:"+str); 
		} 
}

BaseClass bc = new ChildClass();
bc.doSomething("override"); // will signal error

```
