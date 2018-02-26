# Tree model 
QT4_WRAP_CPP(treemodel_moc   treemodel.h)
add_library(treemodel SHARED treemodel.cpp ${treemodel_moc})
target_link_libraries(treemodel ${QT_LIBRARIES} treeitem)
