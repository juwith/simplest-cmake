add_library(helloLib SHARED hello_lib.c)

install (TARGETS helloLib
         LIBRARY DESTINATION lib)
