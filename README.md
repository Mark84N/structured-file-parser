# structured-file-parser
Receives structured txt file and creates a tree-like structure in memory.
Use a compiler that supports c++14. I used only STL features. 
The program responds to several errors: for example, missing parenthesis ({||}), or the beginning of the node's name with number.
I tested different entry files, program wokrs good. The order of variables in output (std::out, as well as file) may vary from 
source file slightly due to the recursive traversal of branches, but it does not affect the structure of the memory - each node knows
its variables, parents and children. For security reasons, instead of raw pointers shared use in conjunction with the weak, to
avoid circular references.
