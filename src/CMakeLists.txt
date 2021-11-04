set(
    %{PROJECT_NAME}_HEADERS

)

set(
    %{PROJECT_NAME}_SOURCES
    main.cpp
)

add_executable(
    %{PROJECT_NAME}
    ${%{PROJECT_NAME}_HEADERS}
    ${%{PROJECT_NAME}_SOURCES}
)