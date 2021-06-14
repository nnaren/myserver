message(${CMAKE_CURRENT_SOURCE_DIR}/../datetime)
message("Start make lib libmyserver.a")
include_directories(
    ${PROJECT_SOURCE_DIR}
)

aux_source_directory(. SRC_LIST)
file(GLOB SRC_DATETIME "../datetime/*.cc")
file(GLOB SRC_THREAD "../thread/*.cc")
file(GLOB SRC_LOGGING "../logging/*.cc")

add_library(myserver STATIC ${SRC_LIST} ${SRC_DATETIME} ${SRC_THREAD} ${SRC_LOGGING})