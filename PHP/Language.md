# Junior Level
PHP tags (standard, echo, short). 

Single line comments; multi-line comments.

Write data to the script’s output: echo vs print();

Script termination. 

Data types: 4 scalar types, 4 compound types, 2 special types. Pseudo-types. 

Type Casting (with casting operators and functions). Detecting Types. 

Variables (naming, case-sensitivity). Variable variables.

Constants. Possible ways to define. Possible values that they contain. Magic constants.

### Operators
Operator precedence.

Arithmetic operators ($a**2 etc)

Assignment operators ($a = 1 vs $a += 1, $a = $b vs $a = &$b etc)

Bitwise Operators

Comparison Operators ($a == $b,  $a === $b etc); Comparing of float values with epsilon technique.

Error Control operator

Execution (backtick) operator

Incrementing/Decrementing Operators (echo $a++ vs echo ++$a)

Logical Operators ($a && $b, $a || $b, !$a etc.)

String operators (concatenation and concatenating assignment)

Array Operators ($arr + $arrB,  $arr == $arrB etc. )

Type Operators (instanceof)

Debug functions (var_dump(), var_export(), print_r())

### Control structures
if, while, for, foreach, switch and their alternative syntax.

'Fall through' in switch statement

continue and break statements

Ternary Operators

Null coalescing operator (??)

require vs include

### Functions.
Global and functional scope.

Type-hinting in functions.

Return type declaration.

Arguments by reference.

Variable length argument list: func_get_args() and variadics

Static variables in functions

### Strings
Single quotes vs Double quotes

Heredoc and Nowdoc Syntax

Strings as Arrays

Search & replace
 
Using printf() for formatting

### Arrays
Enumerative and associative

Short array syntax

Iteration of an array:
* by using reset(), current(),next() 
* by using foreach

Working with arrays as a stack and as a queue

Validate (in_array(), array_key_exists() etc)

Sort and shuffle arrays

### Web
HTTP request: HTTP method, URI, headers and request body.

HTTP response: status code,headers and content.

Web-Form submit

Data format inside request body

$_GET, $_POST, $_REQUEST

$_FILES

Сookies and sessions in php

### OOP Fundamentals
Class vs object

Inheritance

Class methods and properties visibility. Default visibility.

Working with filesystem with C-style functions (open/create, read, write, and close a file handle, working with folders, controlling file access)

# Middle Level
### Arrays
Iteration of an array by specific functions with callbacks.

Compare arrays (array_diff(),  array_intersect() etc)

Array merging (array_merge vs '+')

### Strings
Regular expressions (preg_match(), named matches etc)

Multibyte string functions (mb_*)

Dealing with URL strings: encoding, decoding and parsing

### OOP
get_class() and instanceof keyword

final keyword

$this vs self

static keyword

late static binding

Magic methods (constructors, object as callable, overloading etc)

Interfaces and Abstract Classes

Scope resolution operator

::class keyword

Namespaces

Horizontal inheritance via traits

### Errors and Exceptions
Error Reporting

Handling Errors, set_error_handler()
   
Exception  class, extending Exception class. Throwable interface

Throwing and catching Exceptions, set_exception_handler()  

### Autoloading
require vs require_once vs __autoload() vs spl_autoload_register()

PSR-0 vs PSR-4

Working with filesystem via streams in PHP

file_get_contents(), file_put_contents()


### Data formats
JSON (encode/decode,  from/into objects and arrays)

Dates and Times : DateTime and DateTimeImmutable classes

XML:SimpleXml and Dom (document parsing, xpath queries, create and modify documents)
Document exchange between SimpleXml and Dom

### Security
‘Filter input Escape output’ rule

ctype_* functions, filter_var()
 
Password security: password_hash() and password_verify()

Symmetric and asymmetric keys concepts

HTTPS concept

Cross-site scripting (XSS)

Cross-Site Request Forgeries

SQL injection attacks prevention

Ways to defend against session fixation and session hijacking.

Remote code injection and allow_url_fopen directive in php.ini
 
### Output buffering control 
ob_start(), ob_get_contents(), ob_end_clean();

### PHP in console
Running php code in console

Running php built-in server

Running php linter

Writing a simple CLI program on PHP

### WebServices
REST (messages format, endpoints naming, HTTP methods as API verbs, data format inside of a message body, read message body from 'php://input', HTTP status codes in response, HATEOAS, API versioning)

SOAP (WSDL file, SoapClient and SoapServer classes)

Oauth

### Working with Databases
MySQL Improved Extension (mysqli)
PDO MySQL
PDO prepared statements, fetching query results, transactions with PDO

### Other
phpdoc (@param, @return, @var etc)

Script delay execution. Script max execution time. Evaluate a string as PHP code. 

Image Processing and Generation

# Senior Level
### OOP
Anonymous classes

Cloning object

Reflection API

### Anonymous functions and Closures
Closure class

Using $this in closures

Specifying a class with bindTo()

Predefined Interfaces:  ArrayAccess, Serializable, Traversable, Iterator and IteratorAggregate

Generators

### SPL 
Data structures (SplStack, SplFixedArray etc)

Iterators (ArrayIterator, RecursiveIteratorIterator  etc )
 
Exceptions (LogicException, BadFunctionCallException etc )

Functions (class_implements(), class_uses())

### Working with external resources via streams
stream_socket_server() and stream_socket_client()

Stream filters.  I/O streams: 'php://stdin' and 'php://stdout'

### Other
Run PHP process in the background

Code profiling and optimization
