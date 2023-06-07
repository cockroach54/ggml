#
# polyglot6b

set(TEST_TARGET polyglot6b)
add_executable(${TEST_TARGET} main.cpp)
target_link_libraries(${TEST_TARGET} PRIVATE ggml common common-ggml)

#
# polyglot6b-quantize

set(TEST_TARGET polyglot6b-quantize)
add_executable(${TEST_TARGET} quantize.cpp)
target_link_libraries(${TEST_TARGET} PRIVATE ggml common common-ggml)
