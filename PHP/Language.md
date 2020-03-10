# Junior Level
PHP tags (standard, echo, short). 

Single line comments; multi-line comments.

Write data to the script’s output: echo vs print();

Script termination. 

Data types: 4 scalar types, 4 compound types, 2 special types. Pseudo-types. (*) 

Type Casting (with casting operators and functions). Detecting Types. (*)  

Variables
    * naming, case-sensitivity (*)
    * Variable variables.

Constants:
* Possible ways to define. 
* Possible types that they contain. 
* Magic constants. (*) 

### Operators
Operator precedence.

Arithmetic operators ($a**2 etc)

Assignment operators ($a = 1 vs $a += 1, $a = $b vs $a = &$b etc) (*) 

Comparison Operators ($a == $b,  $a === $b etc); Comparing of float values with epsilon technique. (*) 

Error Control operator

Incrementing/Decrementing Operators (echo $a++ vs echo ++$a)

Logical Operators ($a && $b, $a || $b, !$a etc.). Limitations of using with different types of arguments. (*) 

String operators (concatenation and concatenating assignment)

Array Operators ($arr + $arrB,  $arr == $arrB etc. ) (*) 

Type Operators (instanceof) (*) 

Debug functions (var_dump(), var_export(), print_r())

### Control structures
if, while, for, foreach, switch and their alternative syntax.

'Fall through' in switch statement

continue and break statements (*)

Ternary Operators (*) 

Null coalescing operator (??) (*) 

Spaceship operator (<=>)

require vs include

### Functions
Global and functional scope, 'global' keyword, $GLOBALS

Typed parameters and return type declaration. (*) 

Nullable and void type declarations.

Argument default value

Arguments by reference. (*) 

Arguments unpacking. (function test(...$args){})

### Strings
Single quotes vs Double quotes (*) 

Heredoc and Nowdoc Syntax
* Indentation changes in PHP 7.3

Strings as Arrays. Positive and negative offsets.

Search & replace (*)
 
Using printf(), sprintf() for formatting

### Arrays
Enumerative and associative (*)

Short array syntax

Iteration of an array by using foreach

Working with arrays as a stack and as a queue: array_push(), array_pop(), array_shift(), array_unshift()

Validate (in_array(), array_key_exists() etc)

Sort and shuffle arrays (*)

Spread Operator in Array Expression

Unpacking arrays to variables using list(). Difference between unpacking by value and by reference. 

### Web
HTTP request: HTTP method, URI, headers and request body. (*)

HTTP response: status code,headers and content. (*)

Web-Form submit

Data format inside request body

$_GET, $_POST, $_REQUEST (*)

$_FILES

Cookies and sessions in php (*)

### OOP Fundamentals
Class vs object (*)

Inheritance

Class methods and properties visibility. Default visibility. (*)

Accessing protected/private class properties

Typed properties

### Other
phpdoc (*)
* tags (@param, @return, @var etc). 
* Differences from type hinting 

Working with filesystem with C-style functions (open/create, read, write, and close a file handle, working with folders)

# Middle Level

Difference between a language construct and a built-in function

### Operators
Execution (backtick) operator

Bitwise Operators

### Arrays
Iteration of an array: (*)
* by using reset(), current(),next() 
* by specific functions with callbacks

Compare arrays (array_diff(),  array_intersect() etc)

Array merging (array_merge vs '+') (*)

### Strings
Regular expressions (*)
* preg_match(), flags, named matches 
* preg_replace*() functions. Replace using matches, callbacks 

Multibyte string functions (mb_*)

Dealing with URL strings: encoding, decoding and parsing (*)

### Functions
Variable length argument list: func_get_args() and variadics

Static variables in functions (*)

Anonymous functions and Closures concepts. Arrow functions (*)

call_user_func(), call_user_func_array() (*)

### OOP
get_class() and instanceof keyword

final keyword

$this vs self (*)

static properties and methods (*)

Magic methods (*)
* constructors, 
* overloading methods and properties
* object as callable
* serialization and json encoding control
     __serialize/__unserialize. vs __sleep/__wakeup

Interfaces and Abstract Classes (*)

Scope resolution operator

::class constant

Namespaces. Use, group use, aliases (*)

### Errors and Exceptions
Error Reporting

Handling Errors, set_error_handler()
   
Exception  class, extending Exception class. Throwable interface (*)

Throwing and catching Exceptions, set_exception_handler(), Multi-Catch Exception Handling (*)

Expectations

### Autoloading
require vs require_once (*)

__autoload()(deprecated) vs spl_autoload_register()

[PSR-0](https://www.php-fig.org/psr/psr-0/) (Deprecated) vs [PSR-4](https://www.php-fig.org/psr/psr-4/) (*)

### Data formats
JSON (encode/decode, from/into objects and arrays) (*)

Dates and Times : DateTime and DateTimeImmutable classes

XML:SimpleXml and Dom (document parsing, xpath queries, create and modify documents)
Document exchange between SimpleXml and Dom

### Security
‘Filter input Escape output’ rule (*)

ctype_* functions, filter_var()
 
Password security: password_hash() and password_verify()

HTTPS concept (*)

Cross-site scripting (XSS) (*)

Cross-Site Request Forgeries

SQL injection attacks prevention (*)

Remote code injection and allow_url_fopen directive in php.ini
 
### Output buffering control 
ob_start(), ob_get_contents(), ob_end_clean(); (*)

### PHP in console
Running php code in console (*)

Running php built-in server

Running php linter

Writing a simple CLI program on PHP (*)

### WebServices
REST (messages format, endpoints naming, HTTP methods as API verbs, data format inside of a message body, read message body from 'php://input', HTTP status codes in response, HATEOAS, API versioning) (*)

SOAP (WSDL file, SoapClient and SoapServer classes)

Oauth (*)

### Working with Databases
MySQL Improved Extension (mysqli)

PDO MySQL

PDO prepared statements, fetching query results, transactions with PDO (*)

### Other

Working with filesystem via streams in PHP (*)

file_get_contents(), file_put_contents()

FTP functions in PHP

Working with curl

Script delay execution. Script max execution time. Evaluate a string as PHP code. (*)

Image Processing and Generation

# Senior Level
### OOP
Late static binding (self::$property vs static::$property) (*)

Horizontal inheritance via traits (*)

Anonymous classes

Cloning object

Reflection API

Closure class (*)

Using $this in closures (*)

Specifying a class with bindTo()

Predefined Interfaces:  ArrayAccess, Serializable, Traversable, Iterator and IteratorAggregate (*)

Generators. yield, yield from, Generator::gerReturn()

### SPL 
Data structures (SplStack, SplFixedArray etc)

Iterators (ArrayIterator, RecursiveIteratorIterator  etc ) (*)
 
Exceptions (LogicException, BadFunctionCallException etc ) (*)

Functions (class_implements(), class_uses())

### Working with external resources via streams
stream_socket_server() and stream_socket_client()

Stream filters.  I/O streams: 'php://stdin' and 'php://stdout'

### Other
Using queues for asynchronous and synchronous delegating of operations.

Foreign function interface (FFI)

### Performance
Code profiling and optimization (*)
* possible bottlenecks
* ways of determining the problem

PHP Preloading

OpCache

[Some tips of Improving PHP Performance] (https://www.keycdn.com/blog/php-performance)