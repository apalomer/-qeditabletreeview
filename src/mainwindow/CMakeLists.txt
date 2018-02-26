# Main window 
QT4_WRAP_CPP(mainwindow_moc mainwindow.h)
QT4_WRAP_UI(mainwindow_ui mainwindow.ui)
add_library(mainwindow SHARED mainwindow.cpp ${mainwindow_moc} ${mainwindow_ui})
target_link_libraries(mainwindow ${QT_LIBRARIES} treemodel)
