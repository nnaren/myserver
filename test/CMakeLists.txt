include_directories(
    ${PROJECT_SOURCE_DIR}
)
set(TEST test11)
Set(Sources
    ${TEST}.cc
)
add_executable(${TEST} ${Sources})
target_link_libraries(${TEST} myserver pthread)