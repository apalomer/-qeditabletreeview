# Tree item
QT4_WRAP_CPP(treeitem_moc   treeitem.h)
add_library(treeitem SHARED treeitem.cpp ${treeitem_moc})
target_link_libraries(treeitem ${QT_LIBRARIES})
