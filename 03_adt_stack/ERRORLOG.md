# ERRORLOG

## 1) September 13th, 2026 at 11:08 pm
I got the error "undefined reference to `Stack::peek() const'
collect2.exe: error: ld returned 1 exit status
mingw32-make[3]: *** [CMakeFiles\03_adt_stack.dir\build.make:117: 03_adt_stack.exe] Error 1
mingw32-make[2]: *** [CMakeFiles\Makefile2:180: CMakeFiles/03_adt_stack.dir/all] Error 2
mingw32-make[1]: *** [CMakeFiles\Makefile2:187: CMakeFiles/03_adt_stack.dir/rule] Error 2
mingw32-make: *** [Makefile:149: 03_adt_stack] Error 2."
The reason for getting this error was that I had commented out the peek method in "Stack.cpp" but forgotten I did that, so it called a method that wasn't defined.