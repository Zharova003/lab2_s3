cmake_minimum_required(VERSION 3.17)
project(lab2_s3)

set(CMAKE_CXX_STANDARD 14)
add_subdirectory(gtest/googletest)

include_directories(gtest/googletest/googletest/include)
add_executable(lab2_s3 main.cpp SparceVector.h Histogram.h Person.h Dictionary.h BinaryTree.h ArraySequence.h Sequence.h LinkedListSequence.h LinkedList.h DynamicArray.h AlphabetIndex.h Interface.h Tests.cpp)
target_link_libraries(lab2_s3 gtest)