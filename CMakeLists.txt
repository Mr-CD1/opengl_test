cmake_minimum_required(VERSION 3.0.0)
project(opengl_test VERSION 0.1.0 LANGUAGES C CXX)

include_directories(includes)
link_libraries("${PROJECT_SOURCE_DIR}/lib/glfw3.lib") #链接之前生成的静态库文件


aux_source_directory(./src DIR_ALL_SRC)	
add_executable(${PROJECT_NAME} ${DIR_ALL_SRC}) 