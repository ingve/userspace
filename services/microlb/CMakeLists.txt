cmake_minimum_required(VERSION 2.8.9)
project (service C CXX)

option(PORTABLE "" OFF)
option(ENABLE_S2N "" ON)
include(../../userspace.cmake)

os_add_executable(linux_microlb "Linux userspace microLB test"
    service.cpp
  )
