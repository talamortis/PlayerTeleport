CU_SET_PATH("CMAKE_MALL_TELEPORT_DIR" "${CMAKE_CURRENT_LIST_DIR}")

AC_ADD_SCRIPT("${CMAKE_CURRENT_LIST_DIR}/src/mod-mall-teleport.cpp")

AC_ADD_SCRIPT_LOADER("MallTeleport"      "${CMAKE_CURRENT_LIST_DIR}/src/loader.h")

CU_ADD_HOOK(AFTER_WORLDSERVER_CMAKE "${CMAKE_CURRENT_LIST_DIR}/src/cmake/after_ws_install.cmake")

message("-- Mall Teleport CONFIGURED --")
