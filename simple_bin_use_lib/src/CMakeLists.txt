add_executable(helloCall call_hello.c)

target_link_directories(helloCall PRIVATE ${HELLOLIB_LIBRARY_DIRS})
target_link_libraries(helloCall ${HELLOLIB_LIBRARIES})
include_directories(${HELLOLIB_INCLUDEDIR})

install(TARGETS helloCall DESTINATION bin)
