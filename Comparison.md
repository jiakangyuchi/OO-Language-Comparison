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
   
   python:The automatic processing of docstrings to become properties of their owner. In general all of Python's brilliant introspection features make it a very unique language, from the ability to use help() to the ability to use __doc__ as a first-class property of an object. For example:
   
>>> class DocStringException(Exception):

...     """Error message is the same as docstring"""

...     def __str__(self):

...         return repr(self.__doc__)

... 

>>> class ExampleException(DocStringException):

...     """An example happened"""

... 

>>> raise ExampleException

Traceback (most recent call last):

  File "<stdin>", line 1, in <module>
  
__main__.ExampleException: 'An example happened'
   
[Go to README.md](README.md)
