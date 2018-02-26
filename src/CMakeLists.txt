# Tree item
add_subdirectory(treeitem)

# Tree model
add_subdirectory(treemodel)

# Main  window
add_subdirectory(mainwindow)

# Main
add_executable(main main.cpp )
target_link_libraries(main ${QT_LIBRARIES} mainwindow)
