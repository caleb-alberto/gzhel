# engine/core/CMakeLists.txt

file(GLOB_RECURSE CORE_SOURCE_FILES
    "src/*.h"
    "src/*.cpp"
)

set(SFML_DIR "${EXTERNAL_LIBRARIES_FOLDER}/sfml")

# Create a static library for "core"
add_library(core STATIC
    ${CORE_SOURCE_FILES}
)

target_include_directories(core PUBLIC "src")
target_include_directories(core PUBLIC ${EXTERNAL_LIBRARIES_FOLDER})
target_include_directories(core PUBLIC "${SFML_DIR}/include")
target_include_directories(core PUBLIC ${CMAKE_SOURCE_DIR}/engine)

target_link_libraries(core PUBLIC 
    sfml-graphics 
    sfml-window 
    sfml-system 
    sfml-audio 
    sfml-network 
)

set_target_properties(core PROPERTIES FOLDER "engine")
