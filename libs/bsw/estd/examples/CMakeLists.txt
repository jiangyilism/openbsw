add_executable(
    estdExamples
    algorithm.cpp
    array.cpp
    big_endian.cpp
    constructor.cpp
    deque.cpp
    functional.cpp
    index_sequence.cpp
    indestructible.cpp
    iterator.cpp
    little_endian.cpp
    math.cpp
    memory.cpp
    multi_slice.cpp
    memory.cpp
    none.cpp
    optional.cpp
    ordered_map.cpp
    ordered_vector.cpp
    priority_queue.cpp
    ratio.cpp
    result.cpp
    ring.cpp
    string.cpp
    static_assert.cpp
    stack.cpp
    string_view.cpp
    singleton.cpp
    static_assert.cpp
    tiny_ring.cpp
    type_list.cpp
    type_traits.cpp
    typed_mem.cpp
    type_utils.cpp
    tuple.cpp
    uncopyable.cpp
    va_list_ref.cpp
    chrono.cpp
    bitset.cpp
    slice.cpp
    vec.cpp
    vector.cpp
    object_pool.cpp
    forward_list.cpp)

target_link_libraries(estdExamples PRIVATE estd estdMock gmock_main platform)

gtest_discover_tests(estdExamples PROPERTIES LABELS "estdExamples")
