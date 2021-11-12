# set cmake minimum required
# ----------------------------------
cmake_minimum_required(VERSION 3.21.0)

# set project
# ----------------------------------
project(libdiscord VERSION 0.1.0 LANGUAGES C)

# setup cmake package
# ----------------------------------
# set(PACKAGE discord)
# set(CPACK_PACKAGE_NAME discord)

# Compilation
# ----------------------------------
set(CMAKE_C_STANDARD 99)

# add subdirectories
# ----------------------------------
add_subdirectory(lib)

# for debugging purposes, the bot is built with the library for now :)
# ----------------------------------
add_subdirectory(bot)