cmake_minimum_required(VERSION 3.12)

set(CPPM_VERSION 0.0.13)
include(cmake/cppm_loader.cmake)
cppm_project()

project(asio VERSION 1.18.2 LANGUAGES C CXX)
cppm_setting()
cppm_cxx_standard(17)
cppm_compiler_option(DEFAULT)



cppm_target_define(asio INTERFACE)


set(asio_global_deps )
cppm_target_dependencies(asio
   ${asio_global_deps})


cppm_target_install(asio)

