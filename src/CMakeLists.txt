add_executable(BaseEngine
        main.cpp
        Core/GameEngine.cpp
        Core/Counter.cpp
        Subsystems/GameSubsystem.cpp
        Subsystems/InputSubsystem.cpp
        Subsystems/RendererSubsystem.cpp
)

target_link_libraries(BaseEngine
    PRIVATE
        SDL3::SDL3
        imgui
        "${CMAKE_SOURCE_DIR}/libs/opengl32.lib"
)