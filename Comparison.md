# OO-Language-Comparison

   [Go to README.md](README.md)
   
   [Go to code.txt](code.txt)
    
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
  
* Reflection
  * What reflection abilities are supported?
  
    python: A Python script can find out about the type, class, attributes and methods of an object.
    
    php: with Reflection, you won’t need to use many of these classes or methods.
  
  * How is reflection used?
  
    check code.txt please
    
* Memory management
  * How is it handled?
  
    php: The most important of its features for the Hacker, and the first thing to mention is tracking allocations. Tracking allocations allow the memory manager to avoid leaks, a thorn in the side of most Hackers. When PHP is built in debug mode (--enable-debug), detected leaks are reported, in a perfect world they would never get to deployment.
    
    python: Python's memory allocation and deallocation method is automatic. The user does not have to preallocate or deallocate memory by hand as one has to when using dynamic memory allocation in languages such as C or C++. Python uses two strategies for memory allocation reference counting and garbage collection. Manual Garbage Collection is also allowed.
  
  * How does it work?
  
    php: From the Hacker's perspective, the memory management API looks very much like libc's (or whoever the Hacker prefers !) malloc implementation.
  
    python: Memory management in Python involves a private heap containing all Python objects and data structures. The management of this private heap is ensured internally by the Python memory manager. The Python memory manager has different components which deal with various dynamic storage management aspects, like sharing, segmentation, preallocation or caching.
    
  * Garbage collection?
  
    php: A PHP variable is stored in a container called a "zval". A zval container contains, besides the variable's type and value, two additional bits of information. The first is called "is_ref" and is a boolean value indicating whether or not the variable is part of a "reference set". With this bit, PHP's engine knows how to differentiate between normal variables and references. 
    
    python:  Python schedules garbage collection based upon a threshold of object allocations and object deallocations. When the number of allocations minus the number of deallocations are greater than the threshold number, the garbage collector is run. Automatic garbage collection will not run if your Python device is running out of memory.
    
  * Automatic reference counting?
  
    both yes.
  
* Comparisons of references and values
  * How are values compared? (i.e. comparing two strings)
    
    Python uses "is" instead of "===" in php.
    
    php uses "!==" to find out if $a is not equal to $b, or they are not of the same type.
    
    php uses "<=>" to find out if an integer less than, equal to, or greater than zero when $a is respectively less than, equal to, or greater than $b
  
* Null/nil references
  * Which does the language use? (null/nil/etc)
  
    python:none;
    
    php:null
 
  * Does the language have features for handling null/nil references?
  
    python:has no value or the value is None.
    
    php: has no value or the value is NULL
    
* Errors and exception handling
    
    php:The error reporting functions allow you to customize what level and kind of error feedback is given, ranging from simple notices to customized functions returned during errors.
    
    python:It is possible to write programs that handle selected exceptions. Look at the following example, which asks the user for input until a valid integer has been entered, but allows the user to interrupt the program (using Control-C or whatever the operating system supports); note that a user-generated interruption is signalled by raising the KeyboardInterrupt exception.


* Lambda expressions, closures, or functions as types

  python: Python supports the creation of anonymous functions (i.e. functions that are not bound to a name) at runtime, using a construct called "lambda". This is not exactly the same as lambda in functional programming languages, but it is a very powerful concept that's well integrated into Python and is often used in conjunction with typical functional concepts like filter(), map() and reduce().

  php:a lambda function is an anonymous PHP function that can be stored in a variable and passed as an argument to other functions or methods. A closure is a lambda function that is aware of its surrounding context.

* Implementation of listeners and event handlers

  check code.txt please.

* Singleton
  * How is a singleton implemented?
  
    python:Possibly the simplest design pattern is the singleton, which is a way to provide one and only one object of a particular type. To accomplish this, you must take control of object creation out of the hands of the programmer. One convenient way to do this is to delegate to a single instance of a private nested inner class
    
    php:In the singleton pattern a class can distribute one instance of itself to other classes.
  
  * Can it be made thread-safe?
  
    php: yes, but your php version has to be thread-safe.
    
    python: yes
  
  * Can the singleton instance be lazily instantiated?
  
    python:yes
    
    php:yes
  
* Procedural programming
  * Does the language support procedural programming?
    
    python:yes
    
    php: yes
    
* Functional programming
  * Does the language support functional programming?
  
    python: yes, but it is not very good for functional programming.
    
    php:yes
    
* Multithreading
  * Threads or thread-like abilities
  
    python: only one thread can safely execute code in the interpreter at the same time.
    
    php: PHP is not a threaded language : its engine and its code don't manage threads to parallelize its own internal work. PHP doesn't offer threads to users : You can't use threads with the PHP language natively. 
  
  * How is multitasking accomplished?
    
    php: it hides the complex async work behind a promises-based interface.
    
    python: MultiTasking is a tiny Python library lets you convert your Python methods into asynchronous, non-blocking methods simply by using a decorator.
    
   [Go to README.md](README.md)
   
   [Go to code.txt](code.txt)
