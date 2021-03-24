add_library(fontcache SHARED SDL_FontCache.h SDL_FontCache.c)
find_package(PkgConfig)
pkg_check_modules(SDL2 REQUIRED sdl2 SDL2_ttf)
target_link_libraries(fontcache ${SDL2_LIBRARIES})
