set(
        SRC_LIST
        OS.cpp
        OSCore.cpp
        OSPcb.cpp
        OSPcbManager.cpp
        OSSem.cpp
        OSSemManager.cpp
)

include_directories(
        ${PROJECT_SOURCE_DIR}/include/os/oscore
        ${PROJECT_SOURCE_DIR}/include/device/fs
        ${PROJECT_SOURCE_DIR}/include/device/processor
        ${PROJECT_SOURCE_DIR}/include/device/memory
        ${PROJECT_SOURCE_DIR}/include/config
        ${PROJECT_SOURCE_DIR}/include/os/scheduler
        ${PROJECT_SOURCE_DIR}/include/device/printer
        ${PROJECT_SOURCE_DIR}/include/device/voicer
)

add_library(oscore STATIC ${SRC_LIST})