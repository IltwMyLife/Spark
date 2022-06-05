set(INCROOT ${PROJECT_SOURCE_DIR}/include/Spark)
set(SRCROOT ${PROJECT_SOURCE_DIR}/src/Spark)

set(SRC
    ${SRCROOT}/Main.cpp
)

add_executable(${PROJECT_NAME} ${SRC})

set_property(TARGET ${PROJECT_NAME} PROPERTY CXX_STANDARD 17)

target_link_libraries(${PROJECT_NAME} PRIVATE sfml-system sfml-window sfml-graphics)