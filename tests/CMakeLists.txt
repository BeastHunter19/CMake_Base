set(
    %{PROJECT_NAME}_TEST_SOURCES
    test_main.cpp
)

add_executable(TestMain ${%{PROJECT_NAME}_TEST_SOURCES})
target_include_directories(TestMain PRIVATE ${CMAKE_SOURCE_DIR}/src)
target_link_libraries(TestMain PRIVATE doctest::doctest)
add_test(NAME MainTest COMMAND TestMain)