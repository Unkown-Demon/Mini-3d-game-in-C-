cmake_minimum_required(VERSION 3.10)
project(Simple3DGame CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# Find necessary packages
find_package(OpenGL REQUIRED)
find_package(GLEW REQUIRED)
find_package(glfw3 REQUIRED)
# GLM is header-only and installed via libglm-dev, so we don't need find_package
# find_package(GLM REQUIRED)

# Add source files
file(GLOB_RECURSE SOURCE_FILES "src/*.cpp")

# Create executable
add_executable(Simple3DGame ${SOURCE_FILES})

# Link libraries
target_link_libraries(Simple3DGame
    PRIVATE
        OpenGL::GL
        GLEW::GLEW
        glfw
# GLM::GLM is not needed as it's header-only
)

# Set output directory
set_target_properties(Simple3DGame PROPERTIES RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin)
