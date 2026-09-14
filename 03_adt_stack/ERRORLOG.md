# ERRORLOG

## 1) September 13th, 2026 at 11:08 pm
I got the error "undefined reference to `Stack::peek() const'
collect2.exe: error: ld returned 1 exit status
mingw32-make[3]: *** [CMakeFiles\03_adt_stack.dir\build.make:117: 03_adt_stack.exe] Error 1
mingw32-make[2]: *** [CMakeFiles\Makefile2:180: CMakeFiles/03_adt_stack.dir/all] Error 2
mingw32-make[1]: *** [CMakeFiles\Makefile2:187: CMakeFiles/03_adt_stack.dir/rule] Error 2
mingw32-make: *** [Makefile:149: 03_adt_stack] Error 2."
The reason for getting this error was that I had commented out the peek method in "Stack.cpp" but forgotten I did that, so it called a method that wasn't defined. To fix that, I just removed the /* and the */

## 2) September 14th, 2026 at 1:38 pm
I got the error(s) "error: 'cout' was not declared in this scope; did you mean 'std::cout'?
   45 |         std:cout<<"Stack is empty, can't remove from it"<<std::endl;
      |             ^~~~
      |             std::cout
In file included from C:\Users\nawfa\CLionProjects\CS210CPPRepo\03_adt_stack\Stack.cpp:11:
C:/Users/nawfa/AppData/Local/Programs/CLion/bin/mingw/lib/gcc/x86_64-w64-mingw32/15.2.0/include/c++/iostream:65:18: note: 'std::cout' declared here
   65 |   extern ostream cout;          ///< Linked to standard output
      |                  ^~~~
C:\Users\nawfa\CLionProjects\CS210CPPRepo\03_adt_stack\Stack.cpp: In member function 'int Stack::peek() const':
C:\Users\nawfa\CLionProjects\CS210CPPRepo\03_adt_stack\Stack.cpp:60:55: warning: control reaches end of non-void function [-Wreturn-type]
   60 |         std::cout<<"Stack is empty, can't peek"<<std::endl;
      |                                                       ^~~~
mingw32-make[3]: *** [CMakeFiles\03_adt_stack.dir\build.make:92: CMakeFiles/03_adt_stack.dir/03_adt_stack/Stack.cpp.obj] Error 1
mingw32-make[2]: *** [CMakeFiles\Makefile2:180: CMakeFiles/03_adt_stack.dir/all] Error 2
mingw32-make[1]: *** [CMakeFiles\Makefile2:187: CMakeFiles/03_adt_stack.dir/rule] Error 2
mingw32-make: *** [Makefile:149: 03_adt_stack] Error 2
" I got this error because, as the suggestion says, I did forget a colon in the printing line while working on the functionality of peek. To fix it, I just added the colon.