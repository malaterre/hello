project(hello)
add_library(foo SHARED foo.c)
set_target_properties(foo PROPERTIES VERSION 1.0 SOVERSION 0)
install(TARGETS foo
  RUNTIME DESTINATION bin
  LIBRARY DESTINATION lib
)
