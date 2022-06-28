# Funciones integradas comunes
[ Mas información](https://docs.python.org/3/library/functions.html)
## Conversion de entero a binario:
````python
print(bin(10))
````
OUT:
````bash
0b1010
````
## Conversion de entero a hexadecimal
````python
print(hex(10))
````
OUT:
````bash
0xa
````
## Int() con base: Reconversion a entero(base 10)
````python
print(int('0b1010',2))
````
OUT:
````bash
10
````
## abs(): Valor absoluto de un numero (distancia)
````python
print(abs(-10))
print(abs(10))
````
OUT:
````bash
10
10
````

## round(): Redondeo de un flotante a entero.
Menor de .5 a la baja, Mayor o igual a .5 al alza
````python
print(round(5.5))
print(round(5.4))
````
OUT:
````bash
6
5
````
## eval(): Evalua una cadena como una expresion
Acepta variables si se han definido anteriormente
````python
n = 10
print(eval('2+5'))
print(eval('n*10 - 5'))
````
OUT:
````bash
7
95
````
## help(): Invocar el menu de ayuda del interprete de Python
````python
help()
````
OUT:
````python
Welcome to Python 3.5's help utility! If this is your first time using Python, you should definitely check out the tutorial on the Internet at [http://docs.python.org/3.5/tutorial/](http://docs.python.org/3.5/tutorial/). Enter the name of any module, keyword, or topic to get help on writing Python programs and using Python modules. To quit this help utility and return to the interpreter, just type "quit". To get a list of available modules, keywords, symbols, or topics, type "modules", "keywords", "symbols", or "topics". Each module also comes with a one-line summary of what it does; to list the modules whose name or summary contain a given string such as "spam", type "modules spam". help> topics Here is a list of available topics. Enter any topic name to get more help. ASSERTION DELETION LOOPING SHIFTING ASSIGNMENT DICTIONARIES MAPPINGMETHODS SLICINGS ATTRIBUTEMETHODS DICTIONARYLITERALS MAPPINGS SPECIALATTRIBUTES ATTRIBUTES DYNAMICFEATURES METHODS SPECIALIDENTIFIERS AUGMENTEDASSIGNMENT ELLIPSIS MODULES SPECIALMETHODS BASICMETHODS EXCEPTIONS NAMESPACES STRINGMETHODS BINARY EXECUTION NONE STRINGS BITWISE EXPRESSIONS NUMBERMETHODS SUBSCRIPTS BOOLEAN FLOAT NUMBERS TRACEBACKS CALLABLEMETHODS FORMATTING OBJECTS TRUTHVALUE CALLS FRAMEOBJECTS OPERATORS TUPLELITERALS CLASSES FRAMES PACKAGES TUPLES CODEOBJECTS FUNCTIONS POWER TYPEOBJECTS COMPARISON IDENTIFIERS PRECEDENCE TYPES COMPLEX IMPORTING PRIVATENAMES UNARY CONDITIONAL INTEGER RETURNING UNICODE CONTEXTMANAGERS LISTLITERALS SCOPING CONVERSIONS LISTS SEQUENCEMETHODS DEBUGGING LITERALS SEQUENCES help> ATRIBUTES No Python documentation found for 'ATRIBUTES'. Use help() to get the interactive help utility. Use help(str) for help on the str class. help> ATTRIBUTES Attribute references ******************** An attribute reference is a primary followed by a period and a name: attributeref ::= primary "." identifier The primary must evaluate to an object of a type that supports attribute references, which most objects do. This object is then asked to produce the attribute whose name is the identifier. This production can be customized by overriding the "__getattr__()" method. If this attribute is not available, the exception "AttributeError" is raised. Otherwise, the type and value of the object produced is determined by the object. Multiple evaluations of the same attribute reference may yield different objects. Related help topics: getattr, hasattr, setattr, ATTRIBUTEMETHODSWelcome to Python 3.5's help utility! If this is your first time using Python, you should definitely check out the tutorial on the Internet at [http://docs.python.org/3.5/tutorial/](http://docs.python.org/3.5/tutorial/). Enter the name of any module, keyword, or topic to get help on writing Python programs and using Python modules. To quit this help utility and return to the interpreter, just type "quit". To get a list of available modules, keywords, symbols, or topics, type "modules", "keywords", "symbols", or "topics". Each module also comes with a one-line summary of what it does; to list the modules whose name or summary contain a given string such as "spam", type "modules spam". help> topics Here is a list of available topics. Enter any topic name to get more help. ASSERTION DELETION LOOPING SHIFTING ASSIGNMENT DICTIONARIES MAPPINGMETHODS SLICINGS ATTRIBUTEMETHODS DICTIONARYLITERALS MAPPINGS SPECIALATTRIBUTES ATTRIBUTES DYNAMICFEATURES METHODS SPECIALIDENTIFIERS AUGMENTEDASSIGNMENT ELLIPSIS MODULES SPECIALMETHODS BASICMETHODS EXCEPTIONS NAMESPACES STRINGMETHODS BINARY EXECUTION NONE STRINGS BITWISE EXPRESSIONS NUMBERMETHODS SUBSCRIPTS BOOLEAN FLOAT NUMBERS TRACEBACKS CALLABLEMETHODS FORMATTING OBJECTS TRUTHVALUE CALLS FRAMEOBJECTS OPERATORS TUPLELITERALS CLASSES FRAMES PACKAGES TUPLES CODEOBJECTS FUNCTIONS POWER TYPEOBJECTS COMPARISON IDENTIFIERS PRECEDENCE TYPES COMPLEX IMPORTING PRIVATENAMES UNARY CONDITIONAL INTEGER RETURNING UNICODE CONTEXTMANAGERS LISTLITERALS SCOPING CONVERSIONS LISTS SEQUENCEMETHODS DEBUGGING LITERALS SEQUENCES help> ATRIBUTES No Python documentation found for 'ATRIBUTES'. Use help() to get the interactive help utility. Use help(str) for help on the str class. help> ATTRIBUTES Attribute references ******************** An attribute reference is a primary followed by a period and a name: attributeref ::= primary "." identifier The primary must evaluate to an object of a type that supports attribute references, which most objects do. This object is then asked to produce the attribute whose name is the identifier. This production can be customized by overriding the "__getattr__()" method. If this attribute is not available, the exception "AttributeError" is raised. Otherwise, the type and value of the object produced is determined by the object. Multiple evaluations of the same attribute reference may yield different objects. Related help topics: getattr, hasattr, setattr, ATTRIBUTEMETHODS
````