# OO-Language-Comparison
Compare Python and Php

* Language purpose/genesis
  * Why was the language created?
  
  php:It is a widely-used Open Source general-purpose scripting language that is especially suited for web development and can be embedded  into HTML.
  
  python: Guido van Rossum(the author) decided to write an interpreter for the new scripting language which is a descendant of ABC that  would appeal to Unix/C hackers. 
  
  * What problems was the language trying to address?
  
  php:The main goal of the language is to allow web developers to write dynamically generated web pages quickly
  
  python:Making it fun, beautiful, simple and readable, and making it an ideal language for scripting and rapid application development in many areas on most platforms.
  
  * Is the language a reaction to a previous language or a replacement for another language?
  
  Php:Its syntax draws upon C, Java, and Perl.
  
  python:The Python interpreter is easily extended with new functions and data types implemented in C or C++ (or other languages callable from C).
  
 * Unique features of the language
   * Does the language have any particularly unique features?
   
   php:Yes, like variable variables, Real-Time Access Monitoring, and PHP supports variable usage without declaring its data type.
   
   python:The automatic processing of docstrings to become properties of their owner. In general all of Python's brilliant introspection features make it a very unique language, from the ability to use help() to the ability to use __doc__ as a first-class property of an object.

* Name spaces
  * How are name spaces implemented?
  * How are name spaces used?
  
  php:In the PHP world, namespaces are designed to solve two problems that authors of libraries and applications encounter when creating re-usable code elements such as classes or functions:

1 Name collisions between code you create, and internal PHP classes/functions/constants or third-party classes/functions/constants.

2 Ability to alias (or shorten) Extra_Long_Names designed to alleviate the first problem, improving readability of source code.

PHP Namespaces provide a way in which to group related classes, interfaces, functions and constants. 

  python:A namespace is a mapping from names to objects. Most namespaces are currently implemented as Python dictionaries, but that’s normally not noticeable in any way (except for performance), and it may change in the future. Examples of namespaces are: the set of built-in names (containing functions such as abs(), and built-in exception names); the global names in a module; and the local names in a function invocation. In a sense the set of attributes of an object also form a namespace. The important thing to know about namespaces is that there is absolutely no relation between names in different namespaces; for instance, two different modules may both define a function maximize without confusion — users of the modules must prefix it with the module name.
  
 * Types
   * What types does the language support?
   
   php:String, Integer, Float (floating point numbers - also called double), Boolean, Array, Object, NULL, Resource.
   
   python:str, bytearray, bytes, list, tuple, set, frozenset, dict, int, float, complex, bool, ellipsis.
   
   * Are both reference and value types supported?
   
   php:yes
   
   python:yes
   
   * Can new value types be created?
   
   php:no
   
   python:yes
   
* Classes
  * Defining
  
  php:Basic class definitions begin with the keyword class, followed by a class name, followed by a pair of curly braces which enclose the definitions of the properties and methods belonging to the class.

The class name can be any valid label, provided it is not a PHP reserved word. A valid class name starts with a letter or underscore, followed by any number of letters, numbers, or underscores. As a regular expression, it would be expressed thus: ^[a-zA-Z_\x7f-\xff][a-zA-Z0-9_\x7f-\xff]*$.

A class may contain its own constants, variables (called "properties"), and functions (called "methods").

python: Class definitions, like function definitions (def statements) must be executed before they have any effect. (You could conceivably place a class definition in a branch of an if statement, or inside a function.)

Non-static attributes in php are like self. in python, and static attrubutes in php are like classes in python。

  * Creating new instances
  
  php:In the class context, it is possible to create a new object by new self and new parent.
  
  python:Class instantiation uses function notation. Just pretend that the class object is a parameterless function that returns a new instance of the class.
  
  * Constructing/initializing
  
  constructor is implied to be a static which is different with php.
  
  * Destructing/de-initializing
  
  In php, parent destructors will not be called implicitly by the engine. In order to run a parent destructor, one would have to explicitly call parent::__destruct() in the destructor body.
  
* Instance reference name in data type (class)
  * this?  self?
  
  Python does not have "this", it use "self" as a reference to the instance. And php use "this" as a reference to the instance.
  
* Properties
  * Getters and setters...write your own or built in?
  
  both build in.
  
  * Backing variables?
  
  both yes.
  
  * Computed properties?
  
  both yes.
  
  Python code doesn’t typically use the get and set methods so common in PHP. it has a construct called a “property”.
  
* Interfaces / protocols
  * What does the language support?
  
  php:both
  
  python:both
  
  * What abilities does it have?
  
    It's possible for interfaces to have constants in both languages.

  * How is it used?
  
    php:Object interfaces allow you to create code which specifies which methods a class must implement, without having to define how these methods are handled.

Interfaces are defined in the same way as a class, but with the interface keyword replacing the class keyword and without any of the methods having their contents defined.

All methods declared in an interface must be public; this is the nature of an interface.

   python: Interface requirements are checked at class creation time, rather than at instance creation time. This means that interface can tell you if a class fails to meet the requirements of an interface even if you never create any instances of that class. interface requires that method signatures of interface implementations are compatible with the signatures declared in the interface. 
  
* Inheritance / extension
  
  Python has multiple inheritance, and there's less need for interfaces.
  
  php does not has multiple inheritance.
[Go to README.md](README.md)
