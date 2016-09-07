cmake_minimum_required(VERSION 3.5)
project(algorithms)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

set(SOURCE_FILES
    include/2darray.h
    include/8queen.h
    include/astar.h
    include/avl.h
    include/base64.h
    include/bellman_ford.h
    include/binary_search_tree.h
    include/bitset.h
    include/bloom_filter.h
    include/btree.h
    include/bubble_sort.h
    include/dictionary.h
    include/dijkstra.h
    include/directed_graph.h
    include/disjoint-set.h
    include/dos_tree.h
    include/double_linked_list.h
    include/edmonds_karp.h
    include/fenwick_tree.h
    include/fib-heap.h
    include/generic.h
    include/graph_defs.h
    include/graph_search.h
    include/hash_code.h
    include/hash_multi.h
    include/hash_string.h
    include/hash_table.h
    include/heap.h
    include/huffman.h
    include/imath.h
    include/insertion_sort.h
    include/integer.h
    include/interval_tree.h
    include/k-means.h
    include/kmp.h
    include/kruskal_mst.h
    include/lcs.h
    include/LRU_cache.h
    include/max_subarray.h
    include/md5.h
    include/merge_sort.h
    include/palindrome.h
    include/perfect_hash.h
    include/prim_mst.h
    include/prime.h
    include/priority_queue.h
    include/queue.h
    include/quick_sort.h
    include/radix_sort.h
    include/random.h
    include/random_select.h
    include/rbtree.h
    include/rbtree_defs.h
    include/relabel_to_front.h
    include/scc.h
    include/selection_sort.h
    include/sha1.h
    include/shell_sort.h
    include/shuffle.h
    include/simhash.h
    include/skiplist.h
    include/sol.h
    include/sort.h
    include/stack.h
    include/suffix_array.h
    include/suffix_tree.h
    include/trie.h
    include/undirected_graph.h
    include/universal_hash.h
    include/word_seg.h
    msvc/alg_vs.h
    msvc/stdbool.h
    src/8queue_demo.cpp
    src/astar_demo.cpp
    src/avl_demo.cpp
    src/base64_demo.cpp
    src/bellman_ford_demo.cpp
    src/binary_search_tree_demo.cpp
    src/bitset_demo.cpp
    src/bloom_filter_demo.cpp
    src/btree_demo.cpp
    src/bubble_sort_demo.cpp
    src/dictionary_demo.cpp
    src/dijkstra_demo.cpp
    src/directed_graph_demo.cpp
    src/disjoint-set_demo.cpp
    src/dos_tree_demo.cpp
    src/double_linked_list_demo.cpp
    src/edmonds_karp_demo.cpp
    src/fenwick_tree_demo.cpp
    src/fib-heap_demo.cpp
    src/graph_demo.cpp
    src/graph_search_demo.cpp
    src/hash_multi_demo.cpp
    src/hash_string_demo.cpp
    src/hash_table_demo.cpp
    src/heap_demo.cpp
    src/huffman_demo.cpp
    src/imath_demo.cpp
    src/insertion_sort_demo.cpp
    src/integer_demo.cpp
    src/interval_tree_demo.cpp
    src/k-means_demo.cpp
    src/kmp_demo.cpp
    src/kruskal_mst_demo.cpp
    src/lcs_demo.cpp
    src/LRU_cache_demo.cpp
    src/m_based_demo.cpp
    src/max_subarray_demo.cpp
    src/md5_demo.cpp
    src/merge_sort_demo.cpp
    src/palindrome_demo.cpp
    src/perfect_hash_demo.cpp
    src/prim_mst_demo.cpp
    src/prime_decompose.c
    src/prime_demo.cpp
    src/priority_queue_demo.cpp
    src/queue_demo.cpp
    src/quick_sort_demo.cpp
    src/radix_sort_demo.cpp
    src/random_demo.cpp
    src/random_select_demo.cpp
    src/rbtree_demo.cpp
    src/relabel_to_front_demo.cpp
    src/scc_demo.cpp
    src/selection_sort_demo.cpp
    src/sha1_demo.cpp
    src/shell_sort_demo.cpp
    src/shuffle_demo.cpp
    src/simhash_demo.cpp
    src/skiplist_demo.cpp
    src/sort_demo.cpp
    src/stack_demo.cpp
    src/suffix_array_demo.cpp
    src/suffix_tree_demo.cpp
    src/trie_demo.cpp
    src/undirected_graph_demo.cpp
    src/universal_hash_demo.cpp
    src/word_seg_demo.cpp
    utils/byteorder.h
    utils/gb18030.h
    LICENSE
    README.md)

add_executable(algorithms ${SOURCE_FILES})

add_executable(8queue_demo src/8queue_demo.cpp include/8queen.h)
add_executable(astar_demo src/astar_demo.cpp include/astar.h)
add_executable(avl_demo src/avl_demo.cpp include/avl.h)
add_executable(base64_demo src/base64_demo.cpp include/base64.h)
add_executable(bellman_ford_demo src/bellman_ford_demo.cpp include/bellman_ford.h)
add_executable(binary_search_tree_demo src/binary_search_tree_demo.cpp include/binary_search_tree.h)
add_executable(bitset_demo src/bitset_demo.cpp include/bitset.h)
add_executable(bloom_filter_demo src/bloom_filter_demo.cpp include/bloom_filter.h)
add_executable(btree_demo src/btree_demo.cpp include/btree.h)
add_executable(bubble_sort_demo src/bubble_sort_demo.cpp include/bubble_sort.h)
add_executable(dictionary_demo src/dictionary_demo.cpp include/dictionary.h include/hash_table.h include/random.h)
add_executable(dijkstra_demo src/dijkstra_demo.cpp include/directed_graph.h include/dijkstra.h)
add_executable(directed_graph_demo src/directed_graph_demo.cpp include/directed_graph.h)
add_executable(disjoint_set_demo src/disjoint-set_demo.cpp include/disjoint-set.h)
add_executable(dos_tree_demo src/dos_tree_demo.cpp include/dos_tree.h)
add_executable(double_linked_list_demo src/double_linked_list_demo.cpp include/sol.h include/double_linked_list.h)
add_executable(edmonds_karp_demo src/edmonds_karp_demo.cpp include/edmonds_karp.h)
add_executable(fenwick_tree_demo src/fenwick_tree_demo.cpp include/fenwick_tree.h)
add_executable(fib-heap_demo src/fib-heap_demo.cpp include/fib-heap.h)
add_executable(graph_demo src/graph_demo.cpp include/undirected_graph.h)
add_executable(graph_search_demo src/graph_search_demo.cpp include/directed_graph.h include/graph_search.h)
add_executable(hash_multi_demo src/hash_multi_demo.cpp include/hash_multi.h)
add_executable(hash_string_demo src/hash_string_demo.cpp include/hash_string.h)
add_executable(hash_table_demo src/hash_table_demo.cpp include/hash_table.h)
add_executable(heap_demo src/heap_demo.cpp include/heap.h)
add_executable(huffman_demo src/huffman_demo.cpp include/huffman.h)
add_executable(imath_demo src/imath_demo.cpp include/imath.h)
add_executable(insertion_sort_demo src/insertion_sort_demo.cpp include/generic.h include/insertion_sort.h)
add_executable(integer_demo src/integer_demo.cpp include/integer.h)
add_executable(interval_tree_demo src/interval_tree_demo.cpp include/interval_tree.h)
add_executable(k-means_demo src/k-means_demo.cpp include/k-means.h)
add_executable(kmp_demo src/kmp_demo.cpp include/kmp.h)
add_executable(kruskal_mst_demo src/kruskal_mst_demo.cpp include/undirected_graph.h include/kruskal_mst.h)
add_executable(lcs_demo src/lcs_demo.cpp include/lcs.h)
add_executable(LRU_cache_demo src/LRU_cache_demo.cpp include/LRU_cache.h)
add_executable(m_based_demo src/m_based_demo.cpp include/imath.h include/prime.h)
add_executable(max_subarray_demo src/max_subarray_demo.cpp include/max_subarray.h)
add_executable(md5_demo src/md5_demo.cpp include/md5.h)
add_executable(merge_sort_demo src/merge_sort_demo.cpp include/merge_sort.h)
add_executable(palindrome_demo src/palindrome_demo.cpp include/palindrome.h)
add_executable(perfect_hash_demo src/perfect_hash_demo.cpp include/perfect_hash.h)
add_executable(prim_mst_demo src/prim_mst_demo.cpp include/undirected_graph.h include/prim_mst.h)
add_executable(prime_demo src/prime_demo.cpp include/prime.h)
add_executable(priority_queue_demo src/priority_queue_demo.cpp include/priority_queue.h)
add_executable(queue_demo src/queue_demo.cpp include/queue.h)
add_executable(quick_sort_demo src/quick_sort_demo.cpp include/quick_sort.h)
add_executable(radix_sort_demo src/radix_sort_demo.cpp include/radix_sort.h)
add_executable(random_demo src/random_demo.cpp include/random.h)
add_executable(random_select_demo src/random_select_demo.cpp include/random_select.h)
add_executable(rbtree_demo src/rbtree_demo.cpp include/rbtree.h)
add_executable(relabel_to_front_demo src/relabel_to_front_demo.cpp include/edmonds_karp.h include/relabel_to_front.h)
add_executable(scc_demo src/scc_demo.cpp include/scc.h)
add_executable(selection_sort_demo src/selection_sort_demo.cpp include/selection_sort.h)
add_executable(sha1_demo src/sha1_demo.cpp include/sha1.h)
add_executable(shell_sort_demo src/shell_sort_demo.cpp include/shell_sort.h)
add_executable(shuffle_demo src/shuffle_demo.cpp include/shuffle.h)
add_executable(simhash_demo src/simhash_demo.cpp include/simhash.h)
add_executable(skiplist_demo src/skiplist_demo.cpp include/skiplist.h)
add_executable(sort_demo src/sort_demo.cpp include/sort.h)
add_executable(stack_demo src/stack_demo.cpp include/stack.h)
add_executable(suffix_demo src/suffix_array_demo.cpp include/suffix_array.h)
add_executable(suffix_tree_demo src/suffix_tree_demo.cpp include/suffix_tree.h)
add_executable(trie_demo src/trie_demo.cpp include/trie.h)
add_executable(undirected_graph_demo src/undirected_graph_demo.cpp include/undirected_graph.h)
add_executable(universal_hash_demo src/universal_hash_demo.cpp include/universal_hash.h)
add_executable(word_seg_demo src/word_seg_demo.cpp include/word_seg.h)