ADD_EXECUTABLE(multi_compile_uint main.cpp dummy.cpp)

IF (ENABLE_OPENSSL)
	ADD_DEFINITIONS(-DCINATRA_ENABLE_HTTPS)
ENDIF()

TARGET_LINK_LIBRARIES(multi_compile_uint ${EXTRA_LIBS})