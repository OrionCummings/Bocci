add_executable(Bocce
    main.c
    init.c
    debug.c
    drawing.c
    # networking.c
    # graphics.c
    # physics.c
    # resources.c
    # data_structures.c
    # database.c
    # cli.c
    )

target_include_directories(Bocce PUBLIC ../inc)

target_compile_options(Bocce PRIVATE
    -pedantic 
    -Wall 
    -Wextra 
    -Wconversion 
    -Wundef 
    -Werror  
    -Wno-unused-parameter
    -Wno-unused-variable
)
target_link_libraries(Bocce PRIVATE raylib)
