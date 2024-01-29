list(APPEND CMAKE_MODULE_PATH "${CMAKE_CURRENT_LIST_DIR}/cmake")

project(helloworld_go Go)

include(golang)

file(GLOB SRC_FILES CONFIGURE_DEPENDS
    ${CMAKE_CURRENT_SOURCE_DIR}/*.go
)

add_go_executable(${PROJECT_NAME} ${SRC_FILES})