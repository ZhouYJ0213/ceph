
add_executable(unittest_seastore_journal
  test_seastore_journal.cc
  ../gtest_seastar.cc)
add_ceph_unittest(unittest_seastore_journal)
target_link_libraries(
  unittest_seastore_journal
  ${CMAKE_DL_LIBS}
  crimson-seastore)

add_executable(unittest_seastore_cache
  test_seastore_cache.cc
  ../gtest_seastar.cc)
add_ceph_unittest(unittest_seastore_cache)
target_link_libraries(
  unittest_seastore_cache
  ${CMAKE_DL_LIBS}
  crimson-seastore)
