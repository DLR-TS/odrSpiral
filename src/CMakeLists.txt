# STATIC library
add_library(odrSpiral STATIC odrSpiral.c)
target_include_directories(odrSpiral PUBLIC ${PROJECT_SOURCE_DIR}/include)
set_property(TARGET odrSpiral PROPERTY POSITION_INDEPENDENT_CODE ON)

# Demo program
add_executable (odrSpiralDemo main.c)
if(WIN32)
  target_link_libraries (odrSpiralDemo LINK_PUBLIC odrSpiral)
else(WIN32)
  # Unix requires explicit static linking of math library "m" additionally
  target_link_libraries (odrSpiralDemo LINK_PUBLIC odrSpiral m)
endif(WIN32)
