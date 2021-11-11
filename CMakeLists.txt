add_library(fontcache STATIC SDL_FontCache.h SDL_FontCache.c)
find_package(SDL2 REQUIRED)
find_package(SDL2_ttf REQUIRED)
target_link_libraries(fontcache ${SDL2_LIBRARIES} ${SDL2_TTF_LIBRARIES})
