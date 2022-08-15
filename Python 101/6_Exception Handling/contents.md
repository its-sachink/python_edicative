## Exception Handling

Let’s say you try to open a file, but you typed in the wrong path or you ask the user for information and they type in some garbage. You don’t want your program to crash, so you implement exception handling. In Python, the construct is usually wrapped in what is know as a **try/except**.

- Some common built-in exceptions are

**Exception** (this is what almost all the others are built off of)
**AttributeError** - Raised when an attribute reference or assignment fails.
**IOError** - Raised when an I/O operation (such as a print statement, the built-in open() function or a method of a file object) fails for an I/O-related reason, e.g., “file not found” or “disk full”.
**ImportError** - Raised when an import statement fails to find the module definition or when a from … import fails to find a name that is to be imported.
**IndexError** - Raised when a sequence subscript is out of range.
**KeyError** - Raised when a mapping (dictionary) key is not found in the set of existing keys.
**KeyboardInterrupt** - Raised when the user hits the interrupt key (normally Control-C or Delete).
**NameError** - Raised when a local or global name is not found.
**OSError** - Raised when a function returns a system-related error.
**SyntaxError** - Raised when the parser encounters a syntax error.
**TypeError** - Raised when an operation or function is applied to an object of inappropriate type. The associated value is a string giving details about the type mismatch.
**ValueError** - Raised when a built-in operation or function receives an argument that has the right type but an inappropriate value, and the situation is not described by a more precise exception such as IndexError.
**ZeroDivisionError** - Raised when the second argument of a division or modulo operation is zero.

