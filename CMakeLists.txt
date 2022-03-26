cmake_minimum_required( VERSION 3.5 )

project( xwinwrap )

set( CMAKE_CXX_STANDARD 17 )

add_executable( xwinwrap
  xwinwrap.c
)

target_link_libraries( xwinwrap
  -lXrandr -lXext -lX11 -lrt
)