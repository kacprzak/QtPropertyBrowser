
SET(example_name simple)

SET(KIT_SRCS
  main.cpp
  )
  
INCLUDE_DIRECTORIES(
  ${CMAKE_CURRENT_SOURCE_DIR}
  ${CMAKE_CURRENT_BINARY_DIR}
  )
  
ADD_EXECUTABLE(${example_name} ${KIT_SRCS})
QT5_USE_MODULES(${example_name} Widgets)
TARGET_LINK_LIBRARIES(${example_name} ${PROJECT_NAME})
