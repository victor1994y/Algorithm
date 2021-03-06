cmake_minimum_required(VERSION 3.6)
project(Algorithm)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++14")

#add_library(. DataStructures inked_list.hpp)

include_directories(
        ${PROJECT_SOURCE_DIR}
        ${PROJECT_SOURCE_DIR}/DataStructures
        ${PROJECT_SOURCE_DIR}/Algorithm
        ${PROJECT_SOURCE_DIR}/Tests)

set(SOURCE_FILES
        Algorithm/bucket_sort.h
        Algorithm/radix_sort.h
        DataStructures/linked_list.h
        DataStructures/list_node.h
        DataStructures/polynomial.h
        DataStructures/polynomial_unit.h
        Tests/bucket_sort.test.h
        Tests/linked_list.test.h
        Tests/list_node.test.h
        Tests/polynomial.test.h
        Tests/radix_sort.test.h
        main.cpp
        main.h
        utils.h
        optional.hpp
        DataStructures/stack.h Tests/stack.test.h Algorithm/symbol_pair_checker.cpp Algorithm/symbol_pair_checker.h Tests/symbol_pair_checker.test.h Algorithm/postfix_expression_manager.h Tests/postfix_expression_manager.test.h DataStructures/queue.h Tests/queue.test.h DataStructures/queue_based_on_array.h Tests/queue_based_on_array.test.h Algorithm/binary_search.h Algorithm/selection_sort.h Tests/selection_sort.test.h Algorithm/insertion_sort.h Tests/insertion_sort.test.h Algorithm/shell_sort.h Tests/shell_sort.test.h Algorithm/merge_sort.h Tests/merge_sort.test.h Algorithm/quick_sort.h Tests/quick_sort.test.h DataStructures/priority_queue.h Tests/priority_queue.test.h DataStructures/binary_heap.h Algorithm/heap_sort.h DataStructures/symbol_table.h DataStructures/symbol_table_elements.h DataStructures/tree_element.h DataStructures/2_3_tree.h DataStructures/binary_tree_node.h DataStructures/2_3_tree_node.h DataStructures/red_black_tree.h DataStructures/red_black_tree_node.h Tests/red_black_tree.test.h DataStructures/avl_tree.h Tests/avl_tree.test.h DataStructures/hash_table.h Tests/hash_table.test.h DataStructures/graph.h DataStructures/graph_adj_set.h Tests/graph.test.h Algorithm/graph_algorithm.h Tests/grapha_algorithm.test.h DataStructures/digraph.h Tests/digraph.test.h Algorithm/digraph_algorithm.h Tests/digraph_algorithm.test.h DataStructures/weighted_graph_adj_set.h DataStructures/weighted_graph.h Tests/weighted_graph.test.h Algorithm/weighted_graph_algorithm.h Tests/weighted_graph_algorithm.test.h Algorithm/union_find.h DataStructures/weighted_digraph.h Tests/weighted_digraph.test.h Algorithm/weighted_digraph_algorithm.h Tests/weighted_digraph_algorithm.test.h)

add_executable(Algorithm ${SOURCE_FILES})
