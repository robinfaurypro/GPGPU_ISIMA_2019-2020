cmake_minimum_required(VERSION 3.15.3 FATAL_ERROR)

project(vulkan_lesson)

find_package(Vulkan REQUIRED)

add_executable(vulkan_lesson src/main.cpp)

target_include_directories(vulkan_lesson PRIVATE Vulkan::Vulkan)

target_link_libraries(vulkan_lesson Vulkan::Vulkan)

set_target_properties(vulkan_lesson PROPERTIES CXX_STANDARD 11)
