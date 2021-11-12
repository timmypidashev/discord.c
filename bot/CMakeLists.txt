cmake_minimum_required(VERSION "3.21.0")

project(OneCoolBot LANGUAGES C)

add_executable(${PROJECT_NAME} client.c)

target_link_libraries(${PROJECT_NAME}
    PRIVATE discord
)