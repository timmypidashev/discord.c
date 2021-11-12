# cmake minimu required
# ----------------------------------
cmake_minimum_required(VERSION 3.21.0)

# set project name
# ----------------------------------
project(discord LANGUAGES C)

# sources
# ----------------------------------
set(SOURCES
    discord.c
    discord.h
)

# add library
add_library(
    ${PROJECT_NAME} STATIC ${SOURCES}
)

# Set Library Includes
# ----------------------------------
target_include_directories(${PROJECT_NAME} PUBLIC
    ${CMAKE_CURRENT_SOURCE_DIR}
)

# Set target link libraries
# ----------------------------------
# link any external dependencies here!