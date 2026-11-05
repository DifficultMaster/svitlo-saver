include(FetchContent)

FetchContent_Declare(
	grpc
	GIT_REPOSITORY https://github.com/grpc/grpc.git
    GIT_TAG v1.83.2
    GIT_SUBMODULES_RECURSE TRUE
)

FetchContent_MakeAvailable(grpc)

set(PROTO_DIR "${CMAKE_SOURCE_DIR}/shared/proto")

add_executable(SvitloSaver_core
	src/main.cpp
)

target_include_directories(SvitloSaver_core PRIVATE
	include
)

