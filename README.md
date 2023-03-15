# Lab-5_202001065

## Github Repository:

The repository used for the static analysis is called MyGPTReader by the github user, madawei2699.
The link to this repository is: https://github.com/madawei2699/myGPTReader.
This repository includes one python file, named server.py which was analysed using PyLint. 


## Tool Output:

server.py:30:0: C0301: Line too long (217/100) (line-too-long)

server.py:86:0: C0301: Line too long (101/100) (line-too-long)

server.py:110:0: C0303: Trailing whitespace (trailing-whitespace)

server.py:132:0: C0303: Trailing whitespace (trailing-whitespace)

server.py:162:0: C0301: Line too long (101/100) (line-too-long)

server.py:203:0: C0304: Final newline missing (missing-final-newline)

server.py:1:0: C0114: Missing module docstring (missing-module-docstring)

server.py:39:0: C0116: Missing function or method docstring (missing-function-docstring)

server.py:42:0: C0116: Missing function or method docstring (missing-function-docstring)

server.py:60:0: C0116: Missing function or method docstring (missing-function-docstring)

server.py:64:16: C0103: Variable name "e" doesn't conform to snake_case naming style (invalid-name)

server.py:70:0: C0116: Missing function or method docstring (missing-function-docstring)

server.py:73:0: C0116: Missing function or method docstring (missing-function-docstring)

server.py:88:0: C0116: Missing function or method docstring (missing-function-docstring)

server.py:93:0: C0116: Missing function or method docstring (missing-function-docstring)

server.py:99:15: W3101: Missing timeout argument for method 'requests.get' can cause your program to hang indefinitely (missing-timeout)

server.py:106:8: W0702: No exception type(s) specified (bare-except)

server.py:111:0: C0116: Missing function or method docstring (missing-function-docstring)

server.py:124:15: W3101: Missing timeout argument for method 'requests.post' can cause your program to hang indefinitely (missing-timeout)

server.py:128:8: W0702: No exception type(s) specified (bare-except)
server.py:133:0: C0116: Missing function or method docstring (missing-function-docstring)

server.py:147:0: C0116: Missing function or method docstring (missing-function-docstring)

server.py:147:0: C0103: Function name "get_answer_from_chatGPT" doesn't conform to snake_case naming style (invalid-name)

server.py:166:0: C0116: Missing function or method docstring (missing-function-docstring)

server.py:177:0: C0116: Missing function or method docstring (missing-function-docstring)

server.py:3:0: C0411: standard import "import re" should be placed before "from flask import Flask, request" (wrong-import-order)

server.py:4:0: C0411: standard import "import os" should be placed before "from flask import Flask, request" (wrong-import-order)

server.py:9:0: C0411: standard import "import json" should be placed before "from flask import Flask, request" (wrong-import-order)

server.py:17:0: C0411: standard import "import concurrent.futures" should be placed before "from flask import Flask, request" (wrong-import-order)


## My understanding of the output

1. C0301: Line too long (217/100) (line-too-long)
This error shows that a line of code exceeds the suggested length of 100 characters. There are 217 letters on one line of the code.

2. C0301: Line too long (101/100) (line-too-long)
Similar to the first error, the offending line in this instance is only 101 characters long—just one character longer..

3. C0303: Trailing whitespace (trailing-whitespace)
This error shows that a line's conclusion contains whitespace. The spaces can be eliminated to correct this.

4. C0304: Final newline missing (missing-final-newline)
This error means that the ending of this file does not contain a newline character. We can fix this mistake by adding a newline character.

5. C0114: Missing module docstring (missing-module-docstring)
This error indicates that the complete module lacks a docstring. A text called a "docstring" explains the function and goal of a module.

6. C0116: Missing function or method docstring (missing-function-docstring)
The error indicates that docstring is absent for a particular function or method

7. C0103: Variable name "e" doesn't conform to snake_case naming style (invalid-name)
The variable name "e" does not adhere to the snake case naming practise, which is the cause of the error.

8. W3101: Missing timeout argument for method 'requests.get' can cause your program to hang indefinitely (missing-timeout)
This warning indicates that a timeout argument is missing from a call to the 'requests.get' method. By adding a timeout argument, we can prevent the program from hanging indefinitely.

9. W0702: No exception type(s) specified (bare-except)
This error shows that an exception block does not define the kinds of errors it will detect.

10. C0103: Function name "get_answer_from_chatGPT" doesn't conform to snake_case naming style (invalid-name)
This error is similar to error C0103 (error 7), but it refers to a function name instead of a variable name.

11. C0411: standard import "import re" should be placed before "from flask import Flask, request" (wrong-import-order)
This error indicates that third-party imports should come before regular imports. The "import re" declaration sould be placed above the "from flask import Flask, request" sentence in this situation.

12. C0412: Imports from package slack_bolt are not grouped (ungrouped-imports)
This error tells that we should group imports from the 'slack bolt' package.
