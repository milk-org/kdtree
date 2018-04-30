project(lib_kdtree_project)

include_directories ("${PROJECT_SOURCE_DIR}/src")
include_directories ("${PROJECT_SOURCE_DIR}/..")
add_library(kdtree SHARED kdtree.c)

install(TARGETS kdtree DESTINATION lib)
install(FILES kdtree.h DESTINATION include)

