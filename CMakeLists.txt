cmake_minimum_required(VERSION 3.16...3.23)

project(
    "Game Engine Architecture"
    LANGUAGES CXX
    VERSION "0.1.0"
    DESCRIPTION "Following the book by Jason Gregory"
    HOMEPAGE_URL "https://github.com/Phytolizer/game-engine-architecture"
)

set(CMAKE_CXX_STANDARD 20)

include(FetchContent)
FetchContent_Declare(
    fmt
    GIT_REPOSITORY "https://github.com/fmtlib/fmt.git"
    GIT_TAG "8.1.1"
)
FetchContent_MakeAvailable(fmt)

FetchContent_Declare(
    spdlog
    GIT_REPOSITORY "https://github.com/gabime/spdlog.git"
    GIT_TAG "v1.9.2"
)
FetchContent_MakeAvailable(spdlog)
