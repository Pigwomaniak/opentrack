otr_module(migration BIN)
target_link_libraries(opentrack-migration opentrack-logic opentrack-spline)
if(CMAKE_COMPILER_IS_CLANGXX)
    target_compile_options(${self} PRIVATE "-Wno-weak-vtables")
endif()
