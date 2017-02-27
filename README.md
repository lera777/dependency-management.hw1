Dependency Management. Home Work 1
===============
0\. Preconditions
---------------
All tasks should be done only with raw JDK tools:
* `javac`
* `jar`
* etc

1\. Create Client interface JAR
---------------

Create new project and declare new interface named `Client`, that will have following contract:

```java
public interface Client{
    void setName(String name);
    void sayHello();
}
```

Create custom manifest file and fill following properties with your information:
* `Specification-Title` - The value is a string that defines the title of the extension specification
* `Specification-Vendor` - The value is a string that defines the organization that maintains the extension specification
* `Build-Date` - The value is a string that defines the date on which JAR file was build in following format: `YYYY-MM-DD`

Be sure to have appropriate package structure.

Prepare `.bat`/`.sh` script that should perform following:
* compile `Client` interface
* create `.jar` file with compiled class and custom `MANIFEST.MF`

2\. Create Client implementation executable JAR
---------------

Create new project and declare new implementation of `Client` interface named `ConsoleClient`.

This implementation should work with user input and system error output.

Create `Main` class, that creates new `Client` instantiated with `ConsoleClient` instance and:
* ask for user name
* greet user

Create custom manifest file and fill following properties with your information:
* `Main-Class` - The value is a string that denotes entry point of application
* `Specification-Title` - The value is a string that defines the title of the extension specification
* `Specification-Vendor` - The value is a string that defines the organization that maintains the extension specification
* `Build-Date` - The value is a string that defines the date on which JAR file was build in following format: `YYYY-MM-DD`

Prepare `.bat`/`.sh` script that should perform following:
* compile `ConsoleClient` and `Main` classes
* create executable `.jar` file

Prepare `.bat`/`.sh` script that should perform following:
* run executable `.jar` file with needed dependencies
