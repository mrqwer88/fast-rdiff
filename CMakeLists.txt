cmake_minimum_required (VERSION 2.8)

# Install req: yum install -y openssl-devel log4cpp-devel

project(FastRdiff)

find_package(OpenSSL REQUIRED)

add_executable(fastrdiff fastrdiff.cpp)
target_link_libraries(fastrdiff ssl)
target_link_libraries(fastrdiff log4cpp)
