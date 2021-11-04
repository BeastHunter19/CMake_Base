set(
    %{PROJECT_NAME}_TEST_SOURCES
    test_main.cpp
)

add_executable(TestMain ${%{PROJECT_NAME}_TEST_SOURCES})
target_link_libraries(TestMain PRIVATE DocTest)
add_test(NAME MainTest COMMAND TestMain)