cmake_minimum_required(VERSION 3.4.1)
set(lttp_src ${lttp_src})
list(APPEND lttp_src
        api.c
        http.c
        llhttp.c
)
include_directories(.)
add_library( llhttp
        STATIC
        ${lttp_src})