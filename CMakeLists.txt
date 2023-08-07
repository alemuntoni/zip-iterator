cmake_minimum_required(VERSION 3.12)
project(ZipIterator)

add_executable(test_zip_two test_zip_two.cpp)
target_compile_features(test_zip_two PRIVATE cxx_std_17)

add_test(test_zip_two test_zip_two)


add_executable(test_zip_tuple test_zip_tuple.cpp)
target_compile_features(test_zip_tuple PRIVATE cxx_std_20)

add_test(test_zip_tuple test_zip_tuple)
