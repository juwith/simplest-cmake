add_library(helloLib SHARED hello_lib.c)

set_target_properties(helloLib PROPERTIES PUBLIC_HEADER "hello_lib.h")

install(TARGETS helloLib
		LIBRARY DESTINATION lib
		PUBLIC_HEADER DESTINATION include)
