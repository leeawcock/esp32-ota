# This file was automatically generated for projects
# without default 'CMakeLists.txt' file.

# FILE(GLOB_RECURSE app_sources ${CMAKE_SOURCE_DIR}/src/*.*)

# idf_component_register(SRCS ${app_sources})

# from original CMakeLists.txt downloaded from Github source
set(COMPONENT_SRCS "main.c". 
                   "wifi.c")
set(COMPONENT_ADD_INCLUDEDIRS ".")
register_component()
# Embed the server root certificate into the final binary
# target_add_binary_data(${COMPONENT_TARGET} "server_certs/ca_cert_github.pem" TEXT)
# target_add_binary_data(${COMPONENT_TARGET} "server_certs/ca_cert_bitbucket.pem" TEXT)
# target_add_binary_data(${COMPONENT_TARGET} "server_certs/ca_cert_field.pem" TEXT)
# target_add_binary_data(${COMPONENT_TARGET} "server_certs/ca_cert_sharepoint.pem" TEXT)
target_add_binary_data(${COMPONENT_TARGET} "server_certs/ca_cert.pem" TEXT)