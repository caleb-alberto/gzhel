# SFML
add_subdirectory(sfml)

set_target_properties(sfml-window PROPERTIES FOLDER "include/SFML")
set_target_properties(sfml-audio PROPERTIES FOLDER "include/SFML")
set_target_properties(sfml-graphics PROPERTIES FOLDER "include/SFML")
set_target_properties(sfml-network PROPERTIES FOLDER "include/SFML")
set_target_properties(sfml-system PROPERTIES FOLDER "include/SFML")

include_directories("${CMAKE_CURRENT_SOURCE_DIR}/SFML/include")

