# Why enum is used in java
* enums in Java are used to define a fixed set of named constants. They provide a way to create a collection of related values, making the code more readable, maintainable, and error-resistant. Enums enhance code clarity by replacing magic numbers or strings with self-explanatory, named constants. They improve type safety, preventing the assignment of invalid values, and can be utilized in switch statements for efficient control flow. Enums also support iteration over their values and can include instance variables and methods, allowing developers to associate data and behavior with each constant. This combination of features makes enums a valuable tool for defining and working with a limited set of related values in Java programs.
# Constructor in enum
* Enums are a data type in programming languages used to define a collection of named constants.
  These constants are typically used to represent a set of discrete values that are meaningful in a specific context.
  Enums make code more readable and self-documenting by replacing magic numbers or strings with descriptive names.

Here are some key points about enums:

1. Named Constants:
Enums allow you to define named constants. For example, instead of using 0 and 1 to represent weekdays and weekends, you can define an enum with the names Monday, Tuesday, Wednesday, etc., making the code more readable and understandable.

2. Distinct Values:
Enumerations represent distinct values, meaning each enum constant is unique within the enum type. This ensures that the values used are restricted to a specific set of options.

3. Sequential Numbers:
Enum values are often assigned sequential integers starting from 0 (although this can be customized). For instance, if you don't specify values for the enum constants, they will be assigned 0, 1
# Abscract method in enum:
* An abstract method in an enum is a method that is declared without an implementation, and must be implemented by each enum member. This allows each enum member to define its own behavior for a given operation, without having to use a switch statement on the enum type.

* Enums and Abstract Methods: While an enum itself cannot have abstract methods, you can define an interface with abstract methods and then have enum constants implement those methods. This allows you to enforce specific behavior for each enum constant.

* Interface Implementation: Enum constants implement the abstract methods defined in an interface that they declare they implement. Each enum constant provides its 
 own implementation of these methods, allowing for distinct behavior for each constant.

* Enforcing Behavior: Abstract methods in enums are useful for ensuring that each enum constant adheres to a specific contract or interface. It provides a way to 
 define a consistent set of methods that each constant must implement.
# Parameterized enum
* Parameterized enums can be useful for a variety of purposes. 
*Data-Driven Enums: Parameterized enums are used when you need to associate specific data or parameters with each enum constant. This data can be of any type, such as strings, numbers, or custom objects.

* Constructor with Parameters: To create parameterized enums, you define a constructor within the enum class that accepts the desired parameters. Each enum constant then provides values for these parameters when it's declared.

* Private Fields: The enum constants can have private fields to store the parameters. These fields are initialized in the constructor and can be accessed through getter methods.

* Methods and Behavior: Parameterized enums often include methods to access and manipulate the associated data. These methods can provide behavior or operations related to the enum constants.

* Real-World Modeling: Parameterized enums are especially useful when modeling real-world entities that have attributes or characteristics unique to each constant. Examples include representing fruits with color and taste or countries with population and GDP.

* Enhanced Expressiveness: Parameterized enums make code more expressive by encapsulating data and behavior within the enum itself. This improves code readability and maintainability.

* Enumerating Values: You can still iterate through the enum constants using values() and use them in switch statements or other control structures.
# Default enum in java
* default enums provided by the Java Standard Library offer a structured and standardized way to represent specific sets of values within various domains and functionalities. These enums are accessible through different packages and serve diverse purposes. Here's a summary of the default enums in Java:
Date and Time Enums: The java.time package provides enums like DayOfWeek and Month for representing days of the week and months of the year. These are crucial for modern date and time operations.
File System Enums: In the java.nio.file package, the FileVisitResult enum is used to determine the result of file and directory traversal operations, aiding file manipulation and management.
* HTTP Enums: In web development and the Spring Framework, enums like HttpStatus and HttpMethod (from org.springframework.http) are used to represent HTTP status codes and request methods, respectively.
Swing UI Enums: The JOptionPane enum (part of the Swing library) simplifies the creation of dialog boxes with various types, such as informational, warning, question, and error messages, enhancing user interaction in graphical applications.
* Annotation Processing Enums: The ElementType enum (from java.lang.annotation) is crucial for Java's annotation processing, specifying where annotations can be applied within code elements like classes, methods, and fields.
Thread State Enum: The Thread.State enum (from java.lang) represents the possible states of a thread in Java, aiding in thread management and synchronization.
Legacy Date and Time Enums: In older versions of Java, the java.util package offered DayOfWeek and Month enums with similar functionality to their java.time counterparts.
