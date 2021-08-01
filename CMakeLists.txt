add_library(iw-ev STATIC ev.c)
target_compile_definitions(iw-ev PUBLIC EV_STANDALONE=1 EV_CHILD_ENABLE=0)
target_include_directories(iw-ev PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
