cmake_minimum_required(VERSION 3.14 FATAL_ERROR)

project(MyProject)

include(cmake/CPM.cmake)

set(IMPL_GLFW OFF)
set(IMPL_SDL ON)
set(IMPL_OPENGL2 OFF)
set(IMPL_OPENGL3 ON)
set(IMGUI_FREETYPE OFF)
set(IMPL_EXTRAS ON)

CPMAddPackage(NAME LuaJIT-GL
    GITHUB_REPOSITORY sonoro1234/LuaJIT-GL
    GIT_TAG main
)

CPMAddPackage(NAME LuaJIT-SDL2
    GITHUB_REPOSITORY Simon-L/LuaJIT-SDL2
    GIT_TAG master
)

CPMAddPackage(NAME LuaJIT-ImGui
    GITHUB_REPOSITORY Simon-L/LuaJIT-ImGui
    GIT_TAG docking_inter
)



