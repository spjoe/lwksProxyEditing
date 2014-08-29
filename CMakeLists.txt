cmake_minimum_required (VERSION 2.6)
project (lwksProxyEditing)

set (lwksProxyEditing_VERSION_MAJOR 0)
set (lwksProxyEditing_VERSION_MINOR 0)
set (lwksProxyEditing_VERSION_BUILD 1)

configure_file (
  "${PROJECT_SOURCE_DIR}/lwksProxyClipConverter"
  "${PROJECT_BINARY_DIR}/lwksProxyClipConverter"
  )
  
configure_file (
  "${PROJECT_SOURCE_DIR}/lwksChangeTo"
  "${PROJECT_BINARY_DIR}/lwksChangeTo"
  )

install (PROGRAMS ${PROJECT_BINARY_DIR}/lwksProxyClipConverter DESTINATION bin)
install (PROGRAMS lwksChangeToHigh DESTINATION bin)
install (PROGRAMS lwksChangeToProxy DESTINATION bin)
install (FILES ${PROJECT_BINARY_DIR}/lwksChangeTo DESTINATION include)
